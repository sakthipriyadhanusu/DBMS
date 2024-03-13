# EXP NO 1: ER DIAGRAM CREATION, RELATIONAL MODEL AND SCHEMA GENERATION  
### DATE
## AIM:
<div align="justify">
   To create a ER Diagram for Bank management system or College management system using ERD Plus tool and generate the relational model with schema. 
</div>

## Algorithm
1. Create a login with https://erdplus.com.
2. Create a new ER Diagram with name
3. Create a strong entity, relation and attributes.
4. Create a weak entity, relation and attributes.
5. Specify attributes unique, multivalued and composite attributes.

### ER Diagram 
![Screenshot 2024-03-13 103750](https://github.com/sakthipriyadhanusu/DBMS/assets/119393194/ac7b985a-beac-4ae9-9b44-d4b8076aa002)

### Relational model
![image](https://github.com/sakthipriyadhanusu/DBMS/assets/119393194/d7a6334e-fa7d-46f5-a169-74488f6eac6b)

### SQL DDL Schema 

CREATE TABLE COLLEGE
(
  Coffice INT NOT NULL,
  Cphone INT NOT NULL,
  Cname INT NOT NULL,
  PRIMARY KEY (Cname)
);

CREATE TABLE INSTRUCTOR
(
  Iphone INT NOT NULL,
  Iname INT NOT NULL,
  Ioffice INT NOT NULL,
  rank INT NOT NULL,
  Id INT NOT NULL,
  PRIMARY KEY (Id)
);

CREATE TABLE DEPT
(
  Dname INT NOT NULL,
  Doffice INT NOT NULL,
  Dcode INT NOT NULL,
  Dphone INT NOT NULL,
  PRIMARY KEY (Dname),
  UNIQUE (Dcode)
);

CREATE TABLE COURSE
(
  Ccode INT NOT NULL,
  Credits INT NOT NULL,
  Cdesc INT NOT NULL,
  level INT NOT NULL,
  Coname INT NOT NULL,
  PRIMARY KEY (Ccode)
);

CREATE TABLE STUDENT
(
  SId INT NOT NULL,
  DOB INT NOT NULL,
  Fname INT NOT NULL,
  Lname INT NOT NULL,
  addr INT NOT NULL,
  phone INT NOT NULL,
  major INT NOT NULL,
  PRIMARY KEY (SId)
);

CREATE TABLE SECTION
(
  Secid INT NOT NULL,
  secno INT NOT NULL,
  sem INT NOT NULL,
  year INT NOT NULL,
  bldg INT NOT NULL,
  roomno INT NOT NULL,
  daystime INT NOT NULL,
  PRIMARY KEY (Secid)
);

## RESULT 
<div align="justify">
Thus the ER diagram was drawn and relational diagram, SQL DDL staements are generated using ERD plus tool.
</div>
