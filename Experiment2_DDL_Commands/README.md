# Experiment 2: DDL Commands
# NAME : Shri Lekshman Rikhesh R
# Register no : 212224060249
## AIM
To study and implement DDL commands and different types of constraints.

## THEORY

### 1. CREATE
Used to create a new relation (table).

**Syntax:**
```sql
CREATE TABLE (
  field_1 data_type(size),
  field_2 data_type(size),
  ...
);
```
### 2. ALTER
Used to add, modify, drop, or rename fields in an existing relation.
(a) ADD
```sql
ALTER TABLE std ADD (Address CHAR(10));
```
(b) MODIFY
```sql
ALTER TABLE relation_name MODIFY (field_1 new_data_type(size));
```
(c) DROP
```sql
ALTER TABLE relation_name DROP COLUMN field_name;
```
(d) RENAME
```sql
ALTER TABLE relation_name RENAME COLUMN old_field_name TO new_field_name;
```
### 3. DROP TABLE
Used to permanently delete the structure and data of a table.
```sql
DROP TABLE relation_name;
```
### 4. RENAME
Used to rename an existing database object.
```sql
RENAME TABLE old_relation_name TO new_relation_name;
```
### CONSTRAINTS
Constraints are used to specify rules for the data in a table. If there is any violation between the constraint and the data action, the action is aborted by the constraint. It can be specified when the table is created (using CREATE TABLE) or after it is created (using ALTER TABLE).
### 1. NOT NULL
When a column is defined as NOT NULL, it becomes mandatory to enter a value in that column.
Syntax:
```sql
CREATE TABLE Table_Name (
  column_name data_type(size) NOT NULL
);
```
### 2. UNIQUE
Ensures that values in a column are unique.
Syntax:
```sql
CREATE TABLE Table_Name (
  column_name data_type(size) UNIQUE
);
```
### 3. CHECK
Specifies a condition that each row must satisfy.
Syntax:
```sql
CREATE TABLE Table_Name (
  column_name data_type(size) CHECK (logical_expression)
);
```
### 4. PRIMARY KEY
Used to uniquely identify each record in a table.
Properties:
Must contain unique values.
Cannot be null.
Should contain minimal fields.
Syntax:
```sql
CREATE TABLE Table_Name (
  column_name data_type(size) PRIMARY KEY
);
```
### 5. FOREIGN KEY
Used to reference the primary key of another table.
Syntax:
```sql
CREATE TABLE Table_Name (
  column_name data_type(size),
  FOREIGN KEY (column_name) REFERENCES other_table(column)
);
```
### 6. DEFAULT
Used to insert a default value into a column if no value is specified.

Syntax:
```sql
CREATE TABLE Table_Name (
  col_name1 data_type,
  col_name2 data_type,
  col_name3 data_type DEFAULT 'default_value'
);
```

**Question 1**
--
<img width="1010" height="350" alt="Screenshot 2026-09-02 223253" src="https://github.com/user-attachments/assets/106515a7-cc6e-4cb1-a920-3a129b45d965" />



<img width="1142" height="356" alt="Screenshot 2026-09-02 223302" src="https://github.com/user-attachments/assets/25c3bb44-f85a-4825-aac1-b515d3b92310" />



**Output:**

<img width="1263" height="350" alt="Screenshot 2026-09-02 223312" src="https://github.com/user-attachments/assets/3b2ac88b-5cb9-4b82-b3a2-20c44c7f3d8d" />


**Question 2**
<img width="1198" height="352" alt="Screenshot 2026-09-02 223327" src="https://github.com/user-attachments/assets/a3304cc3-c7cd-44fe-a5c2-7b94e2b8eed6" />

-- Paste Question 2 here

<img width="1211" height="166" alt="Screenshot 2026-09-02 223345" src="https://github.com/user-attachments/assets/c1fbc7d4-0044-454e-80e7-54371dca42fb" />


**Output:**

<img width="1237" height="358" alt="Screenshot 2026-09-02 223354" src="https://github.com/user-attachments/assets/665054ba-b1df-4e4c-b27b-a28d840241b4" />


**Question 3**
---
<img width="1230" height="418" alt="Screenshot 2026-09-02 223405" src="https://github.com/user-attachments/assets/8310c1b4-8edd-4476-8124-7f988df0e946" />

<img width="1178" height="262" alt="Screenshot 2026-09-02 223413" src="https://github.com/user-attachments/assets/63ea2a3d-c3a0-4d53-a9e3-440595f51bd1" />


**Output:**

<img width="1193" height="441" alt="Screenshot 2026-09-02 223422" src="https://github.com/user-attachments/assets/1ba0aecd-4805-4047-8f68-50e1624d016e" />

**Question 4**
---
<img width="1215" height="402" alt="Screenshot 2026-09-02 223440" src="https://github.com/user-attachments/assets/c35d522d-c13e-4eee-ad93-d5d14d073f16" />


<img width="1232" height="280" alt="Screenshot 2026-09-02 223447" src="https://github.com/user-attachments/assets/677b1270-6623-4632-988f-3fe72870461d" />


**Output:**

<img width="1215" height="325" alt="Screenshot 2026-09-02 223454" src="https://github.com/user-attachments/assets/795d3831-0487-41ca-bde5-d6dec9267e2c" />


**Question 5**
---
<img width="1050" height="462" alt="Screenshot 2026-09-02 223459" src="https://github.com/user-attachments/assets/1ebd066a-71ce-4e05-8b9c-07baa4b87316" />

<img width="898" height="187" alt="Screenshot 2026-09-02 223505" src="https://github.com/user-attachments/assets/bdf3c490-b299-4c5c-b7b3-a0470e868dcc" />



**Output:**
<img width="1220" height="385" alt="Screenshot 2026-09-02 223511" src="https://github.com/user-attachments/assets/d1204ad0-0fe0-4bb1-a6c3-1f000a00e209" />


**Question 6**
---
<img width="1251" height="315" alt="Screenshot 2026-09-02 223518" src="https://github.com/user-attachments/assets/1aa55cc6-3c99-46b8-8806-edbeb38e072f" />

<img width="840" height="280" alt="Screenshot 2026-09-02 223522" src="https://github.com/user-attachments/assets/b963efbd-acce-4931-a36c-9df411313e46" />


**Output:**

<img width="1275" height="417" alt="Screenshot 2026-09-02 223528" src="https://github.com/user-attachments/assets/7c3b67b5-7de5-4209-8353-883cc8db6330" />


**Question 7**
---
<img width="877" height="387" alt="Screenshot 2026-09-02 223533" src="https://github.com/user-attachments/assets/2b8647ef-8760-4568-8876-e8592cc6719c" />

<img width="880" height="325" alt="Screenshot 2026-09-02 223539" src="https://github.com/user-attachments/assets/1f08e0dc-c26c-4d91-8c13-cd4ce95e02d1" />


**Output:**

<img width="1258" height="466" alt="Screenshot 2026-09-02 223548" src="https://github.com/user-attachments/assets/120cd50e-6f49-4cdc-b230-c0c47669f371" />

**Question 8**
---
<img width="1100" height="332" alt="Screenshot 2026-09-02 223553" src="https://github.com/user-attachments/assets/ef64ca67-4423-42f4-902c-cb36b5f7ffb8" />


<img width="477" height="167" alt="Screenshot 2026-09-02 223558" src="https://github.com/user-attachments/assets/bedb46ad-aa00-49a5-80f9-eabeca499079" />


**Output:**
<img width="1218" height="376" alt="Screenshot 2026-09-02 223605" src="https://github.com/user-attachments/assets/c3fd9b96-b3f0-4bf7-971c-87820af5f0bd" />


**Question 9**
---
<img width="1245" height="577" alt="Screenshot 2026-09-02 223612" src="https://github.com/user-attachments/assets/31e27f08-e868-4a37-b183-5f043d2f68c8" />


<img width="553" height="111" alt="Screenshot 2026-09-02 223616" src="https://github.com/user-attachments/assets/850aac56-db00-4f3e-98c1-99cb18e8771a" />

**Output:**

<img width="1222" height="458" alt="Screenshot 2026-09-02 223622" src="https://github.com/user-attachments/assets/49ec6e91-f1ee-4c24-9824-f82705e0cc68" />


**Question 10**
---
<img width="1235" height="356" alt="Screenshot 2026-09-02 223628" src="https://github.com/user-attachments/assets/3ae45f9e-f2a1-4831-a995-9e019d933702" />
<img width="792" height="311" alt="Screenshot 2026-09-02 223633" src="https://github.com/user-attachments/assets/1c3b1c25-8170-4d43-8de5-334d10a3c353" />


**Output:**

<img width="1327" height="388" alt="Screenshot 2026-09-02 223640" src="https://github.com/user-attachments/assets/c2de36f9-b555-4024-b8dc-3abb16a42dcf" />



## RESULT
Thus, the SQL queries to implement different types of constraints and DDL commands have been executed successfully.
