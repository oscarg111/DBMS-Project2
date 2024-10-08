Project 2: Indexing for Relational Algebra Operators

This project focuses on enhancing the performance of relational algebra operations by incorporating indexing mechanisms. Building on the foundational operations from Project 1, Project 2 introduces the use of indices to optimize data retrieval and manipulation.

Relational Algebra Operations with Indexing:
The following operations have been optimized using indexing techniques, making the project more efficient in handling large datasets:

Select (Indexed Select):
Implements an indexed selection operation, allowing for faster retrieval of rows that match a given condition by utilizing an index to quickly locate matching tuples.

Project (Duplicate Elimination):
Enhances the Project operation by efficiently eliminating duplicate tuples using indexing, ensuring that the final output only contains unique rows.

Union (Duplicate Elimination):
Uses indexing to efficiently combine two tables, eliminating duplicates to return all unique rows from both tables without needing a full scan of each table.

Minus (Tuple Existence Check):
Optimizes the Minus operation by checking if each tuple in table r exists in table s using an index, improving the speed of the subtraction process.

Join (Indexed Join):
Implements an indexed join operation, where tables are merged based on common attributes. The use of indices speeds up the matching process, making joins more efficient.

Indexing Implementation:
A BpTreeMap is used to implement the indices, providing an efficient mechanism for searching, inserting, and deleting tuples in the table.
