# RAVE_FASHION
CREATE TABLE rave (id INTEGER PRIMARY KEY, item TEXT, quantity INTEGER, price INTEGER, discount INTEGER ); 

/* 15 MOST SOLD ITEMS */
INSERT INTO rave VALUES (1, "shirt", 5, 12, 6);
INSERT INTO rave VALUES (2, "shorts", 5, 10, 5);
INSERT INTO rave VALUES (3, "pants", 5, 15, 10);
INSERT INTO rave VALUES (4, "bra", 10, 20, 5);
INSERT INTO rave VALUES (5, "socks", 8, 5, 3);
INSERT INTO rave VALUES (6, "necklace", 5, 10, 4);
INSERT INTO rave VALUES (7, "earrings", 9, 7, 3);
INSERT INTO rave VALUES (8, "leggings", 6, 15, 6);
INSERT INTO rave VALUES (9, "swimsuit", 9, 25, 7);
INSERT INTO rave VALUES (10, "mugs", 3, 8, 2);
INSERT INTO rave VALUES (11, "posters", 5, 10, 3);
INSERT INTO rave VALUES (12, "pens", 8, 5, 1);
INSERT INTO rave VALUES (13, "eyeshadow", 6, 10, 3);
INSERT INTO rave VALUES (14, "lipgloss", 5, 5, 1);
INSERT INTO rave VALUES (15, "chapstick", 5, 5, 2);

SELECT * FROM rave ORDER BY price;

/* What's the highest discount at rave? */  
SELECT MAX(discount) as most_discounted_items FROM rave

/* What is the average item sold at rave? */ 
SELECT AVG(item) FROM rave;

/* How many items cost more than 5 at rave? */
SELECT COUNT(*) AS greater_than_5
FROM rave WHERE price > 5;
