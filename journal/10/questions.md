# CSharp and SQL Fundamentals
01. What is the purpose of a `namespace`?

  > exporting classes and methods within classes

02. What is the difference between a `class` and an `interface`?

  > a class has both a definition and an implementation whereas an interface only has a definition.

03. What is the method that returns an instance of a class, yet it has no return type?

  > void

05. In the Car example what is the access modifier of the `Start()` method?

  ```c#
  abstract class Car
  {
    public string Start()
    {

      return "Vroooom";

    }
  }
  ```

  > public

06. In the Car example what is `string` an indication of?

  > data type

07. In the Car example what is `abstract` preventing?

  > Implementation

08. In a SQL table, what is the difference between information in a row and information in a column?

  > rows are an instance of data in the table, while colums are a schema/layout for said data to follow.

09. Demonstrate the necessary SQL for creating a table called `characters` with the values `name, age, description` as strings, and an `int` id.

  > CREATE TABLE
    characters(
      id INT NOT NULL primary key AUTO_INCREMENT,
      name VARCHAR(255) NOT NULL,
      age VARCHAR(255) NOT NULL,
      description VARCHAR(255)
    )default cahrset utf8 COMMENT '';

10. In SQL how can you query more than a single table? Provide an example.

  > Join

  SELECT
  movies.*,
  accounts.*
  FROM movies
  JOIN accounts ON acc.id = movie.creatorId
