# *SQL Case study required code for creating tables*

+ *For creating a patient table*
---
>CREATE TABLE `test`.`patient_table` (
    `Name` VARCHAR(45) NOT NULL,
    `Address` VARCHAR(100) NOT NULL,
    `Date_of_Birth` VARCHAR(45) NOT NULL,
    `Contact_Details` VARCHAR(12) NOT NULL,
    PRIMARY KEY (`Name`),
    UNIQUE INDEX `Contact_Details_UNIQUE` (`Contact_Details` ASC) VISIBLE
);
#
+ *For creating a medical history table*
---
>CREATE TABLE `test`.`medical_history_table` (
    `Diagnoses_Yes_Or_No` VARCHAR(10) NOT NULL,
    `Treatements` VARCHAR(10) NOT NULL,
    `Surgeries` VARCHAR(10) NOT NULL,
    `Medication` VARCHAR(10) NOT NULL,
    PRIMARY KEY (`Diagnoses_Yes_Or_No`)
);
#
+ *For creating a lab result table*
---
>CREATE TABLE `test`.`lab_result_table` (
    `Blood_Test` VARCHAR(10) NOT NULL,
    `Urine_Test` VARCHAR(10) NOT NULL,
    `Imaging_Test` VARCHAR(10) NOT NULL
);
#
+ *For creating a prescription table*
---
>CREATE TABLE `test`.`prescription_table` (
    `Medicine_Name` VARCHAR(45) NOT NULL,
    `Dosage` VARCHAR(45) NOT NULL,
    `Frequency` VARCHAR(45) NOT NULL,
    PRIMARY KEY (`Medicine_Name`)
);
#
+ *For creating a out come table*
---
>CREATE TABLE `test`.`out_come_table` (
    `Read_Mission_Rates` INT NOT NULL,
    `Medication_Adherence` VARCHAR(45) NOT NULL,
    PRIMARY KEY (`Read_Mission_Rates`)
);
#