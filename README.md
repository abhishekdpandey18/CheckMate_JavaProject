# GUI-Based Java Project

## 📋 Project Overview       
To build a two-player GUI-based Chess game in Java, focusing on game rules, move validation, and an interactive interface. The project helps improve skills in object-oriented programming and GUI development.

---

## 🛠️ Development Setup         

### ✅ JDK Version         ✔2
- **JDK Version**: `Java SE Development Kit 17`
- Make sure JDK 17 is installed and configured in your environment.
- [Download JDK](https://www.oracle.com/java/technologies/javase-downloads.html)

### ✅ IDE Used
- **IDE**: `IntelliJ IDEA Community Edition 2023`
- You may also use `Eclipse` or `VS Code` with Java extensions.

---
## 🗃️ Database Schema Design

The project uses a MySQL database to store chess game details and move history.

### 📂 Tables

- **Game**  
  Stores the overall game information like player names, winner, and timestamps.

- **MoveHistory**  
  Stores each move made in a game, including notation, origin/destination squares, and timestamps.

### 📄 SQL Schema File

The database schema is defined in [`schema.sql`](schema.sql), which includes:

```sql
CREATE TABLE Game (...);
CREATE TABLE MoveHistory (...);


