# GUI-Based Java Project

## 📋 Project Overview       
To build a two-player GUI-based Chess game in Java, focusing on game rules, move validation, and an interactive interface. The project helps improve skills in object-oriented programming and GUI development.

---

## ✅ 1. 🛠️ Development Setup (2 Marks)

### ✅ JDK Version         
- **JDK Version**: `Java SE Development Kit 17`
- Make sure JDK 17 is installed and configured in your environment.
- [Download JDK](https://www.oracle.com/java/technologies/javase-downloads.html)

### ✅ IDE Used
- **IDE**: `IntelliJ IDEA Community Edition 2023`
- You may also use `Eclipse` or `VS Code` with Java extensions.
   
---

## ✅ 2. ✅ Project Structure       (1 Marks)
- The project Structure in already given in a text file `CheckMate ## Project Structure.txt`

---

## ✅ 3. 🗃️ Database Schema Design (1 Marks)
The project uses a MySQL database to store chess game details and move history.

---
 
## ✅ 4. 📂 MySQL Tables   (1 Marks)

- **Game**  
  Stores the overall game information like player names, winner, and timestamps.

- **MoveHistory**  
  Stores each move made in a game, including notation, origin/destination squares, and timestamps.
  
- SQL Schema File

The database schema is defined in [`schema.sql`](schema.sql), which includes:
 

```sql
CREATE TABLE Game (...);
CREATE TABLE MoveHistory (...);
```

---

 
## ✅ 5. JDBC Implementation (3 Marks)

We've successfully implemented JDBC to enable interaction between our Java Chess game and a MySQL database.

- A dedicated `DatabaseConnection.java` class was created to handle the database connection logic.
- JDBC is used to connect the Java application to a MySQL database (`chessdb`).
- This connection will support storing and retrieving move history or other game-related data in future extensions.

### 📄 `DatabaseConnection.java` Highlights

```java
package com.chess.database;

import java.sql.Connection;
import java.sql.DriverManager;
import java.sql.SQLException;

public class DatabaseConnection {
    private static final String URL = "jdbc:mysql://localhost:3306/chessdb";
    private static final String USER = "root";
    private static final String PASSWORD = "yourpassword";

    public static Connection getConnection() throws SQLException {
        return DriverManager.getConnection(URL, USER, PASSWORD);
    }
}
```

---

## ✅ 6. Create Model & DAO (3 Marks)
To manage database interactions cleanly and efficiently, we implemented:

🧩 MoveRecord.java (Model)
This class represents a single record of a chess move. It includes:

moveNumber – The sequential number of the move.

whiteMove – Move made by the White player.

blackMove – Move made by the Black player. 
