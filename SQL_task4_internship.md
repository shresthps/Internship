SELECT 
    category,
    customer_id,
    COUNT(order_id) AS total_orders,
    SUM(quantity) AS total_quantity,
    SUM(quantity * price) AS total_sales,
    AVG(quantity * price) AS avg_order_value
FROM orders
GROUP BY category, customer_id
HAVING SUM(quantity * price) > 1000;
