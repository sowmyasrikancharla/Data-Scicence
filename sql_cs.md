# SQL Case study required code for creating tables 

+ For creating a patient table

CREATE TABLE `test`.`patient\_table` (

`  ``Name` VARCHAR(45) NOT NULL,

`  ``Address` VARCHAR(100) NOT NULL,

`  ``Date\_of\_Birth` VARCHAR(45) NOT NULL,

`  ``Contact\_Details` VARCHAR(12) NOT NULL,

`  `PRIMARY KEY (`Name`),

`  `UNIQUE INDEX `Contact\_Details\_UNIQUE` (`Contact\_Details` ASC) VISIBLE);


+ For creating a medical history table

CREATE TABLE `test`.`medical\_history\_table` (   `Diagnoses\_Yes\_Or\_No` VARCHAR(10) NOT NULL,   `Treatements` VARCHAR(10) NOT NULL,

`  ``Surgeries` VARCHAR(10) NOT NULL,

`  ``Medication` VARCHAR(10) NOT NULL,

`  `PRIMARY KEY (`Diagnoses\_Yes\_Or\_No`));

+ For creating a lab result table

CREATE TABLE `test`.`lab\_result\_table` (   `Blood\_Test` VARCHAR(10) NOT NULL,

`  ``Urine\_Test` VARCHAR(10) NOT NULL,

`  ``Imaging\_Test` VARCHAR(10) NOT NULL);

+ For creating a prescription table

CREATE TABLE `test`.`prescription\_table` (   `Medicine\_Name` VARCHAR(45) NOT NULL,   `Dosage` VARCHAR(45) NOT NULL,

`  ``Frequency` VARCHAR(45) NOT NULL,

`  `PRIMARY KEY (`Medicine\_Name`));

+ For creating a out come table

CREATE TABLE `test`.`out\_come\_table` (

`  ``Read\_Mission\_Rates` INT NOT NULL,

`  ``Medication\_Adherence` VARCHAR(45) NOT NULL,   PRIMARY KEY (`Read\_Mission\_Rates`));
