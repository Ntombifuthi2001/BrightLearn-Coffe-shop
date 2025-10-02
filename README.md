SELECT*FROM NTOMBI.MYENI.RETAIL_SALES
LIMIT 10;
 ----------------------------------------------------------- 
SELECT customer_id,
        date,
        total_amount
FROM NTOMBI.MYENI.RETAIL_SALES;

------------------------------------------------------------
SELECT DISTINCT gender
FROM NTOMBI.MYENI.RETAIL_SALES;

------------------------------------------------------------
SELECT DISTINCT customer_id,
                total_amount,
                date
FROM NTOMBI.MYENI.RETAIL_SALES;  

---------------------------------------------------------
SELECT*
FROM NTOMBI.MYENI.RETAIL_SALES
WHERE gender ='Male';

-----------------------------------------------------------
SELECT*
FROM NTOMBI.MYENI.RETAIL_SALES
WHERE gender <>'Male';

------------------------------------------------------------------
SELECT *
FROM NTOMBI.MYENI.RETAIL_SALES
WHERE gender !='Male';
------------------------------------------------------------------

SELECT CUSTOMER_ID,
        DATE,
        GENDER,
        product_category
FROM NTOMBI.MYENI.RETAIL_SALES
WHERE GENDER='Female'AND PRODUCT_CATEGORY='Electronics';

--------------------------------------------------------------------
SELECT customer_id,
       date,
       gender,
       product_category
FROM NTOMBI.MYENI.RETAIL_SALES
WHERE GENDER='Female'OR product_category='Electronics';

--------------------------------------------------------------------
SELECT Customer_id,
        date,
        gender,
        product_category
FROM NTOMBI.MYENI.RETAIL_SALES
WHERE product_category IN ('Clothing', 'Beauty');
------------------------------------------------------------

SELECT Customer_id,
        date,
        product_category,
        age,
        total_amount AS revenue
FROM NTOMBI.MYENI.RETAIL_SALES
WHERE age =30;

----------------------------------------------------------

SELECT Customer_id
        date,
        product_category,
        age,
        total_amount AS revenue
FROM NTOMBI.MYENI.RETAIL_SALES
WHERE age >30 AND age <50;
---------------------------------------------------------------
SELECT Customer_id,
        date,
        PRODUCT_CATEGORY,
        age,
        total_amount AS revenue
FROM NTOMBI.MYENI.RETAIL_SALES
WHERE age BETWEEN 30 AND 50;
------ ----------------------------------------------------------
SELECT Customer_id,
        date AS purchase_date,
        product_category,
        age,
        total_amount AS revenue
 FROM NTOMBI.MYENI.RETAIL_SALES
 WHERE purchase_date!='2023-01-25';
----------------------------------------------------------------------
SELECT TRANSACTION_ID,
        Customer_id,
        date AS Purchase_date,
        product_category,
        total_amount AS revenue,
FROM NTOMBI.MYENI.RETAIL_SALES
WHERE Product_category IN ('Clothing', 'Beauty');
------------------------------------------------------------------------
SELECT Customer_id,
        date,
        product_category,
        age,
        total_amount AS revenue
FROM NTOMBI.MYENI.RETAIL_SALES
WHERE age=30;
------------------------------------------------------------------------
SELECT Customer_id,
        date,
        product_category,
        age,
        total_amount AS revenue,
FROM NTOMBI.MYENI.RETAIL_SALES
WHERE age >30 AND age <50;
-------------------------------------------------------------------------
SELECT Customer_id,
       date AS purchase_data,
       product_category,
       age,
       total_amount AS revenue
FROM  NTOMBI.MYENI.RETAIL_SALES      
WHERE age BETWEEN 30 AND 50;
--------------------------------------------------------------------------
SELECT Customer_id,
       date AS purchase_date,
       product_category,
       age,
       total_amount AS revenue
FROM NTOMBI.MYENI.RETAIL_SALES
WHERE purchase_date !='2023-01-25';
-----------------------------------------------------------------------------
SELECT transaction_id,
       CUSTOMER_ID,
       date AS purchase_date,
       product_category,
       total_amount AS revenue
FROM NTOMBI.MYENI.RETAIL_SALES
WHERE product_category IN ('Beauty','clothing');
-----------------------------------------------------------------------
SELECT transaction_id,
       CUSTOMER_ID,
       date AS purchase_date,
       product_category,
       total_amount AS revenue
FROM NTOMBI.MYENI.RETAIL_SALES
WHERE product_category NOT IN ('Beauty','clothing');
------------------------------------------------------------
SELECT transaction_id,
       CUSTOMER_ID,
       AGE,
       date AS purchase_date,
FROM NTOMBI.MYENI.RETAIL_SALES
WHERE age BETWEEN 18AND 20;
------------------------------------------------------------

SELECT Customer_id,
       price_per_unit AS current_price,
       price_per_unit /2 AS discount_Price,
       date AS purchase_date,
FROM NTOMBI.MYENI.RETAIL_SALES
WHERE age BETWEEN 18 AND 20;
       
 -----------------------------------------------------------       

SELECT Customer_id,
       price_per_unit AS CURRENT_price,
       price_per_unit *2 AS double_Price,
       date AS purchase_date,
FROM NTOMBI.MYENI.RETAIL_SALES
WHERE age BETWEEN 18 AND 20;
------------------------------------------------------------       
       
       






