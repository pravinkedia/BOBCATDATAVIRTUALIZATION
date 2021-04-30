# BOBCATDATAVIRTUALIZATION

#### LOAD Data in DB2 WH

Use Instructions from DataVirtualization_DB2WH_DataLoad_LAB1.docx file

#### Virtualize tables in Data Virtualization for 3 tables in your own schema with above 3 load files

Use Instructions from DataVirtualization_DB2WH_DB2Cloud_VT_LAB2.docx file

#### Join tables to check the DV results

        select E.*,D.DEPTNAME, D.MGRNO, M.FIRSTNME,M.MIDINIT, M.LASTNAME 
        from DEV3.EMPLOYEE E, CP4D.DEPARTMENT D, DEV3.EMPLOYEE M 
        WHERE E.WORKDEPT = D.DEPTNO and D.MGRNO=M.EMPNO;

##### DB2 Warehouse Tables Locally
        
        select * from DVUC.BILLING_DB2WH;
        select * from DVUC.PRODUCTS_DB2WH;
        select * from DVUC.CUSTOMER_SERVICE_DB2WH;

##### DB2 Virtualize table join between DB2 WH on CP4D and DB2 WH on Cloud accounts
        
        select B.*, P.* from DEV3.BILLING_DB2WH B, PRAVIN.PRODUCTS_DB2CLOUD P WHERE B.CUSTOMERID = P."customerID";



