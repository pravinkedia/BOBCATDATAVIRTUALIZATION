# BOBCATDATAVIRTUALIZATION

### LOAD Data in DB2 WH

### Virtualize tables in Data Virtualization for above 3 tables

### Join tables to check the DV results

select E.*,D.DEPTNAME, D.MGRNO, M.FIRSTNME,M.MIDINIT, M.LASTNAME 
from DEV3.EMPLOYEE E, CP4D.DEPARTMENT D, DEV3.EMPLOYEE M 
WHERE E.WORKDEPT = D.DEPTNO and D.MGRNO=M.EMPNO

