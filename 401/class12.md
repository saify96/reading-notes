# Spring RequestMapping

### The annotation is used to map web requests to Spring Controller methods.
- @RequestMapping — by Path
- @RequestMapping — the HTTP Method
- RequestMapping and HTTP Headers
  - 3.1. @RequestMapping With the headers Attribute
  - RequestMapping Consumes and Produces
- RequestMapping With Path Variables
  - Single @PathVariable
  - Multiple @PathVariable
  - @PathVariable With Regex
- RequestMapping With Request Parameters
  - RequestMapping Corner Cases
  - @RequestMapping — Multiple Paths Mapped to the Same Controller Method
  - @RequestMapping — Multiple HTTP Request Methods to the Same Controller Method 
  - @RequestMapping — a Fallback for All Requests Ambiguous Mapping Error
- New Request Mapping Shortcuts
- Spring Framework 4.3 introduced a few new HTTP mapping annotations, all based on @RequestMapping:
  - @GetMapping
  - @PostMapping
  - @PutMapping
  - @DeleteMapping
  - @PatchMapping


# Accessing Data with JPA
- Define a Simple Entity.
- Create Simple Queries.
  - Spring Data JPA focuses on using JPA to store data in a relational database.
- Create an Application Class.
- Build an executable JAR.

# Spring Data repository interfaces
- Spring Data Repositories:
  - CrudRepository provides CRUD functions.
  - PagingAndSortingRepository provides methods to do pagination and sort records.
  - JpaRepository provides JPA related methods such as flushing the persistence context and delete records in a batch.
- JpaRepository contains the full API of CrudRepository and PagingAndSortingRepository.


