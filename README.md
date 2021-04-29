# BOBCATDATAVIRTUALIZATION

#### LOAD Data in DB2 WH

Use Instructions from DataVirtualization_LAB1.doc file

#### Virtualize tables in Data Virtualization for 3 tables in your own schema with above 3 load files

Use Instructions from DataVirtualization_LAB2.doc file

#### Join tables to check the DV results

select E.*,D.DEPTNAME, D.MGRNO, M.FIRSTNME,M.MIDINIT, M.LASTNAME 
from DEV3.EMPLOYEE E, CP4D.DEPARTMENT D, DEV3.EMPLOYEE M 
WHERE E.WORKDEPT = D.DEPTNO and D.MGRNO=M.EMPNO


select * from DVUC.BILLING_DB2WH;

select * from DVUC.PRODUCTS_DB2WH;

select * from DVUC.CUSTOMER_SERVICE_DB2WH;



