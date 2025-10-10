# Ruby on Rails Topics

<details>
<summary>List of all questions:</summary>

```
1.What is the difference between has_many :through and has_and_belongs_to_many? Also state which one is better?

2.What are validations in rails? At what moments of an object's lifecycle validations are checked?

3.What do you mean by polymorphic association in rails? When can one use this association?

4.What are scopes in Rails?

5.What is the difference between class methods and scopes? Are they similar?

6.What do you mean by ActiveRecord callbacks? Explain some ActiveRecord callbacks.

7.How can you define custom validations in rails?

8.What do you mean by STI(single table inheritance)? What are its advantages and disadvantages?

9.What do you mean by migrations in Rails? What is the usage of rails migrations?

10.What do you mean by N+1 query? How can you resolve N+1 query? Explain by an example.

11.What is the difference between includes and joins?

12.What do you mean by self_join association in Rails?

13.What do you mean by ORM? Explain.

14.Is it possible to change the convention of naming a table in rails? If yes, how will you do this? Please explain.

15.What do you mean by Rolling back a migration? How can you rollback a specific migration?

16.What are the Relational and Conditional callbacks in ActiveRecord? Explain them.

17.What are transactional callbacks? Explain them.

18.What do you mean by member and collection routes? Explain.

19.What do you know about namespace and scoped routing? What is the difference between both?

20.Explain the difference between webpacker and sprockets.

21.How many types of associations are in rails?

22.What do you mean by partials in Rails? Explain the usage of partials and the way we can pass local variables to a partial.

23.What are delegates in Rails? Explain usage of delegates.

24.What do you mean by helper classes? Explain.

25.What do you mean by mailers? How many ways to pass arguments to a mailer?

26.What do you mean by concerns in Rails? Explain the way of using a concern.

27.Have you ever used sidekiq? Explain how it works in both production and development environments?

28.What is the difference between a sidekiq worker and rails ActiveJob?

29.What do you mean by rake tasks? How can you define/implement custom rake tasks?

30.Do you know about ActiveStorage? How can you use this?

31.Explain strong parameters.

32.How do you pass default arguments to a controller action where you instantiate a new model object?

33.What are turbolinks into rails?

34.What do you mean by API versioning in Rails? Explain when there is a need to change the version of an API?

35.What is the difference between before_save, before_create and before_update?

36.What do you mean by asset pipeline?

37.What do you mean by default_scope? Please explain.

38.Explain routing in rails.

39.What do you mean by filter actions or controller callbacks? Explain.

40.How can you handle ActiveRecord::RecordNotFound exception for all resources?

41.How many gems for the admin backend have you used? Which gem is better and why?

42.You are asked to implement an admin backend for a web application. What solution will you propose? Any gem or custom admin panel? Also explain the reason.

43. What is the difference between save and save!?

44. How can you pass params to a mailer action?

45. Is it possible to replace the schema.rb file in Rails? If yes, how can you do this?

46. What is ActionCable? Explain.

47. How can you implement user authentication using devise and JWT? Explain the process of it.

48. How many form helpers are provided by rails? Tell the names and differences between them.

49. What is the difference between delete and destroy in Rails?

50. How do you organize your controllers? Tell me about the way that you can make a controller thin.

51. What do you mean by sessions in Rails? In what circumstances do you need to use sessions? Explain.

52. What is the find_each method in Rails? Also explain why the .all method is not ideal to use for loading all the instances of a model at once?

53. What is polymorphic association in Rails? When should you actually use a polymorphic association?

54. What is the difference between eager_load and includes methods? And which one is better?

55. Which of the methods is faster between delete and destroy? Explain why?

56. What is the difference between ActiveModel and ActiveRecord?

57. What is the difference between dependent: :destroy and dependent: :delete_all?

58. What is yield in Ruby? What happens if you call the method, which includes yield, without passing a block?

59. What is the difference between Hash and HashWithIndifferentAccess?

60. In Ruby, how many ways to invoke a method? Illustrate with examples.

61. In Ruby, what is the difference between Strings and Symbols? Explain.

62. What do you mean by schema versioning in Rails? When does it change?

63. What do you mean by reversible migrations?

64. How can you run/rollback any specific migration in Rails?

65. When should you use an up and down method instead of a change method inside your migration? Explain by an example.

66. What is shallow nesting of routes and when is preferable to use this?

67. What do you mean by meta Programming in Ruby? Explain how you can implement this in your program?

68. What do you mean by inject method in Ruby?

69. What is the difference between equal? and eql? method in Ruby?

70. What is the advantage of using hash over an array in Ruby?

71. What is the difference between iterators and loops in Ruby?

72. What are accessor methods in Ruby? List and explain accessor methods.

73. What are class level and module level attributes?

74. What is the difference between include and extend in rails?

75. How many template engines are supported by Rails? Which one is your preference and why?

76. What do you mean by singleton (Eigen) class in Ruby?

77. When do you think is the right time to define a helper method inside a controller in Rails?

78. What is your understanding of DRY code? Explain.

79. What is your approach to write a thin controller? Also explain why a controller should be thin and what are the advantages of it?

80. What is the purpose of initializers directory in a rails project?

81. What is the difference between a gem and Rails engine?

82. What do you mean by a rails engine? Explain when we need to use a rails engine? Also if you know, list a few gems which are engines as well.

83. Is it possible to use two identical keys in a hash? What happens if you use two identical keys in a hash?

84. What is the best way to define a foreign key into an existing table in rails?

85. How many rails versions have you worked with? Also list the changes between the rails versions you have worked on.

86. What is the difference between Array and Enumerator?

87. What is your preference for return response for an API? Jbuilder or ActiveModel serializers? And why?

88. What are the differences between lambda and proc?

89. What do you mean by argumented scopes? When do you need to write argumented scopes?

90. What is the difference between update and update_attribute method?

91. What is the difference between :allow_nil and :allow_blank validation options?

92. What do you mean by strict and conditional validations?

93. When do you need to skip callbacks? List a few of the methods, by using them you can skip callbacks.

94. Is it possible to send emails without rendering a template in Rails? If yes, how will you do this?

95. What is the difference between deliver_now and deliver_later methods for sending emails?

96. What do you mean by upsert?

97. What do you mean by session storage in Rails? Explain.

98. What do you mean by session hijacking?

99. What are the main features of the asset pipeline in Rails?

100. What do you mean by page caching, action caching and fragment caching?

101. Why does ruby not support method overloading?

102. What are modules in Ruby? How can you differentiate class and instance methods in a module?

103. What is the difference between after_save and after_commit?

104. What are mixins in Ruby?

105. What do you mean by the send method in Ruby?

106. Have you worked with sidekiq? Why is it used for?

107. What is the difference between the basic version of sidekiq and sidekiq pro?

108. What are perform and perform_async methods in sidekiq? What is the difference between them?

109. What is the difference between let and let! in RSpec?

110. What are the callbacks? Explain for both the model and controller.

111. What is the difference between uniq and distinct in rails?

112. In rails how you will get objects with at least one child?

113. In what cases the change method is not reversible in a Rails migration?

114. What happens if you do not provide the column type in the remove_column migration?

115. What happens if you rollback a change_column migration within the change method?

116. What is the difference between preload and includes?

117. How many ways to eager loading the associations?

118. What do you mean by content_for in Rails?

119. What do you mean by sanitizing params in Rails?

120. What is the difference between render and redirect in Rails?

121. What is the difference between module and concerns in Rails?

122. What is cattr_accessor ?

123. What is difference between cattr_accessor and attr_accessor ?

124. What is difference between sub and gsub method in Ruby ?

125. How to set a custom primary key in rails model other than id?

126. How to provide custom name to a model table in rails ?

127. What is the difference between is_a? and instance_of? methods in Ruby? Which one you will prefer?
```
</details>

----

<details>
  <summary>Answers for the questions</summary>

<!-- ----------------------------------------- BEGIN Q1 - Q20 ----------------------------------------- -->
  <details>
    <summary>Q1 - Q20</summary>

<!-- ------------------ BEGIN Q1 ------------------ -->
<details>
  <summary>Q1. What is the difference between has_many :through and has_and_belongs_to_many? Also state which one is better?</summary>

----
In Rails, both **has_and_belongs_to_many (HABTM)** and **has_many :through** allow you to model many-to-many associations, but they differ in flexibility and maintainability. HABTM uses a simple join table with two foreign keys and no model of its own. It is fast to set up, but limited since you cannot add validations or callbacks on the join, nor can you easily store extra metadata in the relationship.  

On the other hand, **has_many :through** creates an explicit join model, giving you full ActiveRecord features. This model can include validations, scopes, and additional attributes like timestamps, making it much more versatile. For example, if you have `User` and `Project` models connected by a `Membership` model (with a role for each user’s participation), `has_many :through` would be the better fit.  

**Preferred option:** `has_many :through` is generally better because it makes designs more extensible, maintainable, and closer to real-world modeling. HABTM is recommended only for very simple cases where no extra data is needed.
</details>
<!-- ------------------- END Q1 ------------------- -->

----
<!-- ------------------ BEGIN Q2 ------------------ -->
<details>
  <summary>Q2. What are validations in rails? At what moments of an object's lifecycle validations are checked?</summary>

----
Validations in Rails enforce **data integrity** by ensuring only valid data is saved to the database. They are declared in the model layer and provide rules like presence, uniqueness, numericality, and format checks on attributes. For example, `validates :email, presence: true, uniqueness: true` ensures that every record has an email and that it’s unique.  

Rails invokes validations automatically before **persistence operations**:
- `create`, `save`, and `update` methods run validations.  
- When calling `valid?` or `invalid?` manually.  

They **do not** run when you use `delete`, `delete_all`, or `update_column`, since those methods bypass callbacks.  

This ensures that business logic rules are consistently respected across your application without relying too much on database-level constraints. Validations are an essential part of MVC separation, keeping rules inside models rather than spreading them across controllers or views. Well-designed validations make code cleaner, prevent invalid records from polluting production systems, and ease onboarding for developers by centralizing rules in one place.
</details>
<!-- ------------------- END Q2 ------------------- -->

----
<!-- ------------------ BEGIN Q3 ------------------ -->
<details>
  <summary>Q3. What do you mean by polymorphic association in rails? When can one use this association?</summary>

----
A **polymorphic association** is a special type of relationship in Rails where a single model can belong to more than one other model using a single association. For example, a `Comment` model can be associated with both `Post` and `Photo` models through a polymorphic interface (`commentable_type`, `commentable_id`). This eliminates the need for multiple foreign keys or separate tables for each type of relationship.  

**Use case:** Commonly applied in scenarios where multiple entities share a common behavior such as comments, tags, likes, or attachments. Instead of having `post_comments`, `photo_comments`, and `video_comments`, you design just one `commentable` association.  

**Advantages:**  
- Reduces schema duplication.  
- Keeps the system flexible and makes it easier to extend support for new models without creating new join tables.  

**Disadvantages:**  
- Queries become more complex than standard associations.  
- Indexing across polymorphic columns (`type` + `id`) may have performance challenges.  

**When to use it:** If multiple models share the same feature (like `Comment`, `Tag`, `Attachment`), polymorphism is ideal. But if relationships diverge significantly in behavior, it can be better to use explicit associations or even multiple tables. Polymorphic associations are very powerful but should be applied with careful thought to avoid schema fragility.
</details>
<!-- ------------------- END Q3 ------------------- -->

----
<!-- ------------------ BEGIN Q4 ------------------ -->
<details>
  <summary>Q4. What are scopes in Rails?</summary>

----
In Rails, **scopes** are custom query methods defined within models to encapsulate commonly used database queries in a clean, reusable way. They return `ActiveRecord::Relation` objects, meaning they can be chained with other scopes and queries. Scopes essentially act as saved filters that enhance readability while keeping controllers and services more concise.  

For example:  

    scope :published, -> { where(status: 'published') }
    scope :recent, -> { order(created_at: :desc) }

You can then chain them like:  
`Article.published.recent`  

**Benefits:**  
- Keep query logic within models, adhering to Rails’ "skinny controller, fat model" principle.  
- Enhance code readability by replacing raw queries in controllers.  
- Safe to compose with one another due to returning relations.  

**Advanced uses:** Scopes can also accept arguments:  
`scope :created_before, ->(time) { where("created_at < ?", time) }`  

This allows highly expressive querying and saves duplication in larger applications where filtering is common. Unlike class methods that may return random values, scopes are always expected to produce chainable query objects. In production apps, well-structured scopes simplify maintenance since developers can quickly understand common domain queries like `.active`, `.archived`, or `.recent`.
</details>
<!-- ------------------- END Q4 ------------------- -->

----
<!-- ------------------ BEGIN Q5 ------------------ -->
<details>
  <summary>Q5. What is the difference between class methods and scopes? Are they similar?</summary>

----
At first glance, **scopes** and **class methods** in Rails may appear similar because both encapsulate reusable logic. However, they differ in their design goals and return values.  

- **Scopes**: Always return an `ActiveRecord::Relation`, making them chainable with other scopes and query methods. This guarantees predictable chaining and lazy loading. For example, `User.active.recent` will generate one optimized query.  
- **Class methods**: Offer full Ruby flexibility. They can return anything—numbers, arrays, computations, or relations. Because of this freedom, they are not guaranteed to be chainable.  

Generally, scopes are preferred for reusable database filters, while class methods are used when logic extends beyond simple queries—such as performing calculations, calling external services, or aggregating results.  

**Example difference:**  

    scope :active, -> { where(status: 'active') }

This returns a relation you can chain.  

    def self.average_age
      average(:age)
    end

This is a computation, not a chainable scope.  

In summary, use **scopes for query filtering** and **class methods for broader business logic or operations**. Both tools complement each other: start with scopes to structure queries neatly, and when more power is required, switch to class methods.
</details>
<!-- ------------------- END Q5 ------------------- -->

----
<!-- ------------------ BEGIN Q6 ------------------ -->
<details>
  <summary>Q6. What do you mean by ActiveRecord callbacks? Explain some ActiveRecord callbacks.</summary>

----
**ActiveRecord callbacks** are lifecycle hooks provided by Rails that allow you to run code automatically at specific points in the lifecycle of an ActiveRecord object. They help enforce business rules, keep code DRY, and manage side effects during persistence operations like create, update, or delete.  

Some key callbacks include:  
- **before_validation / after_validation** – called before and after model validations run.  
- **before_save / after_save** – triggered before and after saving a record, regardless of whether it’s a create or update.  
- **before_create / after_create** – executed only on creation. Useful for setting defaults or logging.  
- **before_update / after_update** – similar to create, but for updates.  
- **before_destroy / after_destroy** – useful for cleaning related data.  
- **after_commit / after_rollback** – transactional callbacks that run after DB transactions succeed or fail.  

**Best practice:** Don’t overload callbacks with heavy business logic; otherwise, models can become "fat" and hard to debug. Complex workflows should go in service objects, but lightweight tasks (setting a default, cleaning up data, or logging) are fine to keep in callbacks.  
</details>
<!-- ------------------- END Q6 ------------------- -->

----
<!-- ------------------ BEGIN Q7 ------------------ -->
<details>
  <summary>Q7. How can you define custom validations in rails?</summary>

----
Rails provides powerful built-in validations, but for special scenarios you can create **custom validations** in two main ways:  

1. **Inline with `validate` keyword**  
Inside your model, you declare a custom method and point a `validate` call to it:  

    validate :check_age

    def check_age
      errors.add(:age, "must be greater than 18") if age.present? && age < 18
    end

This method adds an error if a condition fails.  

2. **Reusable custom validator class**  
You can create a class under `app/validators` inheriting from `ActiveModel::Validator`:  

    class EmailDomainValidator < ActiveModel::Validator
      def validate(record)
        unless record.email.ends_with?("@mycompany.com")
          record.errors.add(:email, "must be a company email")
        end
      end
    end

Then include it in the model:  

    validates_with EmailDomainValidator  

This approach is recommended for validations you want to reuse across multiple models.  

**Best practice:** Keep validations concise in models for maintainability. Use custom validators when rules are complex or shared.  
</details>
<!-- ------------------- END Q7 ------------------- -->

----
<!-- ------------------ BEGIN Q8 ------------------ -->
<details>
  <summary>Q8. What do you mean by STI(single table inheritance)? What are its advantages and disadvantages?</summary>

----
**Single Table Inheritance (STI)** is a Rails pattern where multiple classes are backed by a single database table. A `type` column stores the name of the subclass to differentiate behavior.  

For example, consider a `users` table with `Admin < User` and `Customer < User`. Both share the same schema (`email`, `name`), but subclasses can define distinct logic or validations.  

**Advantages:**  
- Avoids duplication of schema across multiple tables.  
- Supports code reuse in a shared parent class.  
- Makes querying easy since all records live in a single table.  

**Disadvantages:**  
- Large tables can get "bloated" with irrelevant columns that apply to only some subclasses.  
- Subclass-specific validations and defaults may feel awkward to implement.  
- Schema changes can negatively affect unrelated subclasses.  
- The `type` column is Rails magic and can break if not maintained properly.  

**When to use:** STI works well if subclasses are conceptually related and share >70% of attributes. For diverging subclasses, prefer other approaches such as **Polymorphic Associations** or **separate tables with composition**.
</details>
<!-- ------------------- END Q8 ------------------- -->

----
<!-- ------------------ BEGIN Q9 ------------------ -->
<details>
  <summary>Q9. What do you mean by migrations in Rails? What is the usage of rails migrations?</summary>

----
**Migrations** are version-controlled Ruby classes that allow you to manage your database schema over time in a structured and consistent way. They act as a DSL over raw SQL, meaning you can define schema changes with Ruby commands while Rails translates them into database-specific SQL.  

You generate migrations with `rails generate migration AddAgeToUsers age:integer`. This creates a migration file with `change` or `up/down` methods describing the operation. Running `rails db:migrate` applies these changes, and `rails db:rollback` reverts them.  

**Usage and Benefits:**  
- Track schema evolution under version control (every migration has a timestamp).  
- Simplify schema modifications across team members and CI/CD workflows.  
- Provide DB-agnostic syntax, keeping your code portable.  
- Allow safe rollbacks when a deploy introduces unintended changes.  

Migrations encourage disciplined schema evolution, making them central to Rails’ philosophy of "convention over configuration" and agile database design.  
</details>
<!-- ------------------- END Q9 ------------------- -->

----
<!-- ------------------ BEGIN Q10 ------------------ -->
<details>
  <summary>Q10. What do you mean by N+1 query? How can you resolve N+1 query? Explain by an example.</summary>

----
The **N+1 query problem** happens when a parent query loads multiple records, but each record triggers its own query to fetch associations. This leads to inefficient performance.  

Example:  

    Post.all.each do |post|
      post.comments.each { |c| puts c.body }
    end

Here:  
- `Post.all` = 1 query.  
- For each post (N times), it queries comments.  
So total = N+1 queries.  

**Fix with eager loading:**  

    Post.includes(:comments).each do |post|
      post.comments.each { |c| puts c.body }
    end

Here, Rails fetches posts and all associated comments in **2 queries total**.  

Other solutions include:  
- `preload` (always separate queries but eager loads children).  
- `eager_load` (forces a `JOIN`, used when conditions are applied).  

**Best practice:** Always check queries during development with tools like `bullet` gem to detect N+1 issues. N+1 queries seem harmless at first but can cause exponential slowdowns in production databases.  
</details>
<!-- ------------------- END Q10 ------------------- -->

----
<!-- ------------------ BEGIN Q11 ------------------ -->
<details>
  <summary>Q11. What is the difference between includes and joins?</summary>

----
Both `includes` and `joins` fetch data from multiple tables, but their intent differs.  

- **joins**: Performs an SQL **INNER JOIN** connecting two or more tables. It does not eager load associations and instead yields results based on join conditions. For example:  

    Post.joins(:comments).where(comments: { spam: false })

is efficient for filtering based on child records.  

- **includes**: Performs **eager loading** to prevent N+1 queries. Depending on usage, it can:  
  - Run two queries (one for posts, one for associated comments), OR  
  - Use a `LEFT OUTER JOIN` if conditions are applied on the association.  

**Key difference:**  
- Use `joins` when you need to filter/search data using associated tables.  
- Use `includes` when you’re displaying associated data and want to avoid N+1 queries.  

**Rule of thumb:** `joins` => filtering, `includes` => preloading/display.  
</details>
<!-- ------------------- END Q11 ------------------- -->

----
<!-- ------------------ BEGIN Q12 ------------------ -->
<details>
  <summary>Q12. What do you mean by self_join association in Rails?</summary>

----
A **self-join** is a relationship where a model creates associations with itself. Rails allows this using `class_name` and `foreign_key` options.  

For example:  

    class Employee < ApplicationRecord
      has_many :subordinates, class_name: "Employee", foreign_key: "manager_id"
      belongs_to :manager, class_name: "Employee", optional: true
    end

This setup allows you to call `employee.subordinates` and retrieve other employees who report to them.  

**Use cases:**  
- Hierarchical data like employees and managers.  
- Friends and followers (users following other users).  
- Categories and subcategories in e-commerce apps.  

Self-joins use a single table for relational hierarchy, making them schema-efficient. However, complex queries (recursive relationships) may require CTEs (`WITH RECURSIVE` queries) or gems for tree-structured data.  
</details>
<!-- ------------------- END Q12 ------------------- -->

----
<!-- ------------------ BEGIN Q13 ------------------ -->
<details>
  <summary>Q13. What do you mean by ORM? Explain.</summary>

----
**Object-Relational Mapping (ORM)** is a technique that maps database tables to programming objects. Rails’ **ActiveRecord** is an ORM layer that enables developers to interact with databases using Ruby code instead of writing raw SQL queries.  

Example: Instead of writing:  
`SELECT * FROM users WHERE age > 18;`  
you write:  
`User.where("age > ?", 18)`  

**Advantages:**  
- Productivity: Developers manage objects instead of writing SQL.  
- Abstraction: Works across multiple databases without rewriting queries.  
- Integrates validations, associations, and callbacks seamlessly with models.  
- Supports migrations and schema versioning.  

**Caveats:**  
- ORMs abstract too much, hiding how queries run—causing poor performance if misused.  
- Developers still need to understand SQL to optimize queries, indexes, and joins.  

In Rails, ActiveRecord embodies the ORM approach by implementing CRUD operations, associations, and lifecycle management automatically, which accelerates application development.  
</details>
<!-- ------------------- END Q13 ------------------- -->

----
<!-- ------------------ BEGIN Q14 ------------------ -->
<details>
  <summary>Q14. Is it possible to change the convention of naming a table in rails? If yes, how will you do this? Please explain.</summary>

----
Rails defaults to pluralized table names mapped from singular model names (`Book` → `books`). But sometimes you may deal with a legacy database or special naming conventions.  

You can override the default behavior by specifying a `self.table_name` inside your model:  

    class BookInventory < ApplicationRecord
      self.table_name = "inventory_master"
    end

This ensures Rails queries `inventory_master` instead of `book_inventories`.  

**Usage scenarios:**  
- Migrating an old system with unusual naming conventions.  
- Integrating Rails with a shared database not originally designed for Rails’ conventions.  

**Best practice:** Stick with Rails conventions whenever possible—they reduce confusion and improve maintainability. Only override table names when absolutely necessary.  
</details>
<!-- ------------------- END Q14 ------------------- -->

----
<!-- ------------------ BEGIN Q15 ------------------ -->
<details>
  <summary>Q15. What do you mean by Rolling back a migration? How can you rollback a specific migration?</summary>

----
Rolling back a migration means undoing previously applied schema changes, restoring the database to an earlier state. Migrations use schema versioning, so Rails knows which migrations have run and which still need applying.  

Options for rollback:  
- `rails db:rollback` → rollback the most recent migration.  
- `rails db:rollback STEP=3` → rollback the last 3 migrations.  
- `rails db:migrate:down VERSION=20230815123456` → rollback a specific migration by timestamp version.  

**Why rollback matters:**  
- Helps recover from schema mistakes during development.  
- Essential when a deployment fails and you need quick recovery.  
- Supports agile schema evolution by safely experimenting with changes.  

**Best practice:** Always ensure your migrations are reversible (using `change` instead of `up/down` where possible). When doing destructive changes (like `remove_column`), write explicit `up` and `down` methods.  
</details>
<!-- ------------------- END Q15 ------------------- -->

----
<!-- ------------------ BEGIN Q16 ------------------ -->
<details>
  <summary>Q16. What are the Relational and Conditional callbacks in ActiveRecord? Explain them.</summary>

----
Rails supports **conditional** and **relational** callbacks to give fine-grained control over execution.  

- **Conditional callbacks**: Add logic for when callbacks should or shouldn’t fire. For example:  

    before_save :normalize_name, if: -> { name_changed? }

This means `normalize_name` only runs if `name` is modified.  

- **Relational callbacks**: Involve associations, like `dependent: :destroy`. Example:  

    has_many :comments, dependent: :destroy

When the parent is destroyed, `destroy` is called on each child, triggering **callbacks** on the children too.  

**Pros:**  
- Useful for resource cleanup (e.g., deleting comments when a post is deleted).  
- Avoids wasting execution when conditions don’t apply.  

**Cons:** Over-using callbacks makes models heavy—best practice is to move complex logic out of models and into service layers.  
</details>
<!-- ------------------- END Q16 ------------------- -->

----
<!-- ------------------ BEGIN Q17 ------------------ -->
<details>
  <summary>Q17. What are transactional callbacks? Explain them.</summary>

----
**Transactional callbacks** only execute after a database transaction has either succeeded or failed. This ensures that side effects (like sending emails or updating caches) are tied to the success of the database operation.  

Key examples:  
- `after_commit`: Runs only when the transaction succeeds. Perfect for firing background jobs, sending confirmation emails, or syncing external services.  
- `after_rollback`: Runs when the transaction fails. Useful for logging failure, cleaning up temporary states.  

Example:  

    after_commit :send_welcome_email, on: :create

If the `User` record fails to save, the callback doesn’t run, ensuring no email is sent for an invalid record.  

**Benefits:**  
- Guarantees data consistency: side effects only happen if the DB is in sync.  
- Prevents race conditions in background jobs triggered too early.  

**Best practice:** Always use `after_commit` instead of `after_save` when you’re triggering external side effects—it prevents invalid actions in case the database rolls back.  
</details>
<!-- ------------------- END Q17 ------------------- -->

----
<!-- ------------------ BEGIN Q18 ------------------ -->
<details>
  <summary>Q18. What do you mean by member and collection routes? Explain.</summary>

----
In Rails routing, **member** and **collection** are used to define custom routes on resources.  

- **Member routes**: Operate on a single resource and thus require its `id`. Example:  

    resources :posts do  
      member { get :preview }  
    end  
    # maps GET /posts/:id/preview → posts#preview  

- **Collection routes**: Apply to the entire collection (no `id`). Example:  

    resources :posts do  
      collection { get :archived }  
    end  
    # maps GET /posts/archived → posts#archived  

**Usage consideration:**  
- Use `member` when the action is about one record (previewing a specific post).  
- Use `collection` when the action applies to group-level operations (fetching all archived posts).  

This makes routes more semantic and aligns closely with REST principles.  
</details>
<!-- ------------------- END Q18 ------------------- -->

----
<!-- ------------------ BEGIN Q19 ------------------ -->
<details>
  <summary>Q19. What do you know about namespace and scoped routing? What is the difference between both?</summary>

----
Rails gives us **namespace** and **scope** to organize routes.  

- **namespace**: Wraps controllers under a given module. It changes both the URL and the controller module. Example:  

    namespace :admin do  
      resources :users  
    end  
    # /admin/users → Admin::UsersController  

- **scope**: Adjusts only the URL path or the URL helper prefix but does not change the controller module. Example:  

    scope "/api" do  
      resources :users  
    end  
    # /api/users → UsersController  

**Difference:**  
- Namespace = isolates your controllers under a module (`Admin::UsersController`).  
- Scope = only rewrites the routes path, controller remains the same.  

**Usage:** Use `namespace` when building an admin panel or API with separate controller logic. Use `scope` when you just want clean URLs but do not need a logical separation inside controllers.  
</details>
<!-- ------------------- END Q19 ------------------- -->

----
<!-- ------------------ BEGIN Q20 ------------------ -->
<details>
  <summary>Q20. Explain the difference between webpacker and sprockets.</summary>

----
Rails historically used **Sprockets** as the asset pipeline to compile and serve CSS, JS, and images. It combines assets, minifies them, and serves them efficiently for production in traditional server-rendered Rails apps.  

However, modern Rails apps often include advanced JavaScript ecosystems like React, Vue, or ES6 modules. Sprockets is not suited for compiling those. Enter **Webpacker**—introduced in Rails 5.1. Webpacker integrates Webpack into Rails, allowing apps to bundle modern JS assets and benefit from npm/Yarn ecosystems.  

**Differences:**  
- **Sprockets**: For CSS, JS, and static assets. Simpler but limited for modern JS.  
- **Webpacker**: For JavaScript heavy apps or SPAs; integrates with JS frameworks and tooling ecosystem.  

**Today:** In Rails 7, Webpacker is deprecated. Tools like **Propshaft** and **esbuild / importmaps** were introduced for simpler, faster builds while still supporting modern needs.  

**Summary:** Sprockets = legacy asset pipeline; Webpacker = bridge to modern JS; Rails 7 moved toward lightweight JS bundling for better DX.  
</details>
<!-- ------------------- END Q20 ------------------- -->

  </details>

----  
<!-- ------------------------------------------ END Q1 - Q20 ------------------------------------------ -->





<!-- ----------------------------------------- BEGIN Q21 - Q40 ----------------------------------------- -->
  <details>
    <summary>Q21 - Q40</summary>

<!-- ------------------ BEGIN Q21 ------------------ -->
<details>
  <summary>Q21. How many types of associations are in rails?</summary>

----
Rails provides several types of associations to model relationships between ActiveRecord objects. They are:  

1. **belongs_to** – Sets up a one-to-one connection with another model, meaning this model stores the foreign key. Example: `Comment belongs_to :post`.  
2. **has_one** – Declares a one-to-one connection from the opposite side, meaning the other model has the foreign key.  
3. **has_many** – Declares a one-to-many connection. Example: `Post has_many :comments`.  
4. **has_many :through** – Sets up many-to-many through a join model.  
5. **has_one :through** – Similar to `has_many :through` but for one-to-one.  
6. **has_and_belongs_to_many (HABTM)** – Sets up direct many-to-many associations via a join table, without join model.  
7. **polymorphic associations** – Allows a model to belong to more than one other model using a single foreign key pair (`id + type`).  
8. **self joins** – A model can relate to itself (like employees having managers).  

Rails provides these flexible options to build rich domain models while keeping relationships consistent and expressive.  
</details>
<!-- ------------------- END Q21 ------------------- -->

----
<!-- ------------------ BEGIN Q22 ------------------ -->
<details>
  <summary>Q22. What do you mean by partials in Rails? Explain the usage of partials and the way we can pass local variables to a partial.</summary>

----
In Rails views, **partials** are small reusable view templates that help break down larger views into manageable components. They follow a naming convention with a leading underscore like `_form.html.erb` or `_comment.html.erb`. Partials improve maintainability, reuse code across pages, and avoid duplication.  

**Usage:**  
You render them using:  

    <%= render "form" %>  

Passing locals:  

    <%= render "comment", comment: @comment %>  

Inside `_comment.html.erb`, you can directly reference `comment`.  

To render a collection:  

    <%= render @comments %>  

Rails will automatically look for `_comment.html.erb` and render it for each element in `@comments`.  

**Benefits:**  
- Keeps views DRY.  
- Improves modularity by separating UI components.  
- Supports collections and nested data rendering.  

In modern Rails, partials (often combined with view components or other patterns) ensure large apps remain readable and maintainable with consistent UI structures.  
</details>
<!-- ------------------- END Q22 ------------------- -->

----
<!-- ------------------ BEGIN Q23 ------------------ -->
<details>
  <summary>Q23. What are delegates in Rails? Explain usage of delegates.</summary>

----
Rails’ **delegate** method allows you to call methods on associated objects directly without manually chaining them. It is part of `ActiveSupport`.  

Example:  

    class Order < ApplicationRecord
      belongs_to :customer
      delegate :email, :name, to: :customer, prefix: true
    end

Now instead of `order.customer.email`, you can call `order.customer_email`. This makes the model’s API more expressive.  

**Usage:**  
- Improves readability by exposing frequently-used attributes or behaviors of associated objects.  
- Helps avoid deep navigation across associations.  
- Keeps controllers and views cleaner since they don’t need to drill into associations repeatedly.  

**Best practice:** Use delegates for attributes that are frequently accessed in high-level contexts (like user’s name or email on associated models). Avoid over-delegation which can bloat the model’s API unnecessarily.  
</details>
<!-- ------------------- END Q23 ------------------- -->

----
<!-- ------------------ BEGIN Q24 ------------------ -->
<details>
  <summary>Q24. What do you mean by helper classes? Explain.</summary>

----
In Rails, **helpers** are modules that store methods intended to be used inside views. They provide a clean way to extract logic out of templates, keeping views concise and readable. Rails automatically creates a helper module for every controller (e.g., `UsersHelper` for `UsersController`).  

For example, if you want to format a timestamp:  

    module UsersHelper
      def formatted_date(user)
        user.created_at.strftime("%b %d, %Y")
      end
    end

Then in a view file:  

    <%= formatted_date(@user) %>  

**Why use helpers?**  
- Keep presentation logic out of views for better readability.  
- Encourage code reuse.  
- Improve separation of concerns.  

**Advanced:** Rails also offers `ApplicationHelper` as a global helper for all views. For larger applications, splitting helpers into modules or replacing them with service objects or "view components" can keep things more organized.  
</details>
<!-- ------------------- END Q24 ------------------- -->

----
<!-- ------------------ BEGIN Q25 ------------------ -->
<details>
  <summary>Q25. What do you mean by mailers? How many ways to pass arguments to a mailer?</summary>

----
In Rails, **mailers** are special classes designed to send emails. A mailer class inherits from `ApplicationMailer` and provides methods for generating email messages using models and view templates.  

Example:  

    class UserMailer < ApplicationMailer
      def welcome_email(user)
        @user = user
        mail(to: @user.email, subject: "Welcome!")
      end
    end

You call it with:  

    UserMailer.welcome_email(@user).deliver_now  

**Ways to pass arguments:**  
1. Pass an object as an argument (most common).  
   `UserMailer.welcome_email(user)`  
2. Pass primitive arguments such as IDs or attributes, then find or construct objects inside the mailer.  
   `UserMailer.notify_email(user_id, status)`  

**Best practice:** Keep mailers slim – only handle email composition and delegate heavy logic to models or service objects. This ensures emails are maintainable and properly tested.  
</details>
<!-- ------------------- END Q25 ------------------- -->

----
<!-- ------------------ BEGIN Q26 ------------------ -->
<details>
  <summary>Q26. What do you mean by concerns in Rails? Explain the way of using a concern.</summary>

----
**Concerns** in Rails are a way to share modularized chunks of code between models and controllers without duplicating logic. Essentially, they are Ruby modules placed inside `app/models/concerns` or `app/controllers/concerns`. They help reduce duplication and keep models/controllers lean.  

Example (Model concern):  

    module Trackable
      extend ActiveSupport::Concern
      included do
        before_save :track_timestamp
      end

      def track_timestamp
        self.tracked_at = Time.current
      end
    end

Usage:  

    class User < ApplicationRecord
      include Trackable
    end

Now all `User` objects automatically use this behavior.  

**Why use concerns:**  
- Encourages modular and reusable code.  
- Improves separation of cross-cutting logic (auditing, token generation, validations).  
- Keeps models and controllers thin.  

**Caution:** Don’t overuse concerns – too many can reintroduce spaghetti-code by scattering logic.  
</details>
<!-- ------------------- END Q26 ------------------- -->

----
<!-- ------------------ BEGIN Q27 ------------------ -->
<details>
  <summary>Q27. Have you ever used sidekiq? Explain how it works in both production and development environments?</summary>

----
Yes, **Sidekiq** is a background job processor in Rails that uses Redis as a queue. It enables asynchronous and scheduled job execution, making it ideal for tasks like sending emails, processing payments, or API calls without blocking web requests.  

**How it works:**  
- Sidekiq pushes jobs into Redis queues.  
- Worker processes constantly fetch jobs from Redis and execute them in separate threads.  
- It’s multi-threaded (unlike DelayedJob/Resque), making it highly efficient.  

**Development:** Usually you run `bundle exec sidekiq` alongside your Rails server. Jobs execute quickly, but you can scale down concurrency to avoid resource exhaustion.  

**Production:** Sidekiq runs as a separate process (often supervised using systemd, Docker, or Heroku workers). Using a Redis instance, multiple Sidekiq processes can run in parallel across machines, scaling workloads efficiently.  

Sidekiq provides monitoring via a web UI (`/sidekiq`) to check job queues, retries, and failures. In production, job retries with exponential backoff improve reliability.  

**Summary:** Sidekiq leverages Redis + threads for reliable background processing, runs alongside Rails in dev, but is managed as a service in production for scalability.  
</details>
<!-- ------------------- END Q27 ------------------- -->

----
<!-- ------------------ BEGIN Q28 ------------------ -->
<details>
  <summary>Q28. What is the difference between a sidekiq worker and rails ActiveJob?</summary>

----
- **ActiveJob** is a framework abstraction in Rails for background jobs. It provides a common API for multiple backends like Sidekiq, DelayedJob, Resque, etc.  
- **Sidekiq Worker** is the native API specific to Sidekiq, offering full access to advanced features like retry configurations, scheduling, job prioritization, and concurrency tuning.  

**Differences:**  
- ActiveJob focuses on portability. With ActiveJob, you can switch from Sidekiq to Resque without changing your code. But it only supports a simplified feature set.  
- Sidekiq’s worker classes (`include Sidekiq::Worker`) unlock all Sidekiq-specific features like middleware, queue monitoring, rate-limiting, etc.  

**Best practice:** If your app might switch job processors → use ActiveJob. If you are committed to Sidekiq long-term and want advanced features → use workers directly. Some apps combine both for flexibility.  
</details>
<!-- ------------------- END Q28 ------------------- -->

----
<!-- ------------------ BEGIN Q29 ------------------ -->
<details>
  <summary>Q29. What do you mean by rake tasks? How can you define/implement custom rake tasks?</summary>

----
**Rake tasks** in Rails are Ruby code tasks run in the command line to automate scripts like database maintenance, data imports, or deployments. Rails comes with many built-in rake tasks, such as `db:migrate`.  

To define custom rake tasks, create a file under `lib/tasks/` (e.g., `lib/tasks/my_tasks.rake`):  

    namespace :my_app do
      desc "Print friendly greeting"
      task :greet => :environment do
        puts "Hello from custom rake task!"
      end
    end

Run it with:  

    rake my_app:greet  

**Best practice:** Use rake tasks for *automation scripts* that interact with Rails models/environment. For heavy lifting or complex workflows, wrap them in service classes and invoke those services inside the rake task body for cleaner maintainability.  
</details>
<!-- ------------------- END Q29 ------------------- -->

----
<!-- ------------------ BEGIN Q30 ------------------ -->
<details>
  <summary>Q30. Do you know about ActiveStorage? How can you use this?</summary>

----
**ActiveStorage** is the Rails framework for file uploads introduced in Rails 5.2. It simplifies attaching files to ActiveRecord models and supports cloud storage (Amazon S3, Google Cloud, Azure) as well as local disk.  

Setup: Add ActiveStorage tables via:  

    rails active_storage:install  
    rails db:migrate  

Usage:  

    class User < ApplicationRecord
      has_one_attached :avatar
      has_many_attached :documents
    end

Then in controllers:  
- Upload: `@user.avatar.attach(params[:avatar])`  
- Access: `url_for(@user.avatar)`  

Rails automatically handles storage service abstraction and generates signed URLs for security.  

**Advanced:** ActiveStorage supports image processing, direct uploads with JavaScript, and variant generation (resizing/thumbnails).  

**Benefits:**  
- Built-in Rails feature (no external gems).  
- Direct integration with cloud services.  
- Eliminates complexity of third-party uploaders like Paperclip or CarrierWave.  

It’s the Rails way of modern file handling.  
</details>
<!-- ------------------- END Q30 ------------------- -->

----
<!-- ------------------ BEGIN Q31 ------------------ -->
<details>
  <summary>Q31. Explain strong parameters.</summary>

----
**Strong Parameters** is Rails’ mechanism for preventing **mass-assignment vulnerabilities** by explicitly permitting parameters passed from forms or APIs. Without strong parameters, malicious users could tamper with hidden fields (like `admin=true`) and update sensitive attributes.  

Example in a controller:  

    def user_params
      params.require(:user).permit(:name, :email, :age)
    end  

Now only `:name`, `:email`, and `:age` can be assigned. All others are ignored.  

**Benefits:**  
- Protects your application from untrusted input.  
- Makes parameter handling explicit, clear, and testable.  

**Best practice:** Always whitelist only the attributes that are safe to update from forms or API requests. When exposing APIs, strong parameters are critical for securing your endpoints.  
</details>
<!-- ------------------- END Q31 ------------------- -->

----
<!-- ------------------ BEGIN Q32 ------------------ -->
<details>
  <summary>Q32. How do you pass default arguments to a controller action where you instantiate a new model object?</summary>

----
When you create a new model in a controller and want default attributes, you can initialize the object by merging defaults into `params`.  

Example:  

    def new
      @user = User.new(defaults.merge(params.fetch(:user, {})))
    end

    private

    def defaults
      { role: "guest", active: true }
    end

Alternatively, you can define defaults in the model using `after_initialize` callback:  

    class User < ApplicationRecord
      after_initialize :set_defaults

      def set_defaults
        self.role ||= "guest"
        self.active = true if active.nil?
      end
    end

**Best practice:** Use model-level defaults (`after_initialize` or DB defaults) when the same behavior is needed consistently. Use controller defaults for UI-level form initialization.  
</details>
<!-- ------------------- END Q32 ------------------- -->

----
<!-- ------------------ BEGIN Q33 ------------------ -->
<details>
  <summary>Q33. What are turbolinks into rails?</summary>

----
**Turbolinks** is a Rails library that improves page load performance by intercepting standard link clicks and replacing only the `<body>` and `<title>` of the page via AJAX. This avoids full reloads, making Rails apps feel much faster without turning them into SPAs.  

**How it works:**  
- You keep normal server-rendered views.  
- When you click a link, Turbolinks loads the new page with AJAX.  
- It replaces the current page body instead of reloading the browser context.  

**Benefits:**  
- Faster navigation in Rails applications.  
- Retains state (like JS event listeners) between page loads.  
- Requires very little modification to application code.  

**Limitations:**  
- Some complex JavaScript workflows may break since full reloads don’t happen.  
- State handling can be tricky if you rely on `ready()` events.  

From Rails 7 onwards, Turbolinks has been replaced by **Turbo (part of Hotwire)**, which provides even richer real-time experiences.  
</details>
<!-- ------------------- END Q33 ------------------- -->

----
<!-- ------------------ BEGIN Q34 ------------------ -->
<details>
  <summary>Q34. What do you mean by API versioning in Rails? Explain when there is a need to change the version of an API?</summary>

----
**API versioning** means providing multiple versions of your API endpoints so that changes don’t break existing clients. In Rails, this is usually done by namespacing controllers:  

    namespace :api do  
      namespace :v1 do  
        resources :users  
      end  
      namespace :v2 do  
        resources :users  
      end  
    end  

This maps requests to `Api::V1::UsersController` or `Api::V2::UsersController`.  

**When to version APIs:**  
- When you make **backward-incompatible changes** (removing fields, renaming fields, changing endpoints).  
- When introducing major feature upgrades that may break older clients.  
- When supporting multiple client apps (mobile, web, third party) that can’t all upgrade at once.  

**Best practices for versioning:**  
- Use semantic versioning (`v1`, `v2`).  
- Always document deprecated APIs with expiry timelines.  
- Keep multiple versions active for some time to allow smooth transitions.  

API versioning ensures that innovation doesn’t break compatibility, which is crucial in production systems serving external clients.  
</details>
<!-- ------------------- END Q34 ------------------- -->

----
<!-- ------------------ BEGIN Q35 ------------------ -->
<details>
  <summary>Q35. What is the difference between before_save, before_create and before_update?</summary>

----
These are all Rails callbacks, but they run at different points in a record’s lifecycle:  

- **before_save**: Runs before every save, whether a record is new or persisted (includes both create and update).  
- **before_create**: Runs only when a new record is created, not on updates.  
- **before_update**: Runs only when updating an existing record.  

**Usage:**  
- Use `before_save` for logic that applies to both create and update (ex: normalizing a name).  
- Use `before_create` for defaults that should only apply on new objects (e.g., generate unique token at creation).  
- Use `before_update` to enforce rules for updates only (e.g., prevent status change from `closed` back to `open`).  

Understanding these distinctions prevents bugs where callbacks might fire more often than expected.  
</details>
<!-- ------------------- END Q35 ------------------- -->

----
<!-- ------------------ BEGIN Q36 ------------------ -->
<details>
  <summary>Q36. What do you mean by asset pipeline?</summary>

----
The **Asset Pipeline** in Rails is a framework to manage, compress, and package static assets like JavaScript, CSS, and images. It was introduced in Rails 3.1 using **Sprockets**.  

**Key Features:**  
- **Concatenation:** Combines multiple files into one for fewer HTTP requests.  
- **Minification:** Compresses files for performance.  
- **Preprocessing:** Supports CoffeeScript, Sass, and ERB inside assets.  
- **Digest fingerprints:** Automatically appends unique hash to asset filenames to ensure proper browser caching.  

Assets are stored in `app/assets`, `lib/assets`, or `vendor/assets`.  

**Workflow:**  
- In development: assets served dynamically for fast iteration.  
- In production: assets precompiled into the `/public/assets` folder.  

Although Webpacker replaced some functionality for JS in Rails 5+, the Asset Pipeline is still critical for CSS, images, and classic JS. Rails 7 introduces Propshaft as a modern replacement.  
</details>
<!-- ------------------- END Q36 ------------------- -->

----
<!-- ------------------ BEGIN Q37 ------------------ -->
<details>
  <summary>Q37. What do you mean by default_scope? Please explain.</summary>

----
In Rails, **default_scope** lets you define a default query that applies globally to a model. For instance:  

    class Post < ApplicationRecord
      default_scope { where(published: true) }
    end

Now, `Post.all` will automatically only fetch published records.  

**Pros:**  
- Makes common constraints implicit.  
- Reduces query duplication.  

**Cons:**  
- Can lead to surprising results—for example, when working with associations or wanting *all* records, including unpublished ones.  
- Harder to debug because the scope is always silently applied.  

**Best practice:** Default scopes should be avoided for non-trivial conditions. Instead, use named scopes like `Post.published` for clarity. If using `default_scope`, always provide a way to `unscope` it:  

    Post.unscoped.all  

This prevents unexpected bugs in larger applications.  
</details>
<!-- ------------------- END Q37 ------------------- -->

----
<!-- ------------------ BEGIN Q38 ------------------ -->
<details>
  <summary>Q38. Explain routing in rails.</summary>

----
**Routing** in Rails connects incoming HTTP requests to the appropriate controller actions. Defined in `config/routes.rb`, it maps URLs + HTTP verbs to methods.  

Example:  

    resources :posts  

This creates RESTful routes like:  
- GET `/posts` → `posts#index`  
- POST `/posts` → `posts#create`  
- GET `/posts/:id` → `posts#show`  

You can also define custom member and collection routes, namespaces, scopes, and concerns.  

**Routing helpers:** Rails creates path helpers (`posts_path`, `new_post_path`) for consistency.  

**Advanced routing features:**  
- Constraints (e.g., only match numeric IDs).  
- Nested resources (`posts/:post_id/comments`).  
- Namespacing for admin panels or APIs (`/api/v1/users`).  

**Philosophy:** Rails routing aligns with REST principles to standardize design patterns. Well-structured routes make the application more predictable and easier to maintain.  
</details>
<!-- ------------------- END Q38 ------------------- -->

----
<!-- ------------------ BEGIN Q39 ------------------ -->
<details>
  <summary>Q39. What do you mean by filter actions or controller callbacks? Explain.</summary>

----
In Rails controllers, **filters (callbacks)** are methods that run before, after, or around controller actions to share common logic.  

Examples:  
- `before_action :authenticate_user` – runs before every action.  
- `after_action :log_activity` – runs after actions complete.  
- `around_action :benchmark` – wraps the execution of the method.  

**Uses:**  
- Authentication (`before_action`).  
- Logging or auditing (`after_action`).  
- Setting shared variables for multiple actions.  

These filters reduce duplication of setup/teardown code across actions.  

**Best practice:** Keep filters lightweight. Avoid business logic or complex queries inside filters—delegate to services or models. Filters are best for cross-cutting concerns (auth, logging, localization, etc).  
</details>
<!-- ------------------- END Q39 ------------------- -->

----
<!-- ------------------ BEGIN Q40 ------------------ -->
<details>
  <summary>Q40. How can you handle ActiveRecord::RecordNotFound exception for all resources?</summary>

----
When a resource lookup fails in Rails (e.g., `User.find(params[:id])` and no record exists), an `ActiveRecord::RecordNotFound` exception is raised. By default this shows a 404 error in development, but you may want a standardized handling.  

You can handle globally in `ApplicationController`:  

    class ApplicationController < ActionController::Base
      rescue_from ActiveRecord::RecordNotFound, with: :not_found

      private
      def not_found
        render file: "#{Rails.root}/public/404.html", status: :not_found
      end
    end

For APIs, you can render JSON instead:  

    render json: { error: "Resource not found" }, status: :not_found  

**Benefit:** This centralizes exception handling so you don’t need to wrap every `find` call in `rescue` blocks. It leads to cleaner code, better user experience, and consistent API responses.  
</details>
<!-- ------------------- END Q40 ------------------- -->

  </details>

---- 
<!-- ------------------------------------------ END Q21 - Q40 ------------------------------------------ -->






<!-- ----------------------------------------- BEGIN Q41 - Q60 ----------------------------------------- -->
  <details>
    <summary>Q41 - Q60</summary>

<!-- ------------------ BEGIN Q41 ------------------ -->
<details>
  <summary>Q41. How many gems for the admin backend have you used? Which gem is better and why?</summary>

----
Popular gems for building admin backends in Rails include:  
- **ActiveAdmin** – Feature-rich and highly customizable. Provides DSL to quickly build admin dashboards, filters, and CRUD interfaces.  
- **RailsAdmin** – Simpler, works out-of-the-box, offers CRUD with nice UI, but less customizable than ActiveAdmin.  
- **Administrate** (by Thoughtbot) – Clean, modern, minimalistic approach. Opinionated, less features than ActiveAdmin but highly maintainable.  

**Which is better?** It depends on project needs:  
- If you need quick setup and lots of built-in features and filters → **ActiveAdmin** is better.  
- If your project demands simplicity with high maintainability and flexibility for custom UI → **Administrate** is preferred.  

As a mid-senior dev, I’d recommend **ActiveAdmin** for enterprise/admin-heavy apps and **Administrate** when UI consistency is more important than advanced features.  
</details>
<!-- ------------------- END Q41 ------------------- -->

----
<!-- ------------------ BEGIN Q42 ------------------ -->
<details>
  <summary>Q42. You are asked to implement an admin backend for a web application. What solution will you propose? Any gem or custom admin panel? Also explain the reason.</summary>

----
The solution depends on project requirements.  

1. **Using a gem (ActiveAdmin or Administrate):**  
   - Fast development -> low time-to-market.  
   - Covers common needs: CRUD, filters, exports, authentication hooks.  
   - Good for projects where the admin is not central functionality but still needed.  

2. **Custom admin panel:**  
   - Provides maximum flexibility and fine control over UI/UX.  
   - Good for projects where admin workflows are complex or domain-specific (e.g., financial dashboards, specialized process flows).  

**My recommendation:**  
- If admin is more of a utility, go with **ActiveAdmin** or **Administrate**.  
- If the admin backend is a **key differentiator or customer-facing product module**, invest in a custom-built panel.  

This balances development cost, scalability, and maintainability.  
</details>
<!-- ------------------- END Q42 ------------------- -->

----
<!-- ------------------ BEGIN Q43 ------------------ -->
<details>
  <summary>Q43. What is the difference between save and save!?</summary>

----
- **save**: Persists a record and returns `true` if validations pass; returns `false` if validations fail. It does not raise exceptions.  
- **save!**: Same behavior, but raises an `ActiveRecord::RecordInvalid` exception if validations fail.  

**Example:**  

    user = User.new(name: nil)  
    user.save   # returns false (no exception)  
    user.save!  # raises ActiveRecord::RecordInvalid  

**When to use:**  
- Use `save` in scenarios where failure is expected/handled with conditionals.  
- Use `save!` when validation failure is exceptional and should be highlighted (e.g., within background jobs or service objects).  

As a mid-senior engineer, I prefer `save!` in business logic so failures don’t fail silently.  
</details>
<!-- ------------------- END Q43 ------------------- -->

----
<!-- ------------------ BEGIN Q44 ------------------ -->
<details>
  <summary>Q44. How can you pass params to a mailer action?</summary>

----
You can pass parameters directly to mailer methods just like controller methods.  

For instance:  

    class UserMailer < ApplicationMailer
      def notification_email(user, message)
        @user = user
        @message = message
        mail(to: @user.email, subject: "New Message")
      end
    end

Call it with:  

    UserMailer.notification_email(@user, "Welcome!").deliver_now  

Alternatively, you may pass only simple arguments like IDs and then load the object inside the mailer for better reliability:  

    def notify(user_id)
      @user = User.find(user_id)
      mail(to: @user.email, subject: "Hello")
    end  

This ensures the mailer works consistently even if background jobs serialize the mail call.  
</details>
<!-- ------------------- END Q44 ------------------- -->

----
<!-- ------------------ BEGIN Q45 ------------------ -->
<details>
  <summary>Q45. Is it possible to replace the schema.rb file in Rails? If yes, how can you do this?</summary>

----
Yes. By default, Rails maintains `schema.rb` as the auto-generated representation of the current database schema. However, you can replace it with `structure.sql` when using more advanced database features not supported by the schema dumper (like triggers, stored procedures, partial indexes).  

**Enable in `config/application.rb`:**  

    config.active_record.schema_format = :sql  

This generates `db/structure.sql` instead of `db/schema.rb` when you run `db:migrate`.  

**When to use:**  
- If you use basic Rails migrations → stick to `schema.rb`.  
- If you rely heavily on advanced DB features (check constraints, partial indexes, custom SQL) → use `structure.sql` for accuracy.  
</details>
<!-- ------------------- END Q45 ------------------- -->

----
<!-- ------------------ BEGIN Q46 ------------------ -->
<details>
  <summary>Q46. What is ActionCable? Explain.</summary>

----
**ActionCable** is Rails’ solution to integrate WebSockets (real-time communication) into a Rails app. It allows server and client to maintain a persistent connection, enabling instant data updates without page reloads.  

**How it works:**  
- ActionCable has `channels` (like controllers for WebSocket streams).  
- Clients subscribe to channels, and servers can broadcast messages.  
- Each user can have multiple subscriptions (e.g., chatroom, notifications).  

Example: A Chat app using ActionCable can broadcast new messages to all subscribed clients instantly.  

**Benefits:**  
- Native WebSocket support fully integrated into Rails.  
- Follows the conventions of MVC with Channels.  
- Works with Redis for scaling across multiple servers.  

**Use cases:** Chat applications, live dashboards, notifications, collaborative editing, real-time games.  

In modern Rails apps, ActionCable + Hotwire/Turbo Streams provide real-time interactivity without heavy JavaScript frameworks.  
</details>
<!-- ------------------- END Q46 ------------------- -->

----
<!-- ------------------ BEGIN Q47 ------------------ -->
<details>
  <summary>Q47. How can you implement user authentication using devise and JWT? Explain the process of it.</summary>

----
To implement authentication with **Devise + JWT**, you combine Devise’s authentication management with JWT tokens for stateless API access.  

**Steps:**  
1. Add `devise` and `devise-jwt` gems.  
2. Configure your User model:  

    class User < ApplicationRecord
      devise :database_authenticatable, :registerable,
             :jwt_authenticatable,
             jwt_revocation_strategy: JwtDenylist
    end  

3. Create a `JwtDenylist` model/table to store revoked tokens.  
4. Configure Devise initializer to use JWT strategy.  
5. When a user logs in/signs up, Devise issues a JWT to the client.  
6. Client includes this token in headers (`Authorization: Bearer <token>`) for future requests.  
7. Devise reads the token, validates it, and authenticates the user without a session.  

**Advantages:**  
- Works well for APIs (mobile apps, SPAs).  
- No need for session cookies.  
- Stateless architecture scales better.  

This setup provides the convenience and security of Devise combined with scalability of JWT-based API authentication.  
</details>
<!-- ------------------- END Q47 ------------------- -->

----
<!-- ------------------ BEGIN Q48 ------------------ -->
<details>
  <summary>Q48. How many form helpers are provided by rails? Tell the names and differences between them.</summary>

----
Rails provides a number of helpers for creating forms:  

1. **form_for** – Used for model-based forms. Deprecated in favor of `form_with`.  
2. **form_tag** – Used to create forms not bound to a model (deprecated).  
3. **form_with** – Introduced in Rails 5.1, unifies both `form_for` and `form_tag`. Automatically infers whether form is model-based or not.  

Supporting helpers: `text_field`, `email_field`, `number_field`, `password_field`, `select`, `check_box`, etc.  

**Differences:**  
- `form_for` → focuses on models.  
- `form_tag` → standalone.  
- `form_with` → modern replacement, more concise, supports Ajax (when `local: false`).  

**Best practice:** Use `form_with` for consistency and future readiness.  
</details>
<!-- ------------------- END Q48 ------------------- -->

----
<!-- ------------------ BEGIN Q49 ------------------ -->
<details>
  <summary>Q49. What is the difference between delete and destroy in Rails?</summary>

----
Both remove a record but behave differently:  

- **delete** – Removes the record directly from the database using SQL `DELETE`. It skips callbacks and validations. It simply issues `DELETE FROM table WHERE id=...`.  
- **destroy** – Runs model callbacks (`before_destroy`, `after_destroy`) and executes dependent logic (`dependent: :destroy` on associations).  

**Example:**  

    user.delete   # record removed immediately
    user.destroy  # callbacks + associations handled

**Which to use:**  
- Use `destroy` in most cases to preserve data integrity.  
- Use `delete` if you need raw speed and are absolutely sure you don’t need callbacks/child deletions.  

As a mid-senior engineer, I’d stress `destroy` is safer, but `delete` is faster for bulk operations under controlled conditions.  
</details>
<!-- ------------------- END Q49 ------------------- -->

----
<!-- ------------------ BEGIN Q50 ------------------ -->
<details>
  <summary>Q50. How do you organize your controllers? Tell me about the way that you can make a controller thin.</summary>

----
Organizing controllers is about keeping them lean and ensuring separation of concerns. A well-structured Rails controller should only coordinate the flow between models, business logic, and views, not contain heavy computation.  

**Best practices to keep controllers thin:**  
- **Move logic to models, scopes, and service objects.** Example: Use model validations and scopes for data filtering.  
- **Use concerns** for shared behavior across controllers.  
- **Use before_action filters** only for common setup (like authentication).  
- **Use serializers (ActiveModel Serializer / JBuilder)** for complex JSON responses.  
- **Service and Form objects:** Heavy workflows (like payment processing) should be encapsulated into classes outside controllers.  

By following these patterns, controllers remain small and focused (~5–10 lines per action ideally). Thin controllers improve maintainability, testability, and readability, especially in larger applications.  
</details>
<!-- ------------------- END Q50 ------------------- -->

----
<!-- ------------------ BEGIN Q51 ------------------ -->
<details>
  <summary>Q51. What do you mean by sessions in Rails? In what circumstances do you need to use sessions? Explain.</summary>

----
Rails **sessions** allow you to store stateful information between HTTP requests (which are normally stateless). Sessions are usually stored as signed cookies, but can also use server stores (Redis, Memcached, ActiveRecord).  

**Common use cases:**  
- Authentication → storing current user ID after login.  
- Shopping carts → keeping cart items while navigating around.  
- Flash messages → passing one-time messages between requests.  

Example in a controller:  

    session[:user_id] = @user.id  
    session.delete(:user_id)  

**Why use sessions:** PostgreSQL or REST APIs are stateless, but sessions are essential for persistent web experiences. They are stored securely (signed, optionally encrypted cookies).  

**When to avoid:** API-only applications typically don’t use Rails sessions. Instead, they rely on JWT tokens or OAuth.  
</details>
<!-- ------------------- END Q51 ------------------- -->

----
<!-- ------------------ BEGIN Q52 ------------------ -->
<details>
  <summary>Q52. What is the find_each method in Rails? Also explain why the .all method is not ideal to use for loading all the instances of a model at once?</summary>

----
- **find_each**: Batches query results and iterates over them in chunks (default 1000). Example:  

    User.find_each(batch_size: 500) do |user|
      puts user.name
    end  

This avoids loading the entire dataset into memory.  

- **all method** → `User.all.each` loads every user into memory at once. This is inefficient and risky for large tables, potentially crashing the app with out-of-memory errors.  

**Best practice:**  
- Use `.find_each` or `.in_batches` for large datasets.  
- Use `.all` only for small datasets where memory load isn’t an issue.  

Rails implements `.find_each` with batching SQL queries (`LIMIT/OFFSET` or primary key ranges), keeping performance scalable.  
</details>
<!-- ------------------- END Q52 ------------------- -->

----
<!-- ------------------ BEGIN Q53 ------------------ -->
<details>
  <summary>Q53. What is polymorphic association in Rails? When should you actually use a polymorphic association?</summary>

----
A **polymorphic association** allows a model to belong to multiple models via a single association. It uses `*_type` and `*_id` fields to identify which model owns the association.  

Example:  

    class Comment < ApplicationRecord
      belongs_to :commentable, polymorphic: true
    end

Here, `commentable` could be a `Post`, `Photo`, or `Video`.  

**When to use:**  
- When multiple models share a common behavior like comments, tags, likes, or addresses.  
- Helps you design DRY schemas without creating multiple separate join tables.  

**Pros:**  
- Simpler schema, avoids repetitive tables.  
- Scalable design for shared behaviors.  

**Cons:**  
- Queries involve multiple tables indirectly (`commentable_type + id`), can reduce performance.  
- Harder to constrain with strict foreign keys across DB engines.  

Use polymorphism when models truly share the same relation, otherwise explicit `has_many :through` might be better.  
</details>
<!-- ------------------- END Q53 ------------------- -->

----
<!-- ------------------ BEGIN Q54 ------------------ -->
<details>
  <summary>Q54. What is the difference between eager_load and includes methods? And which one is better?</summary>

----
Both `includes` and `eager_load` are used to load associations, but they generate SQL differently.  

- **includes**: Will load associations in 2 queries (one for parent, one for child) unless conditions are applied on the association. If conditions exist, Rails sometimes converts it to a `LEFT OUTER JOIN`.  
- **eager_load**: Forces a `LEFT OUTER JOIN` every time. Essentially `eager_load` = `includes(...).references(...)`.  

**Which is better?**  
- For simple eager loading to avoid N+1 → `includes` (fewer joins, less data).  
- For filtering/sorting on child associations → `eager_load`, since it ensures joined data is available.  

**Summary:** Choose based on query semantics. `includes` is usually preferable, but `eager_load` is needed when writing conditions on associated tables.  
</details>
<!-- ------------------- END Q54 ------------------- -->

----
<!-- ------------------ BEGIN Q55 ------------------ -->
<details>
  <summary>Q55. Which of the methods is faster between delete and destroy? Explain why?</summary>

----
- **delete** is faster because it issues a raw SQL `DELETE` statement directly without instantiating objects or running callbacks.  
- **destroy**, however, instantiates each object, runs `before_destroy`/`after_destroy` callbacks, validates associations, and handles `dependent: :destroy`.  

This makes `destroy` safer but slower.  

**When to use:**  
- For bulk deletions or non-critical data cleanup → use `delete_all` for maximum performance.  
- For sensitive deletions where callbacks are important (clearing caches, sending notifications, cleaning associated records) → use `destroy`.  

**Conclusion:** `delete` is always faster, but `destroy` ensures integrity. Use based on whether business logic depends on callbacks.  
</details>
<!-- ------------------- END Q55 ------------------- -->

----
<!-- ------------------ BEGIN Q56 ------------------ -->
<details>
  <summary>Q56. What is the difference between ActiveModel and ActiveRecord?</summary>

----
- **ActiveRecord**: The ORM for Rails. It directly maps database tables to Ruby classes and provides methods for persistence, associations, and queries. Example: `User < ApplicationRecord`.  
- **ActiveModel**: Provides model-like features (validations, callbacks, naming) **without persistence**. Used for objects that behave like models but don’t map to a DB table.  

**Example:**  
- `User` (ActiveRecord) persists to DB.  
- `ContactForm` can include ActiveModel to get validations, but isn’t backed by DB.  

**Usage:**  
- ActiveRecord for actual database models.  
- ActiveModel for POROs (Plain Old Ruby Objects) like form objects, API response objects, service data.  

This separation allows Rails to extend "model-like" behavior beyond ActiveRecord.  
</details>
<!-- ------------------- END Q56 ------------------- -->

----
<!-- ------------------ BEGIN Q57 ------------------ -->
<details>
  <summary>Q57. What is the difference between dependent: :destroy and dependent: :delete_all?</summary>

----
- **dependent: :destroy**: When a parent is destroyed, associated children are instantiated, and each child’s `.destroy` method is invoked. This means callbacks and validations are executed on the child objects. Safer but slower.  
- **dependent: :delete_all**: Direct SQL `DELETE` is issued for all child records without instantiating them. Much faster but skips callbacks, validations, and doesn’t trigger dependent associations on children.  

**When to use:**  
- Use `:destroy` when child records have important callbacks or cascading dependencies.  
- Use `:delete_all` for better performance when children don’t require extra handling (e.g., log records, cached data).  

This is essentially the same tradeoff as `destroy vs delete`.  
</details>
<!-- ------------------- END Q57 ------------------- -->

----
<!-- ------------------ BEGIN Q58 ------------------ -->
<details>
  <summary>Q58. What is yield in Ruby? What happens if you call the method, which includes yield, without passing a block?</summary>

----
In Ruby, `yield` passes control from a method to a supplied block. It allows flexible customization of method behavior.  

Example:  

    def greet
      puts "Hello"
      yield if block_given?
      puts "Goodbye"
    end

    greet { puts "from block" }

Output:  
`Hello`  
`from block`  
`Goodbye`  

If `yield` is invoked **without** a block passed → `LocalJumpError`. To avoid this, check `block_given?` before yielding.  

**Use cases:** Iterators, callbacks, and dynamic behavior customization. Blocks with yield are fundamental to the Ruby idiom for DSLs and iterators (`each` etc.).  
</details>
<!-- ------------------- END Q58 ------------------- -->

----
<!-- ------------------ BEGIN Q59 ------------------ -->
<details>
  <summary>Q59. What is the difference between Hash and HashWithIndifferentAccess?</summary>

----
- **Hash**: Ruby’s default Hash, differentiates between symbol and string keys. `hash[:key]` is different from `hash["key"]`.  
- **HashWithIndifferentAccess**: Provided by Rails, treats symbol and string keys interchangeably.  

Example:  

    h = { "name" => "John" }
    h[:name]   # => nil  

    h = { name: "John" }.with_indifferent_access
    h[:name]   # => "John"
    h["name"]  # => "John"  

**Use case:** Rails parameters (`params`) are instances of `HashWithIndifferentAccess`, so you don’t need to worry about string/symbol mismatches.  

**Tradeoff:** `HashWithIndifferentAccess` has slight overhead compared to plain `Hash`. Use it when input flexibility matters, otherwise prefer plain Hash.  
</details>
<!-- ------------------- END Q59 ------------------- -->

----
<!-- ------------------ BEGIN Q60 ------------------ -->
<details>
  <summary>Q60. In Ruby, how many ways to invoke a method? Illustrate with examples.</summary>

----
Ruby provides multiple ways to invoke a method:  

1. **Standard dot notation**:  
   `user.name`  
2. **send method**:  
   `user.send(:name)` (useful for metaprogramming, calling private methods).  
3. **public_send**: Similar to `send` but respects access control.  
4. **method + call**:  
   `m = user.method(:name)`  
   `m.call`  
5. **Object#[] operator** (for some DSL-friendly APIs):  
   Example in Hash: `hash[:key]` invokes the `[]` method.  

Each method provides varying flexibility:  
- `send` and `public_send` are powerful tools for dynamic method invocation.  
- Standard dot notation is the most common and readable.  

Proper use of these techniques enables elegant metaprogramming in Ruby.  
</details>
<!-- ------------------- END Q60 ------------------- -->

  </details>

---- 
<!-- ------------------------------------------ END Q41 - Q60 ------------------------------------------ -->






<!-- ----------------------------------------- BEGIN Q61 - Q80 ----------------------------------------- -->
  <details>
    <summary>Q61 - Q80</summary>

<!-- ------------------ BEGIN Q61 ------------------ -->
<details>
  <summary>Q61. In Ruby, what is the difference between Strings and Symbols? Explain.</summary>

----
In Ruby, **Strings** and **Symbols** are both used to represent text, but they behave quite differently:  

- **Strings**: Mutable objects. Every time you create `"hello"` it creates a new object unless frozen. String operations like concatenation and interpolation are common in everyday Ruby code.  
- **Symbols**: Immutable and lightweight identifiers represented with a `:` prefix (`:hello`). They are unique and always reference the same object in memory. This makes them faster for repeated lookup keys.  

**Example:**  

    "name".object_id == "name".object_id   # false  
    :name.object_id == :name.object_id     # true  

**When to use:**  
- Strings for text manipulation, user input, changing data.  
- Symbols for identifiers, keys in hashes, method names, internal references.  

Symbols save memory and are faster when consistency matters, but lack the full set of String methods. Strings are better when dynamic behavior is required. In Rails, parameters are typically converted to symbols when referencing model attributes.  
</details>
<!-- ------------------- END Q61 ------------------- -->

----
<!-- ------------------ BEGIN Q62 ------------------ -->
<details>
  <summary>Q62. What do you mean by schema versioning in Rails? When does it change?</summary>

----
In Rails, **schema versioning** is the practice of managing the state of the database schema over time through migrations. Each migration file contains a timestamp in its filename, which serves as its "version."  

For example: `20250827120000_add_users_table.rb`.  

When you run `rails db:migrate`, Rails applies pending migrations and updates your schema file (`schema.rb` or `structure.sql`). The schema version recorded in the `schema_migrations` table changes with each applied migration.  

**In summary:**  
- Each new migration increases schema version.  
- Version changes whenever migrations are run.  
- This allows teams to sync databases consistently between environments (dev, staging, production).  

Schema versioning ensures your DB schema is reproducible, trackable under source control, and consistent across deployments.  
</details>
<!-- ------------------- END Q62 ------------------- -->

----
<!-- ------------------ BEGIN Q63 ------------------ -->
<details>
  <summary>Q63. What do you mean by reversible migrations?</summary>

----
A **reversible migration** is one that Rails knows how to undo automatically when you rollback, because `change` method can be reversed.  

Example:  

    def change
      add_column :users, :age, :integer
    end

Rails knows how to remove that column if you rollback.  

**Non-reversible cases:**  
- Using raw SQL (`execute`)  
- Custom complex logic (data migrations)  
- `remove_column` without specifying type  

**Solution:** If your migration isn't reversible, you'll need `up` and `down` methods explicitly:  

    def up
      execute "SOME SQL"
    end
    
    def down
      execute "REVERSE SQL"
    end  

Reversible migrations make schema evolution much safer and more automated.  
</details>
<!-- ------------------- END Q63 ------------------- -->

----
<!-- ------------------ BEGIN Q64 ------------------ -->
<details>
  <summary>Q64. How can you run/rollback any specific migration in Rails?</summary>

----
To run a specific migration by version:  

    rails db:migrate:up VERSION=20250827120000  

To rollback (undo) a specific migration:  

    rails db:migrate:down VERSION=20250827120000  

Instead of VERSION, Rails will look for timestamp in the migration filename.  

**Tip:**  
- Use `db:rollback STEP=n` for rolling back a batch of migrations.  
- Use specific `up` and `down` for controlled migrations when debugging/downgrading production safely.  

This selective approach is useful to test migrations individually or handle production issues more carefully.  
</details>
<!-- ------------------- END Q64 ------------------- -->

----
<!-- ------------------ BEGIN Q65 ------------------ -->
<details>
  <summary>Q65. When should you use an up and down method instead of a change method inside your migration? Explain by an example.</summary>

----
Rails provides `change` for reversible migrations, but sometimes migrations cannot be automatically reversed. In such cases, you use `up` and `down`.  

Example (non-reversible with `change`):  

    def change
      remove_column :users, :age
    end

This fails on rollback because Rails doesn’t know the datatype to re-add. Instead:  

    def up
      remove_column :users, :age
    end

    def down
      add_column :users, :age, :integer
    end  

**When to use `up`/`down`:**  
- Removing columns, indexes, or tables.  
- Complex raw SQL changes.  
- Data migrations that need explicit reversal steps.  

Thus, `up`/`down` provide safety when migrations can’t be cleanly reversed automatically.  
</details>
<!-- ------------------- END Q65 ------------------- -->

----
<!-- ------------------ BEGIN Q66 ------------------ -->
<details>
  <summary>Q66. What is shallow nesting of routes and when is preferable to use this?</summary>

----
Shallow nesting in Rails routing avoids overly nested resource URLs by limiting nested routes only where needed.  

Example (deep nesting):  

    resources :posts do
      resources :comments do
        resources :likes
      end
    end

This creates long, unwieldy paths like `/posts/1/comments/2/likes/3`.  

**Shallow nesting:**  

    resources :posts do
      resources :comments, shallow: true
    end

Generates nested routes only for creation (`/posts/:post_id/comments`) but exposes shallow paths like `/comments/:id` for show/update/destroy.  

**Benefits:**  
- Cleaner, shorter URLs.  
- Easier maintenance and avoids "max nesting" rule (Rails recommends no more than 1 level of nesting).  

**When to use:** Always prefer shallow nesting when child resources are meaningful independently (like comments, likes).  
</details>
<!-- ------------------- END Q66 ------------------- -->

----
<!-- ------------------ BEGIN Q67 ------------------ -->
<details>
  <summary>Q67. What do you mean by meta Programming in Ruby? Explain how you can implement this in your program?</summary>

----
**Metaprogramming** in Ruby is the ability for code to write code—defining or modifying methods, classes, or behavior at runtime. Ruby is extremely metaprogramming-friendly with features like `define_method`, `send`, `method_missing`, and `eval`.  

**Example using `define_method`:**  

    class DynamicClass
      [:name, :email].each do |attr|
        define_method(attr) do
          instance_variable_get("@#{attr}")
        end

        define_method("#{attr}=") do |value|
          instance_variable_set("@#{attr}", value)
        end
      end
    end

This dynamically defines getters/setters for `name` and `email`.  

**Uses in Rails:**  
- ActiveRecord dynamically defines attribute readers/writers from DB columns.  
- `method_missing` enables `find_by_name`, `find_by_email`, etc.  

**Caution:** While powerful, overusing metaprogramming can reduce readability and make debugging hard. Use it deliberately for DSLs, dynamic query generation, or reusable abstractions.  
</details>
<!-- ------------------- END Q67 ------------------- -->

----
<!-- ------------------ BEGIN Q68 ------------------ -->
<details>
  <summary>Q68. What do you mean by inject method in Ruby?</summary>

----
The `inject` (or `reduce`) method in Ruby is an **enumerator method** that accumulates results across elements of a collection.  

Example: Sum of array:  

    [1, 2, 3, 4].inject(0) { |sum, n| sum + n }
    # => 10

How it works:  
- Takes an initial accumulator (0 here).  
- Passes each element and the accumulator into the block.  
- Returns the accumulated result after iteration.  

**Use cases:**  
- Summing, multiplying, building hash maps, custom aggregations.  

Example: Convert array to hash:  

    [:a, :b, :c].inject({}) { |h, k| h[k] = k.to_s; h }

**Inject** is versatile and compact, but sometimes less readable than simple loops. It’s ideal for functional programming-style aggregations.  
</details>
<!-- ------------------- END Q68 ------------------- -->

----
<!-- ------------------ BEGIN Q69 ------------------ -->
<details>
  <summary>Q69. What is the difference between equal? and eql? method in Ruby?</summary>

----
- **equal?** → Compares object identity (checks if both references point to the same object in memory). Example:  

    a = "hello"
    b = a
    a.equal?(b) # true  

- **eql?** → Compares both value and type. Example:  

    1.eql?(1.0) # false (different types)  
    1.eql?(1)   # true  

**Also:** `==` compares only value, not type strictly.  

**Summary:**  
- `equal?` → strict identity check.  
- `eql?` → checks value + type (used by Hash keys).  
- `==` → usually just value.  

In practical terms, use `==` for equality, `eql?` for Hash keys, and reserve `equal?` for identity checks.  
</details>
<!-- ------------------- END Q69 ------------------- -->

----
<!-- ------------------ BEGIN Q70 ------------------ -->
<details>
  <summary>Q70. What is the advantage of using hash over an array in Ruby?</summary>

----
The advantage of a **Hash** over an **Array** is that Hashes provide **key-based access** instead of index-based.  

**Benefits of Hash:**  
- Constant time (`O(1)`) access for lookups by key.  
- Readability: `user[:email]` is clearer than `user[3]`.  
- Flexibility: Keys can be strings, symbols, numbers, or even objects.  
- Useful for modeling data where order doesn’t matter but key-to-value mapping is essential.  

Arrays work best for ordered lists or sequential data, while Hashes shine in scenarios where descriptive access is needed or when representing structured records (like JSON objects).  
</details>
<!-- ------------------- END Q70 ------------------- -->

----
<!-- ------------------ BEGIN Q71 ------------------ -->
<details>
  <summary>Q71. What is the difference between iterators and loops in Ruby?</summary>

----
- **Loops** (`while`, `for`, `until`) are **control structures** that repeat a block of code based on conditions. They are lower-level constructs, procedural in nature.  
- **Iterators** are Ruby methods like `.each`, `.map`, `.select`, `.inject` that work on enumerable objects and yield execution to blocks.  

**Example loop:**  

    i = 0
    while i < 5
      puts i
      i += 1
    end  

**Example iterator:**  

    (0..4).each { |i| puts i }  

**Key differences:**  
- Iterators are more idiomatic and Ruby-like.  
- Loops require explicit counters or conditions.  
- Iterators are chainable and functional, often preferred for clarity.  

In Ruby, iterators are encouraged over raw loops since they are safer, more concise, and align with Ruby’s higher-level programming style.  
</details>
<!-- ------------------- END Q71 ------------------- -->

----
<!-- ------------------ BEGIN Q72 ------------------ -->
<details>
  <summary>Q72. What are accessor methods in Ruby? List and explain accessor methods.</summary>

----
Accessor methods control attribute access in a Ruby class. Instead of writing manual getters/setters, Ruby provides convenience macros:  

1. **attr_reader** → Creates getter method only.  
   Example:  

       attr_reader :name  
       # creates def name; @name; end  

2. **attr_writer** → Creates setter method only.  
   Example:  

       attr_writer :name  
       # creates def name=(value); @name = value; end  

3. **attr_accessor** → Creates both getter and setter methods.  
   Example:  

       attr_accessor :name  

**Benefits:**  
- Simplifies code, improves readability.  
- Encapsulation enforced by using getters/setters rather than exposing instance variables directly.  

This is heavily relied on in Rails models and POROs.  
</details>
<!-- ------------------- END Q72 ------------------- -->

----
<!-- ------------------ BEGIN Q73 ------------------ -->
<details>
  <summary>Q73. What are class level and module level attributes?</summary>

----
In Ruby/Rails, you can define attributes accessible on class or module objects.  

- **Class-level attributes:** Store values that apply to the class, not instances. Achieved via `cattr_accessor`. Example:  

    class AppConfig
      cattr_accessor :api_key
    end  

    AppConfig.api_key = "123"  

- **Module-level attributes:** Similar, but inside modules. Used for shared configs. Example:  

    module Settings
      mattr_accessor :currency
    end

    Settings.currency = "USD"  

**Use cases:**  
- Global configurations, caching, library settings.  

**Caution:** Shared mutable state can cause issues in multithreading or tests, so prefer dependency injection or constants where possible.  
</details>
<!-- ------------------- END Q73 ------------------- -->

----
<!-- ------------------ BEGIN Q74 ------------------ -->
<details>
  <summary>Q74. What is the difference between include and extend in rails?</summary>

----
Both are ways to mix a module into a class but differ in scope:  

- **include**: Adds module methods as **instance methods**.  
   Example:  
   `include Trackable` → instances can call `track`.  

- **extend**: Adds module methods as **class methods**.  
   Example:  
   `extend Trackable` → class itself can call `track`.  

**Usage:**  
- Use `include` when behavior belongs to instances (e.g., validations, instance helpers).  
- Use `extend` when you want class-level behavior (e.g., configuration setup).  

In Rails, concerns often use `ActiveSupport::Concern` to allow mixing class and instance methods elegantly.  
</details>
<!-- ------------------- END Q74 ------------------- -->

----
<!-- ------------------ BEGIN Q75 ------------------ -->
<details>
  <summary>Q75. How many template engines are supported by Rails? Which one is your preference and why?</summary>

----
Rails supports several template engines for rendering views:  

- **ERB** (default): Simple and built-in, evaluates Ruby in HTML.  
- **HAML**: Cleaner syntax with indentation-based structure.  
- **Slim**: Very minimal syntax, focused on speed and readability.  

Others exist through gems (Liquid, Mustache, etc.).  

**Preference:**  
For most Rails apps, **ERB** is the standard choice because:  
- It’s officially supported and easiest for teams to understand.  
- No extra dependencies required.  
- Easier onboarding for new developers compared to HAML or Slim.  

However, HAML or Slim might improve readability for teams that already have experience with them.  
</details>
<!-- ------------------- END Q75 ------------------- -->

----
<!-- ------------------ BEGIN Q76 ------------------ -->
<details>
  <summary>Q76. What do you mean by singleton (Eigen) class in Ruby?</summary>

----
A **singleton (eigen) class** in Ruby is an anonymous hidden class created for an object to hold methods unique to that object. This is how Ruby supports defining methods on a single instance without affecting other instances.  

Example:  

    str = "hello"
    def str.shout
      upcase + "!"
    end

Here `shout` is defined on `str` only; `str2 = "hello"` won’t have it.  

Internally, Ruby creates a hidden eigenclass for `str` where `shout` is defined.  

**Use cases:**  
- Defining class methods (via eigenclass of class objects).  
- Adding behavior to a single object dynamically.  

This concept underpins metaprogramming in Ruby and allows flexible dynamic modifications.  
</details>
<!-- ------------------- END Q76 ------------------- -->

----
<!-- ------------------ BEGIN Q77 ------------------ -->
<details>
  <summary>Q77. When do you think is the right time to define a helper method inside a controller in Rails?</summary>

----
Helper methods in controllers should be defined when logic is needed across **views rendered by this controller**, not specific to one view or template.  

Example:  

    class UsersController < ApplicationController
      helper_method :current_user
      def current_user
        @current_user ||= User.find(session[:user_id])
      end
    end  

This makes `current_user` accessible in views without re-defining logic inside helpers.  

**When to use:**  
- Only when the method logically belongs to the controller’s responsibility and is tightly coupled to that controller.  
- For logic shared across all controllers/views, move it to `ApplicationController` or `ApplicationHelper`.  

**Rule of thumb:** Use controller helper methods sparingly. For formatting or view presentation, use helpers. For reusable partials, use presenters or view components.  
</details>
<!-- ------------------- END Q77 ------------------- -->

----
<!-- ------------------ BEGIN Q78 ------------------ -->
<details>
  <summary>Q78. What is your understanding of DRY code? Explain.</summary>

----
**DRY (Don’t Repeat Yourself)** is a software design principle that emphasizes reducing code duplication by promoting reuse and abstraction.  

**In Rails:**  
- Use **concerns** for repeating logic across models/controllers.  
- Use **partials** in views for repeating UI snippets.  
- Extract business workflows into **service objects** for reuse.  
- Use **helpers** for formatting.  
- Prefer **scopes** in models instead of repeating query logic in controllers.  

**Why DRY matters:**  
- Improves maintainability (update logic in one place).  
- Reduces bugs caused by inconsistencies.  
- Makes code easier for new developers to understand.  

However, DRY should be applied carefully—over-abstraction can reduce clarity. The goal is balance: reduce duplication while keeping the codebase understandable and explicit where needed.  
</details>
<!-- ------------------- END Q78 ------------------- -->

----
<!-- ------------------ BEGIN Q79 ------------------ -->
<details>
  <summary>Q79. What is your approach to write a thin controller? Also explain why a controller should be thin and what are the advantages of it?</summary>

----
A **thin controller** follows the philosophy that controllers should only handle request/response coordination, not business logic.  

**My approach:**  
- Push business logic into models, service objects, or background jobs.  
- Use scopes for reusable queries.  
- Rely on serializers/presenters for response formatting.  
- Use before_action filters only for common setup.  
- Extract reusable workflows into POROs or concerns.  

**Why controllers should be thin:**  
- Improves maintainability by centralizing logic in testable units (e.g., models/services).  
- Makes controllers easier to read and ensures consistency across actions.  
- Simplifies testing since business logic is independent and can be tested without HTTP request overhead.  

**Advantages:** Faster development, fewer bugs, cleaner separation of concerns, and a codebase that’s easier to scale and onboard new developers into.  
</details>
<!-- ------------------- END Q79 ------------------- -->

----
<!-- ------------------ BEGIN Q80 ------------------ -->
<details>
  <summary>Q80. What is the purpose of initializers directory in a rails project?</summary>

----
The **`config/initializers`** directory in Rails loads Ruby files during application startup. They are used to configure gems, set global variables, or adjust application-level behavior before requests start.  

**Examples:**  
- Setting Rails configuration:  

    Rails.application.config.time_zone = "Asia/Kolkata"  

- Configuring gems:  

    Devise.setup do |config|
      config.mailer_sender = 'support@app.com'
    end  

- Monkey-patching third-party libraries or setting constants.  

**Best practices:**  
- Keep initializers small and purposeful.  
- Don’t overload them with application business logic—they should only configure and initialize.  
- Group related configuration into separate initializer files (`devise.rb`, `sidekiq.rb`, etc.) for clarity.  

They are crucial for setting up application-wide settings uniformly across environments.  
</details>
<!-- ------------------- END Q80 ------------------- -->

  </details>

---- 
<!-- ------------------------------------------ END Q61 - Q80 ------------------------------------------ -->






<!-- ----------------------------------------- BEGIN Q81 - Q100 ----------------------------------------- -->
  <details>
    <summary>Q81 - Q100</summary>

<!-- ------------------ BEGIN Q81 ------------------ -->
<details>
  <summary>Q81. What is the difference between a gem and Rails engine?</summary>

----
- **Gem**: A packaged library of Ruby code. It can provide functionalities usable in any Ruby/Rails project. Gems don’t necessarily follow Rails structure and usually extend the language or add utilities. Example: `devise`, `nokogiri`.  

- **Rails Engine**: A mini Rails application that can plug into another Rails app. It has its own `app/`, `config/`, routes, controllers, views, models, and initializers. An engine is essentially a "gem with Rails inside it." Example: `Devise` itself is implemented as an engine.  

**Difference:**  
- A gem is general-purpose Ruby; an engine specifically extends Rails functionality.  
- Engines can mount routes and provide isolated Rails codebases; gems usually can’t.  

Rails engines are best when building reusable Rails components that feel like part of the application itself. Gems work better when building general-purpose Ruby libraries.  
</details>
<!-- ------------------- END Q81 ------------------- -->

----
<!-- ------------------ BEGIN Q82 ------------------ -->
<details>
  <summary>Q82. What do you mean by a rails engine? Explain when we need to use a rails engine? Also if you know, list a few gems which are engines as well.</summary>

----
A **Rails engine** is essentially a Rails app that can be embedded into another Rails app. Engines encapsulate functionality such as models, controllers, routes, and views and ship as gems. When mounted into a host app, the engine behaves as if it’s part of the host.  

**When to use:**  
- When building modular, reusable pieces of functionality (authentication, e-commerce modules, CMS).  
- When multiple applications need to share the same logic/UI.  
- For large monoliths where splitting functionality into engines improves maintainability.  

**Examples of gems that are engines:**  
- **Devise** – authentication engine.  
- **Spree** – E-commerce engine.  
- **Forem** – Forum engine.  
- **RailsAdmin / ActiveAdmin** – admin engines.  

Engines are particularly useful for enterprises with multiple apps sharing common functionality. Instead of duplicating code, create an engine and plug it into all apps.  
</details>
<!-- ------------------- END Q82 ------------------- -->

----
<!-- ------------------ BEGIN Q83 ------------------ -->
<details>
  <summary>Q83. Is it possible to use two identical keys in a hash? What happens if you use two identical keys in a hash?</summary>

----
In Ruby hashes, **keys must be unique**. If you use the same key twice, the last written value overrides the earlier one.  

Example:  

    h = { name: "Alice", name: "Bob" }
    h[:name] # => "Bob"  

The second entry overwrites the first because hash keys are unique.  

If you require multiple values for a single name, use:  
- An **array** as the value → `name: ["Alice", "Bob"]`.  
- A **multi-value hash structure** using libraries.  

So, *two identical keys cannot coexist; the last one always wins*.  
</details>
<!-- ------------------- END Q83 ------------------- -->

----
<!-- ------------------ BEGIN Q84 ------------------ -->
<details>
  <summary>Q84. What is the best way to define a foreign key into an existing table in rails?</summary>

----
Rails provides migration helpers for foreign keys. The best practice is to use `add_reference` or `add_foreign_key`.  

Example with `add_reference`:  

    add_reference :comments, :post, foreign_key: true  

This creates `post_id` column in `comments` and adds a foreign key constraint.  

Alternatively:  

    add_foreign_key :comments, :posts  

**Why best practice?**  
- Ensures referential integrity at the DB level.  
- Works consistently across environments.  
- Helps prevent orphaned rows.  

Always prefer explicit foreign keys in migrations for better data reliability.  
</details>
<!-- ------------------- END Q84 ------------------- -->

----
<!-- ------------------ BEGIN Q85 ------------------ -->
<details>
  <summary>Q85. How many rails versions have you worked with? Also list the changes between the rails versions you have worked on.</summary>

----
This depends on personal experience. For a mid-senior engineer, expected answer:  

"I’ve worked with Rails 5, 6, and 7."  

**Major changes between them:**  
- **Rails 5** introduced ActionCable, API-only mode, Attributes API.  
- **Rails 6** featured multiple database support, ActionMailbox, ActionText, Parallel Testing, and Zeitwerk autoloader.  
- **Rails 7** modernized assets: dropped default Webpacker, added Importmaps, ESBuild, Propshaft, and Hotwire integration by default. It also enhanced asynchronous queries.  

As a candidate, emphasize familiarity with differences like autoloading (classic vs Zeitwerk), asset management, new Action framework features, and scalability improvements.  
</details>
<!-- ------------------- END Q85 ------------------- -->

----
<!-- ------------------ BEGIN Q86 ------------------ -->
<details>
  <summary>Q86. What is the difference between Array and Enumerator?</summary>

----
- **Array**: A concrete data structure that stores values in memory and grants access by index. Example: `[1,2,3]`.  
- **Enumerator**: An object representing deferred iteration. It doesn’t hold data itself but defines how to enumerate over it.  

Example:  

    arr = [1, 2, 3]
    enum = arr.each
    enum.class # => Enumerator
    enum.next  # => 1  

**Benefits of Enumerator:**  
- Lazy evaluation.  
- Can represent infinite sequences (e.g., `(1..Float::INFINITY).lazy`).  
- Useful for chaining operations without loading all data into memory.  

**Summary:** Arrays store actual data; Enumerators model iteration over data. Enumerator = abstract iteration, Array = actual structure.  
</details>
<!-- ------------------- END Q86 ------------------- -->

----
<!-- ------------------ BEGIN Q87 ------------------ -->
<details>
  <summary>Q87. What is your preference for return response for an API? Jbuilder or ActiveModel serializers? And why?</summary>

----
Both tools enable Rails to format structured API responses:  

- **Jbuilder**: View-based JSON builder using templates. Flexible, integrates into Rails views. Easy for APIs sharing logic with server-rendered views.  
- **ActiveModel Serializers (AMS)**: Model-based serializer classes. Helps keep logic near models, supports relationships, and makes API consistent.  

**Preference:**  
For large APIs, I prefer **ActiveModel Serializers** because they enforce consistent structures, handle relationships elegantly, and keep template logic out of controllers. Jbuilder tends to tightly couple views and JSON, making it less portable in large JSON-only APIs.  

However, Jbuilder works fine for small apps or when views + JSON share logic. In API-heavy apps or when following JSON:API standards, AMS is superior.  
</details>
<!-- ------------------- END Q87 ------------------- -->

----
<!-- ------------------ BEGIN Q88 ------------------ -->
<details>
  <summary>Q88. What are the differences between lambda and proc?</summary>

----
Both `lambda` and `proc` are callable objects in Ruby, but they differ in semantics.  

- **lambda**:  
  - Strict arity (checks arguments count).  
  - Treated like a method (returns to caller).  

- **proc**:  
  - Lenient arity (ignores missing/excess arguments).  
  - A `return` inside a proc exits the enclosing method, not just the proc.  

**Example:**  

    l = ->(x,y){ x+y }
    l.call(1,2)        # works
    l.call(1)          # ArgumentError

    p = Proc.new { |x,y| x+y }
    p.call(1)          # => nil

**Usage:**  
- Use lambdas when acting like small functions.  
- Use procs to allow flexible argument handling.  

In Rails, lambdas are widely used in **scopes** because of their strict and predictable behavior.  
</details>
<!-- ------------------- END Q88 ------------------- -->

----
<!-- ------------------ BEGIN Q89 ------------------ -->
<details>
  <summary>Q89. What do you mean by argumented scopes? When do you need to write argumented scopes?</summary>

----
Argumented scopes in Rails are scopes that accept parameters. They make queries reusable with varying arguments.  

Example:  

    scope :created_before, ->(time) { where("created_at < ?", time) }

Now you can call:  
`User.created_before(1.week.ago)`  

**When to use:**  
- When filtering logic varies depending on conditions.  
- For queries that need dynamic parameters (e.g., filtering by age, dates, status).  

Argumented scopes keep controllers concise and reusable by encapsulating logic inside the model. They are essential for DRY query building.  
</details>
<!-- ------------------- END Q89 ------------------- -->

----
<!-- ------------------ BEGIN Q90 ------------------ -->
<details>
  <summary>Q90. What is the difference between update and update_attribute method?</summary>

----
- **update**: Updates record with validation and runs callbacks. Can update multiple attributes. Example: `user.update(name: "John", age: 30)`.  
- **update_attribute**: Updates a single attribute directly in DB, bypasses validations but still triggers callbacks. Example: `user.update_attribute(:name, "John")`.  

**Summary:**  
- `update` → Safe, validations + callbacks.  
- `update_attribute` → Unsafe, skips validations.  
- There’s also `update_column` which skips validations **and** callbacks, directly writing to DB.  

**Best practice:** Always use `update` unless you need to bypass validations intentionally (e.g., admin scripts, fixing corrupted data).  
</details>
<!-- ------------------- END Q90 ------------------- -->

----
<!-- ------------------ BEGIN Q91 ------------------ -->
<details>
  <summary>Q91. What is the difference between :allow_nil and :allow_blank validation options?</summary>

----
- **allow_nil**: Skips validation if the attribute is `nil`. But `""` (empty string) will still be validated.  
- **allow_blank**: Skips validation if value is `nil` or empty string (and other blank values like whitespace `" "`).  

Example:  

    validates :age, numericality: true, allow_nil: true
    validates :email, format: ..., allow_blank: true

**When to use:**  
- Use `allow_nil` when distinction between nil and empty is important.  
- Use `allow_blank` when both nil and empty values should skip validation.  

This subtle difference matters for form inputs since HTML form fields usually submit empty strings instead of nil.  
</details>
<!-- ------------------- END Q91 ------------------- -->

----
<!-- ------------------ BEGIN Q92 ------------------ -->
<details>
  <summary>Q92. What do you mean by strict and conditional validations?</summary>

----
- **Strict validations:** Raise an exception (`ActiveModel::StrictValidationFailed`) instead of just adding errors. Example:  

    validates :email, presence: true, strict: true  

Useful when invalid data is critical and must not silently fail.  

- **Conditional validations:** Executed only if certain conditions are met. Example:  

    validates :discount_code, presence: true, if: -> { promotion_active? }

Conditional validations make models more flexible by applying rules only in relevant contexts.  

**Summary:** Strict validations enforce hard rules by raising errors, while conditional validations allow context-specific checks.  
</details>
<!-- ------------------- END Q92 ------------------- -->

----
<!-- ------------------ BEGIN Q93 ------------------ -->
<details>
  <summary>Q93. When do you need to skip callbacks? List a few of the methods, by using them you can skip callbacks.</summary>

----
Sometimes callbacks aren’t needed for special cases (bulk imports, data cleanup, performance-sensitive scripts). In such cases, skipping callbacks is necessary.  

Rails provides methods that bypass callbacks:  
- `update_column` → updates a single column, no validation/callback.  
- `update_columns` → updates multiple columns, no validation/callback.  
- `toggle!` → skips validations, updates directly.  
- `decrement! / increment!` → modify numeric fields directly.  
- `delete` → removes record without callbacks.  
- `delete_all` → bulk delete without callbacks.  

**Best practice:** Only skip callbacks deliberately, with careful thought. Otherwise, business rules (dependencies, soft deletes) won’t run.  
</details>
<!-- ------------------- END Q93 ------------------- -->

----
<!-- ------------------ BEGIN Q94 ------------------ -->
<details>
  <summary>Q94. Is it possible to send emails without rendering a template in Rails? If yes, how will you do this?</summary>

----
Yes. By default Rails mailers render a view template, but you can send plain text emails by specifying body directly in `mail()`.  

Example:  

    mail(to: "test@example.com", subject: "Hello", body: "This is a plain text email.")

Alternatively, call `mail` with `content_type: 'text/html'` and supply body directly with HTML.  

**When useful:** Quick notification emails, system alerts, or data exports that don’t require full templates.  

However, for maintainability and proper formatting, templates are preferred in most cases.  
</details>
<!-- ------------------- END Q94 ------------------- -->

----
<!-- ------------------ BEGIN Q95 ------------------ -->
<details>
  <summary>Q95. What is the difference between deliver_now and deliver_later methods for sending emails?</summary>

----
- **deliver_now**: Sends the email immediately in the current thread (synchronous). The web request waits for it to complete.  
- **deliver_later**: Enqueues email sending as a background job via ActiveJob (asynchronous). Requires a background worker like Sidekiq.  

**When to use:**  
- Use `deliver_now` for critical notifications in small apps or non-production.  
- Use `deliver_later` in production for better user experience (non-blocking), scalability, and resilience.  

**Best practice:** Always prefer `deliver_later` with a configured queue adapter in production.  
</details>
<!-- ------------------- END Q95 ------------------- -->

----
<!-- ------------------ BEGIN Q96 ------------------ -->
<details>
  <summary>Q96. What do you mean by upsert?</summary>

----
**Upsert** stands for "update or insert." It’s a database operation that either inserts a new row if it doesn’t exist, or updates it if it does.  

Rails supports this with methods like `insert_all` and `upsert_all`.  

Example:  

    User.upsert({ id: 1, name: "Bob" }, unique_by: :id)

If a record with `id=1` exists → updates its name. Otherwise, inserts new record.  

**Use case:** Synchronizing external data, deduplication, ensuring idempotency in data imports.  

It improves performance by avoiding race conditions and double queries (`find_or_create` then update).  
</details>
<!-- ------------------- END Q96 ------------------- -->

----
<!-- ------------------ BEGIN Q97 ------------------ -->
<details>
  <summary>Q97. What do you mean by session storage in Rails? Explain.</summary>

----
**Session storage** in Rails is the mechanism enabling Rails to persist session data across requests. By default, sessions are stored as signed and encrypted cookies on the client-side.  

Other options:  
- **ActiveRecord store** (sessions saved in `sessions` table).  
- **Cache store** (e.g., Redis, Memcached).  
- **Custom stores** via gems.  

How it works:  

    session[:user_id] = current_user.id

This persists `user_id` across requests.  

**Best practice:**  
- Use cookie store for simple apps (default).  
- Use Redis/DB-backed store for large systems with sensitive sessions.  

Session storage is crucial for authentication, personalization, shopping carts, and cross-request statefulness.  
</details>
<!-- ------------------- END Q97 ------------------- -->

----
<!-- ------------------ BEGIN Q98 ------------------ -->
<details>
  <summary>Q98. What do you mean by session hijacking?</summary>

----
**Session hijacking** is a security exploit where an attacker gains unauthorized access to a user’s session by stealing session identifiers (like cookies). Once compromised, the attacker can impersonate the victim.  

**Common attack vectors:**  
- XSS (stealing cookies through injected scripts).  
- Packet sniffing on unencrypted HTTP.  
- Session fixation attacks.  

**Prevention in Rails:**  
- Use HTTPS (encrypt cookies).  
- Rails signs and encrypts session cookies by default.  
- Regenerate session IDs (`reset_session`) after login.  
- Use `same_site` cookie attributes.  

Mitigating session hijacking is essential for secure authentication handling.  
</details>
<!-- ------------------- END Q98 ------------------- -->

----
<!-- ------------------ BEGIN Q99 ------------------ -->
<details>
  <summary>Q99. What are the main features of the asset pipeline in Rails?</summary>

----
The **Asset Pipeline** streamlines asset management in Rails by:  

- **Concatenation**: Combines multiple files to reduce HTTP requests.  
- **Minification**: Reduces file size by removing whitespace/comments.  
- **Fingerprinting**: Appends unique hash to filenames → enables long cache lifetimes with instant cache busts.  
- **Preprocessing**: Allows SCSS, CoffeeScript, and ERB inside assets.  
- **Logical paths**: Provides helpers like `asset_path`, `javascript_include_tag`.  
- **Organized folders**: `app/assets`, `lib/assets`, `vendor/assets`.  

These features make Rails asset handling production-ready, optimized, and secure. Rails 7 introduces **Propshaft** as a simpler successor.  
</details>
<!-- ------------------- END Q99 ------------------- -->

----
<!-- ------------------ BEGIN Q100 ------------------ -->
<details>
  <summary>Q100. What do you mean by page caching, action caching and fragment caching?</summary>

----
Rails supports multiple caching strategies:  

1. **Page caching** (deprecated in Rails 4+): Stores entire generated HTML pages on disk, served by webserver. Very fast, but no longer supported natively.  
2. **Action caching**: Caches output of entire controller action but still runs filters (useful when auth is needed). Deprecated but available via gems.  
3. **Fragment caching**: Most common in modern Rails. Caches parts of a view with `cache` helper. Example:  

    <%= cache @post do %>
      <%= render @post.comments %>
    <% end %>  

Only the fragment is cached, so partial updates trigger re-render.  

**Best practice today:** Use **fragment caching** with Redis/Memcached + `low-level caching` APIs. Combine with Russian-doll caching for nested partials for maximum efficiency.  
</details>
<!-- ------------------- END Q100 ------------------- -->

  </details>

---- 
<!-- ------------------------------------------ END Q81 - Q100 ------------------------------------------ -->






<!-- ----------------------------------------- BEGIN Q101 - Q120 ----------------------------------------- -->
  <details>
    <summary>Q101 - Q120</summary>

<!-- ------------------ BEGIN Q101 ------------------ -->
<details>
  <summary>Q101. Why does ruby not support method overloading?</summary>

----
Ruby does not support **traditional method overloading** (like Java or C++ where multiple methods with the same name but different argument signatures can exist). In Ruby, if you define multiple methods with the same name, the last definition overrides all previous ones.  

**Reason:**  
- Ruby’s dynamic typing doesn’t require explicit method signatures (argument types are not declared).  
- Instead of overloading, Ruby uses **default arguments**, **variable arguments (`*args`)**, and **keyword arguments** to provide flexibility.  

**Example equivalent of overloading:**  

    def greet(name = "Guest", age = nil)
      puts age ? "Hello #{name}, #{age} years old" : "Hello #{name}"
    end

So instead of overloading, Ruby embraces flexible argument handling to keep the language simple and dynamic. This makes it concise but relies more on runtime checks.  
</details>
<!-- ------------------- END Q101 ------------------- -->

----
<!-- ------------------ BEGIN Q102 ------------------ -->
<details>
  <summary>Q102. What are modules in Ruby? How can you differentiate class and instance methods in a module?</summary>

----
A **module** in Ruby is a collection of methods, constants, and classes. Unlike classes, modules cannot be instantiated. They serve two purposes:  
1. Namespacing (grouping related code to avoid collisions).  
2. Mixins (sharing reusable functionality between classes).  

**Differentiating methods:**  
- **Instance methods**: Defined normally in the module. Classes `include` the module to get these methods.  
- **Class methods**: Defined with `self.method_name` in the module. Classes `extend` the module to get these.  

Example:  

    module Trackable
      def track     # instance method
        puts "Tracking"
      end

      def self.log  # class method
        puts "Log action"
      end
    end

    class User
      include Trackable
    end

    User.new.track   # works
    Trackable.log    # works

Modules are heavily used in Rails via `ActiveSupport::Concern` for clean mixins that define both instance and class methods.  
</details>
<!-- ------------------- END Q102 ------------------- -->

----
<!-- ------------------ BEGIN Q103 ------------------ -->
<details>
  <summary>Q103. What is the difference between after_save and after_commit?</summary>

----
Both are callbacks, but they trigger at different stages of persistence.  

- **after_save**: Runs after the model is saved, whether by create or update, but **before the database transaction is committed**. If the transaction rolls back afterward, side effects may already have occurred.  
- **after_commit**: Runs only once the transaction is fully committed successfully. It ensures side effects occur only if the database changes are permanent.  

**Example use cases:**  
- Use `after_save` for in-memory logic, like caching attributes.  
- Use `after_commit` for sending emails, triggering background jobs, or notifications since these should only happen if the DB record persists.  

**Best practice:** Always prefer `after_commit` for side effects to avoid sending wrong or duplicate notifications in case of rollbacks.  
</details>
<!-- ------------------- END Q103 ------------------- -->

----
<!-- ------------------ BEGIN Q104 ------------------ -->
<details>
  <summary>Q104. What are mixins in Ruby?</summary>

----
**Mixins** are a way to include functionality from a module into a class. Unlike inheritance, which is single in Ruby, mixins allow sharing behavior across multiple classes without creating deep hierarchies.  

Example:  

    module Flyable
      def fly
        "I'm flying!"
      end
    end

    class Bird
      include Flyable
    end

Now `Bird.new.fly` works.  

**Advantages of Mixins:**  
- Avoid code duplication.  
- Provide multiple inheritance-like behavior.  
- Improve modularity and organization of reusable logic.  

Mixins are the foundation for Rails concerns—large applications lean on this to DRY up models and controllers.  
</details>
<!-- ------------------- END Q104 ------------------- -->

----
<!-- ------------------ BEGIN Q105 ------------------ -->
<details>
  <summary>Q105. What do you mean by the send method in Ruby?</summary>

----
The **send** method in Ruby invokes a method dynamically by its name as a symbol or string.  

Example:  

    user = "Alice"
    user.send(:upcase)   # => "ALICE"  

You can even call private/protected methods:  

    class Demo
      private def hello; "hi"; end
    end
    Demo.new.send(:hello) # => "hi"  

**Use cases:**  
- Metaprogramming (calling methods dynamically).  
- DRY design when method names are computed at runtime.  
- Avoid repeating similar code blocks.  

**Caution:** Since `send` bypasses access control (private/protected), it should not be exposed to untrusted input. Use `public_send` if you want respect for method visibility.  
</details>
<!-- ------------------- END Q105 ------------------- -->

----
<!-- ------------------ BEGIN Q106 ------------------ -->
<details>
  <summary>Q106. Have you worked with sidekiq? Why is it used for?</summary>

----
Yes, **Sidekiq** is a background job processing tool for Rails applications. It is used for executing potentially long-running tasks outside of the main web request/response cycle, thus improving app performance and user experience.  

**Why use it?**  
- Offload heavy tasks: email sending, PDF generation, API calls.  
- It uses Redis to store job queues, ensuring persistence.  
- Sidekiq is multi-threaded and highly efficient compared to alternatives like Resque.  
- Supports retries, scheduled jobs, and monitoring with a web UI.  

In production systems, Sidekiq is almost a standard choice when background processing is required.  
</details>
<!-- ------------------- END Q106 ------------------- -->

----
<!-- ------------------ BEGIN Q107 ------------------ -->
<details>
  <summary>Q107. What is the difference between the basic version of sidekiq and sidekiq pro?</summary>

----
- **Sidekiq Basic (Open Source):** Provides core functionality like job queues, retries, retries with backoff, and scheduled jobs. Perfect for most small to medium apps.  
- **Sidekiq Pro (Commercial License):** Adds advanced features:  
  - Reliable fetch (ensures no job loss even during crashes).  
  - Batch jobs (group jobs with callbacks).  
  - Rate limiting.  
  - More queue features like "pause queues."  
- **Sidekiq Enterprise:** Adds even more features like rolling restarts, leader election, security tools.  

**Summary:** Use free Sidekiq for simple apps. Use Pro/Enterprise for enterprises requiring advanced scaling, reliability, and monitoring.  
</details>
<!-- ------------------- END Q107 ------------------- -->

----
<!-- ------------------ BEGIN Q108 ------------------ -->
<details>
  <summary>Q108. What are perform and perform_async methods in sidekiq? What is the difference between them?</summary>

----
When defining a Sidekiq worker:  

    class MailerWorker
      include Sidekiq::Worker
      def perform(user_id)
        UserMailer.welcome_email(User.find(user_id)).deliver_now
      end
    end

- **perform**: This is the instance method implemented in the worker. It contains the job logic that runs in the background process. You normally never call this directly.  
- **perform_async**: Class method used to enqueue a job to Redis asynchronously. Example:  

    MailerWorker.perform_async(user.id)  

This pushes the job into Redis queue, and later Sidekiq picks it up and executes `perform`.  

**In short:** `perform_async` enqueues, `perform` executes.  
</details>
<!-- ------------------- END Q108 ------------------- -->

----
<!-- ------------------ BEGIN Q109 ------------------ -->
<details>
  <summary>Q109. What is the difference between let and let! in RSpec?</summary>

----
In RSpec:  
- **let**: Lazily evaluated. Code inside is executed only when the value is first referenced in the test. Subsequent references reuse the memoized value.  
- **let!**: Eagerly evaluated. Code is executed before each example (like a `before` block), regardless of whether the value is used.  

**Example:**  

    let(:user) { create(:user) }
    let!(:post) { create(:post) }

Here, user is created only if referenced. Post is created before each test no matter what.  

**Best practice:**  
- Use `let` for avoiding unnecessary setup.  
- Use `let!` for setup that must always happen (e.g., side-effects, DB constraints).  
</details>
<!-- ------------------- END Q109 ------------------- -->

----
<!-- ------------------ BEGIN Q110 ------------------ -->
<details>
  <summary>Q110. What are the callbacks? Explain for both the model and controller.</summary>

----
**Callbacks** are hooks in Rails where custom logic runs at specific lifecycle points.  

- **Model callbacks (ActiveRecord):** Triggered during object creation, validation, updating, deletion, or commit. Examples:  
  - `before_validation`, `after_validation`  
  - `before_save`, `after_save`, `before_create`  
  - `after_commit`, `after_destroy`  
  They are used for enforcing consistency, cleaning data, or triggering side effects.  

- **Controller callbacks (filters):** Triggered around controller actions. Examples:  
  - `before_action` (run logic before actions → e.g., authentication).  
  - `after_action` (tracking/logs).  
  - `around_action` (wrap logic around an action).  

**Difference:**  
Model callbacks affect database record lifecycle. Controller callbacks manage request/response lifecycle.  
</details>
<!-- ------------------- END Q110 ------------------- -->

----
<!-- ------------------ BEGIN Q111 ------------------ -->
<details>
  <summary>Q111. What is the difference between uniq and distinct in rails?</summary>

----
Both ensure unique results in queries, but differ slightly:  

- **uniq**: Ruby method (on arrays/results) that removes duplicates in-memory at Ruby level. Deprecated in favor of `distinct`.  
- **distinct**: SQL-level uniqueness. Generates `SELECT DISTINCT …` query.  

Example:  

    User.select(:age).distinct  
    User.pluck(:age).uniq  

In the first, SQL query ensures uniqueness in DB. In the second, Rails fetches all ages then Ruby removes duplicates, which can be inefficient.  

**Best practice:** Always use `distinct` for ActiveRecord queries to leverage DB efficiency.  
</details>
<!-- ------------------- END Q111 ------------------- -->

----
<!-- ------------------ BEGIN Q112 ------------------ -->
<details>
  <summary>Q112. In rails how you will get objects with at least one child?</summary>

----
If you want a parent with at least one associated child, you can use `joins` or `where.exists`.  

Example with joins:  

    Post.joins(:comments).distinct  

This returns posts that have ≥1 comment.  

Alternatively, use `where exists`:  

    Post.where.exists(:comments)  

Rails 6+ adds scopes like `.where.associated(:comments)`.  

**Best practice:** Use SQL joins to ensure filtering at DB rather than instantiating all objects. Adding `.distinct` ensures no duplicates.  
</details>
<!-- ------------------- END Q112 ------------------- -->

----
<!-- ------------------ BEGIN Q113 ------------------ -->
<details>
  <summary>Q113. In what cases the change method is not reversible in a Rails migration?</summary>

----
`change` method in migrations is not reversible when the opposite of an operation is ambiguous. Examples:  
- `remove_column` without specifying column type and options.  
- Arbitrary SQL with `execute`.  
- Complex data migrations that transform data one-way.  
- Renaming indexes with `rename_index` (Rails <= 4.2).  

If Rails cannot infer rollback, it will raise `IrreversibleMigration`.  

**Solution:** Use explicit `up` and `down` methods in such cases to define exact rollback behavior.  
</details>
<!-- ------------------- END Q113 ------------------- -->

----
<!-- ------------------ BEGIN Q114 ------------------ -->
<details>
  <summary>Q114. What happens if you do not provide the column type in the remove_column migration?</summary>

----
If you write `remove_column :users, :age` without specifying type, Rails cannot automatically reverse the migration (rollback). It raises an `IrreversibleMigration` error because on rollback Rails doesn’t know what type `:age` was.  

**Fix:** Always specify the type:  

    remove_column :users, :age, :integer  

Or else define explicit `up` and `down` methods showing how to recreate the column.  
</details>
<!-- ------------------- END Q114 ------------------- -->

----
<!-- ------------------ BEGIN Q115 ------------------ -->
<details>
  <summary>Q115. What happens if you rollback a change_column migration within the change method?</summary>

----
If you use `change_column` inside a `change` block, Rails **cannot reverse it automatically** unless you specify both from- and to-types. It raises `IrreversibleMigration` on rollback.  

Example:  

    change_column :users, :age, :string  

Rollback cannot know the previous type.  

**Solution:** Write explicit `up` and `down`:  

    def up
      change_column :users, :age, :string
    end

    def down
      change_column :users, :age, :integer
    end  

Always document the original type for reversible schema management.  
</details>
<!-- ------------------- END Q115 ------------------- -->

----
<!-- ------------------ BEGIN Q116 ------------------ -->
<details>
  <summary>Q116. What is the difference between preload and includes?</summary>

----
Both load associations but differ in how:  

- **preload**: Always fires separate queries for associations. Example: 1 query for parent, 1 for child collection.  
- **includes**: Decides strategy:  
  - If no child conditions → runs preload-like multiple queries.  
  - If child conditions/ordering are applied → runs a `LEFT OUTER JOIN`.  

**Performance difference:**  
- `preload` = predictability (separate queries).  
- `includes` = sometimes joins.  

Use `preload` when you want guaranteed separation, and `includes` when you want Rails to optimize based on query conditions.  
</details>
<!-- ------------------- END Q116 ------------------- -->

----
<!-- ------------------ BEGIN Q117 ------------------ -->
<details>
  <summary>Q117. How many ways to eager loading the associations?</summary>

----
Ways to eager load in Rails:  

1. **includes** – Eager loads, dynamically decides between multiple queries and a join.  
2. **preload** – Forces eager loading through separate queries.  
3. **eager_load** – Forces eager loading through a single `LEFT OUTER JOIN`.  
4. **joins + select** – Can preload manually, but not typical.  

**Examples:**  

    User.includes(:posts)  
    User.preload(:posts)  
    User.eager_load(:posts)  

**Best practice:**  
- Use `includes` by default to avoid N+1.  
- Use `preload` for guaranteed separate queries.  
- Use `eager_load` when adding conditions based on associations.  
</details>
<!-- ------------------- END Q117 ------------------- -->

----
<!-- ------------------ BEGIN Q118 ------------------ -->
<details>
  <summary>Q118. What do you mean by content_for in Rails?</summary>

----
`content_for` is a Rails helper to capture blocks of view content for later rendering in layouts. Useful when layouts need custom parts like extra JavaScript or sidebars.  

Example:  

    <% content_for :scripts do %>
      <script src="custom.js"></script>
    <% end %>

Then in layout:  

    <%= yield :scripts %>  

**Benefits:**  
- Keeps views DRY by injecting page-specific code into layouts.  
- Great for partials needing additional head/footer content.  
- Improves flexibility for complex layouts.  
</details>
<!-- ------------------- END Q118 ------------------- -->

----
<!-- ------------------ BEGIN Q119 ------------------ -->
<details>
  <summary>Q119. What do you mean by sanitizing params in Rails?</summary>

----
Sanitizing params is the process of filtering user input before using it in queries or assignments. In Rails, it prevents **mass assignment vulnerabilities** and SQL injection.  

**Techniques:**  
- Use **Strong Parameters** (`permit`, `require`).  
- Escape query input with `sanitize_sql_for_conditions`.  
- In views, use `sanitize` or `h` helper to escape HTML.  

Example:  

    params.require(:user).permit(:name, :email)  

**Why important?** User input is untrusted. Sanitizing protects against security vulnerabilities, ensures only allowed attributes are persisted, and prevents malicious code injection via forms/API.  
</details>
<!-- ------------------- END Q119 ------------------- -->

----
<!-- ------------------ BEGIN Q120 ------------------ -->
<details>
  <summary>Q120. What is the difference between render and redirect in Rails?</summary>

----
- **render**: Sends a response immediately without a new HTTP request. You can render a view, partial, or JSON. Example:  

    render :new  

Does not change URL.  

- **redirect_to**: Issues an HTTP 302/301 redirect, instructing browser to make a new request to another URL. Example:  

    redirect_to posts_path  

URL changes, and the browser does another request.  

**Rule of thumb:**  
- Use `render` to display a template in the same request.  
- Use `redirect_to` for POST-redirect-GET patterns, navigation changes, or avoiding duplicate submissions.  
</details>
<!-- ------------------- END Q120 ------------------- -->

  </details>

---- 
<!-- ------------------------------------------ END 101 - Q120 ------------------------------------------ -->






<!-- ----------------------------------------- BEGIN Q121 onwards ----------------------------------------- -->
  <details>
    <summary>Q121 onwards</summary>

<!-- ------------------ BEGIN Q121 ------------------ -->
<details>
  <summary>Q121. What is the difference between module and concerns in Rails?</summary>

----
Both **modules** and **concerns** allow sharing reusable code, but concerns are Rails’ specialized pattern built on top of modules.  

- **Module**: Plain Ruby construct grouping methods/constants. To use them in a class, you do `include` or `extend`.  

- **Concern**: Rails’ extension (`ActiveSupport::Concern`) that makes including modules more structured:
  - Supports separating **class methods** and **instance methods** easily.  
  - Handles dependency ordering when modules extend each other.  

**Example:**

    module Trackable
      extend ActiveSupport::Concern
      included do
        before_save :track
      end
      def track; puts "tracked"; end
      class_methods do
        def tracked_count; count; end
      end
    end

**Key difference:** Concerns are modules + syntactic sugar for clean Rails-compatible organization. Use them when sharing code across models/controllers.  
</details>
<!-- ------------------- END Q121 ------------------- -->

----
<!-- ------------------ BEGIN Q122 ------------------ -->
<details>
  <summary>Q122. What is cattr_accessor ?</summary>

----
`cattr_accessor` is a Rails method that creates **class-level attributes** (similar to `attr_accessor` but at class scope instead of instance scope).  

Example:

    class Config
      cattr_accessor :setting
    end

    Config.setting = "Production"
    Config.setting # => "Production"

**Behavior:**  
- Provides both getter and setter methods on the class.  
- Not tied to instance objects — values shared across all instances.  

Used commonly for global configuration values or feature flags in Rails applications.  
</details>
<!-- ------------------- END Q122 ------------------- -->

----
<!-- ------------------ BEGIN Q123 ------------------ -->
<details>
  <summary>Q123. What is difference between cattr_accessor and attr_accessor ?</summary>

----
- **attr_accessor**: Defines instance-level getters/setters (each object has its own values).  

    class User
      attr_accessor :name
    end
    u1 = User.new; u1.name = "Alice"
    u2 = User.new; u2.name = "Bob"
    # Separate values for each instance  

- **cattr_accessor**: Defines class-level getters/setters (shared across all objects).  

    class User
      cattr_accessor :role
    end
    User.role = "admin"
    User.new.role # => "admin"  

**Summary:**  
Use `attr_accessor` for per-object state, `cattr_accessor` for shared/global state applicable across all instances of the class.  
</details>
<!-- ------------------- END Q123 ------------------- -->

----
<!-- ------------------ BEGIN Q124 ------------------ -->
<details>
  <summary>Q124. What is difference between sub and gsub method in Ruby?</summary>

----
- **sub**: Replaces the **first occurrence** of a pattern in a string.  

    "hello world".sub("o", "0") # => "hell0 world"  

- **gsub** (`global substitute`): Replaces **all occurrences** of a pattern.  

    "hello world".gsub("o", "0") # => "hell0 w0rld"  

**Use cases:**  
- `sub`: when only one replacement is needed.  
- `gsub`: when you need to replace across the entire string.  

Both accept regex, making them powerful for text manipulation.  
</details>
<!-- ------------------- END Q124 ------------------- -->

----
<!-- ------------------ BEGIN Q125 ------------------ -->
<details>
  <summary>Q125. How to set a custom primary key in rails model other than id?</summary>

----
By default Rails uses `id` as the primary key, but you can override with `self.primary_key`.  

Example:  

    class User < ApplicationRecord
      self.primary_key = "uuid"
    end

Now Rails will use the `uuid` column as the primary key for all CRUD operations.  

**Best practices:**  
- Ensure DB column is unique and indexed.  
- Often combined with UUIDs for distributed systems (`enable_extension 'pgcrypto'` in Postgres).  

This is common in enterprise apps where surrogate keys or UUIDs are preferred over auto-increment IDs.  
</details>
<!-- ------------------- END Q125 ------------------- -->

----
<!-- ------------------ BEGIN Q126 ------------------ -->
<details>
  <summary>Q126. How to provide custom name to a model table in rails ?</summary>

----
Rails models map to pluralized table names by default. If your DB uses a different name, override it with `self.table_name`.  

Example:  

    class UserProfile < ApplicationRecord
      self.table_name = "user_info"
    end

Now `UserProfile.all` runs queries against `user_info` table.  

**When useful:**  
- Integrating legacy schemas with non-Rails naming conventions.  
- Working in environments where DB uses custom table names.  

Best practice: Stick to Rails conventions whenever possible; only override where strictly needed to avoid confusing teammates.  
</details>
<!-- ------------------- END Q126 ------------------- -->

----
<!-- ------------------ BEGIN Q127 ------------------ -->
<details>
  <summary>Q127. What is the difference between is_a? and instance_of? methods in Ruby? Which one you will prefer?</summary>

----
- **is_a?**: Checks if an object is an instance of the given class **or subclass**.  

    "hello".is_a?(String)      # => true  
    "hello".is_a?(Object)      # => true  

- **instance_of?**: Checks only if the object is an **exact instance** of the specified class, not subclasses.  

    "hello".instance_of?(String)   # => true  
    "hello".instance_of?(Object)   # => false  

**Which to prefer?**  
Most of the time, `is_a?` is preferred since it respects inheritance and is more flexible in polymorphic designs. Use `instance_of?` when you require exact class matching.  

**Summary:**  
- `is_a?` → checks class & inheritance tree.  
- `instance_of?` → checks exact class only.  
</details>
<!-- ------------------- END Q127 ------------------- -->

  </details>
<!-- ------------------------------------------ END 121 onwards ------------------------------------------ -->


</details>

----
