# Plasticine Soldier Collection Database

This project is a personal SQL database designed to document and organize a collection of hand-made plasticine soldier figurines. It uses SQLite and DB Browser for SQLite to store structured information such as soldier type, colors used, accessories, and creation date.

## Project Overview

The database tracks relevant details for each plasticine sfigures in the collection, including:

- Name of the figure
- Type (e.g., infantry, archer, knight)  
- Gender
- Eye Color
- Height in centimeters  
- Colors used  
- Accessories (e.g., sword, shield)  
- Show the figure was from if it was based on a character from a show 
- Freeform notes or descriptions  

## Tools Used

| Tool                   | Purpose                                 |
|------------------------|-----------------------------------------|
| SQLite                 | Lightweight relational database         |
| DB Browser for SQLite  | GUI for database management             |
| SQL                    | Creating tables and querying data       |

## Table Structure

```sql
CREATE TABLE Soldiers (
    SoldierID INTEGER PRIMARY KEY AUTOINCREMENT,
    Name TEXT NOT NULL,
    Gender TEXT,
    Eye Color TEXT,
    HeightCM REAL,
    Type TEXT,
    ColorsUsed TEXT,
    Accessories TEXT,
    Show TEXT, 
    Notes TEXT
);
