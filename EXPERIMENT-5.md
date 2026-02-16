### 6. EXP5 – Aggregate and String Functions

- *Q1. Count total number of employees*

  sql
  SELECT COUNT(*) FROM EMPLOYEE;
  

- *Q2. Display sum of salaries of all employees*

  sql
  SELECT SUM(SAL) FROM EMPLOYEE;
  

- *Q3. Display maximum salary*

  sql
  SELECT MAX(SAL) FROM EMPLOYEE;
  

- *Q4. Display minimum salary*

  sql
  SELECT MIN(SAL) FROM EMPLOYEE;
  

- *Q5. Display average salary*

  sql
  SELECT AVG(SAL) FROM EMPLOYEE;
  

- *Q6. Display maximum salary among clerks*

  sql
  SELECT MAX(SAL) FROM EMPLOYEE
  WHERE JOB = 'CLERK';
  

- *Q7. Display maximum salary in department 20*

  sql
  SELECT MAX(SAL) FROM EMPLOYEE
  WHERE DEPTNO = 20;
  

- *Q8. Display minimum salary among salesmen*

  sql
  SELECT MIN(SAL) FROM EMPLOYEE
  WHERE JOB = 'SALESMAN';
  

- *Q9. Display average salary of managers*

  sql
  SELECT AVG(SAL) FROM EMPLOYEE
  WHERE JOB = 'MANAGER';
  

- *Q10. Display total salary of analysts in department 40*

  sql
  SELECT SUM(SAL) FROM EMPLOYEE
  WHERE JOB = 'ANALYST' AND DEPTNO = 40;
  

- *Q11. Display employee names in uppercase*

  sql
  SELECT UPPER(ENAME) AS EMPLOYEE_NAME
  FROM EMPLOYEE;
  

- *Q12. Display employee names in lowercase*

  sql
  SELECT LOWER(ENAME) AS EMPLOYEE_NAME
  FROM EMPLOYEE;
  

- *Q13. Display employee names in proper case (first letter capital, rest small)*

  sql
  SELECT CONCAT(UPPER(LEFT(ENAME, 1)), LOWER(SUBSTRING(ENAME, 2)))
  FROM EMPLOYEE;
  

- *Q14. Display length of the string 'PRIYANSHU KUMAR YADAV'*

  sql
  SELECT LENGTH('TANISHA KUMARI');
  

- *Q15. Display length of each employee name along with EMPNO and ENAME*

  sql
  SELECT LENGTH(ENAME), EMPNO, ENAME
  FROM EMPLOYEE;
  

---