## Many to Many relationships 

To execute Many to Many relationships First of all,
## Database Setup :
- create the employee and project tables along with the employee_project join table with employee_id and project_id

## Prepare The model classes Employee and Project need to be created with JPA annotations:
- Both the Employee class and Project classes refer to one another, which means that the association between them is bidirectional.

- In order to map a many-to-many association, we use the @ManyToMany, @JoinTable and @JoinColumn annotations. Let's have a closer look at them.

- The @ManyToMany annotation is used in both classes to create the many-to-many relationship between the entities.

- This association has two sides i.e. the owning side and the inverse side. 

- The @JoinColumn annotation is used to specify the join/linking column with the main table.
