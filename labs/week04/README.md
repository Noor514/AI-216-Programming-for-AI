
**Explanation **

In this lab, different built-in Python data structures were used based on the nature of the problem:

Lists were used for ordered and mutable collections such as product prices, because they allow sorting, filtering, and iteration.

Tuples were used to represent fixed records like geographic coordinates and product details (name, price, quantity), as they ensure data immutability.

Sets were used for handling uniqueness, such as tracking enrolled students and avoiding duplicate product names.

Dictionaries were used to represent structured and categorized data, such as employee records, sales data, and inventory systems, because they provide efficient key-based access.

These data structures were sometimes combined (e.g., dictionary of lists containing tuples) to model real-world systems more effectively.

**Why They Were Appropriate?**

Lists were appropriate for data requiring ordering, sorting, and filtering operations.

Tuples were suitable for fixed data records where values should not be modified accidentally.

Sets ensured uniqueness and made membership checking efficient.

Dictionaries allowed structured organization of related data using meaningful keys, improving readability and scalability.

Using the correct data structure made the programs more efficient, readable, and logically organized.

**Challenges Faced**

Managing nested data structures such as dictionaries containing lists of tuples

Updating tuple-based records (since tuples are immutable)

Ensuring uniqueness of product names using sets

Performing nested iteration for aggregation and reporting tasks
