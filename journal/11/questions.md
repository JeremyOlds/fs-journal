# A bit more CSharp and SQL
1. What does ***inheritance*** accomplish for us in C#?

  > allows us to use methods or parameters in other controllers, models, etc

2. How does ***member inheritance*** work in C#? Does a `Class` inherit all members of the base `Class`?

  > member inheritence takes in all public and internal members of a class. it does not inherit private classes

3. How does ***accessibility*** affect inheritance?

  > it tells you what can and cannot be accessed. private methods will not be inheritable while public ones will.

4. What is the difference between a `PRIMARY KEY` and a `FOREIGN KEY`

  > primary key is the identifier for the row in the sql table

5. What is an ***alias***?

  > a different name for a table.

6. Demonstrate how you would query a join statement that would get all of a doctors patients from the following collections:

  ```SQL
  CREATE TABLE doctors (
    id INT NOT NULL AUTO_INCREMENT,
    -- CODE OMITTED
    PRIMARY KEY (id)
  )

  CREATE TABLE patients (
    id INT NOT NULL AUTO_INCREMENT,
    -- CODE OMITTED
    PRIMARY KEY (id)
  )

  CREATE TABLE patient_doctors (
    id INT NOT NULL AUTO_INCREMENT,
    doctorId INT NOT NULL,
    patientId INT NOT NULL,

    FOREIGN KEY (doctorId)
      REFERENCES doctors(id),
    FOREIGN KEY (patientId)
      REFERENCES patients(id),
  )

  ```

  > SELECT 
  patients.* ,
  patient_doctors.*
  FROM patients
  JOIN patient_doctors ON patient_doctors.doctorId = @doctorId
  WHERE patients.id = patient_doctors.patientId
