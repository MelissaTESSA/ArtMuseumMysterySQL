Alright! Let's create a more complex scenario with multiple tables that require various SQL operations, including JOINs, to retrieve information. I'll provide you with a fictional scenario, tables with sample data, and questions to answer using SQL.

### **Scenario: "The Art Museum Mystery"**:

An ancient artifact goes missing from a city's renowned art museum. The detective division creates a SQLite database to keep track of everyone involved, and clues related to the case.

**Tables & Sample Data**:

1. `Employees` (museum employees details)
    - Columns: `employeeID, firstName, lastName, position`

    | employeeID | firstName | lastName | position       |
    |------------|-----------|----------|----------------|
    | 1          | John      | Doe      | Security       |
    | 2          | Emily     | Smith    | Curator        |
    | 3          | Alan      | White    | Guide          |

2. `Visitors` (details about visitors on the day of the theft)
    - Columns: `visitorID, firstName, lastName, countryOfOrigin`

    | visitorID | firstName | lastName | countryOfOrigin |
    |-----------|-----------|----------|-----------------|
    | 1         | Michael   | Brown    | USA             |
    | 2         | Sarah     | Green    | UK              |
    | 3         | Felix     | Gray     | Germany         |

3. `Suspects` (details about the prime suspects)
    - Columns: `suspectID, type (Visitor/Employee), typeID (the ID from either Visitor or Employee table), reason`

    | suspectID | type     | typeID | reason                |
    |-----------|----------|--------|-----------------------|
    | 1         | Visitor  | 2      | Found near crime scene|
    | 2         | Employee | 1      | Previous theft record |

4. `Clues` (clues found at the museum)
    - Columns: `clueID, description, foundByEmployeeID`

    | clueID | description              | foundByEmployeeID |
    |--------|--------------------------|-------------------|
    | 1      | A torn piece of paper    | 3                 |
    | 2      | A silver pendant         | 1                 |

### **Questions**:

1. Retrieve the names of all suspects and their reasons for suspicion.
2. Find out the total number of visitors from each country on the day of the theft.
3. Identify which employee found the most clues.
4. List the clues found by John Doe.
5. Which position in the museum had the most employees listed as suspects?
6. Get a list of all employees who haven’t found any clues.
7. Were there more visitor suspects or employee suspects?
8. Identify the country of origin of all visitor suspects.
9. List the reasons why employees were suspected.
10. Which clues were found by employees holding the position of "Guide"?
