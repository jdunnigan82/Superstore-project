# Superstore-project

-- SQL query that orders the items by price

SELECT item_name, price
FROM superstore
ORDER BY price;

-- SQL query that will show a statistic about the item prices, like a sum, average, minimum, maximum, or count.


SELECT item_name, category, price, average_rating
FROM superstore
ORDER BY average_rating DESC LIMIT 1;


-- SQL query that will show a statistic about the price for items in the category of "Kitchen Supplies"


SELECT category, AVG(price) AS average_price
FROM superstore
WHERE category = 'Kitchen Supplies'
GROUP BY category;

