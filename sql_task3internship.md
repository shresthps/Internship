SELECT * FROM authors;

SELECT name, email 
FROM members
WHERE email IS NOT NULL;

SELECT title 
FROM books
WHERE title LIKE '%Harry%';

SELECT * 
FROM loans
WHERE loan_date BETWEEN '2026-02-01' AND '2026-02-10';

SELECT title, author_id 
FROM books
WHERE author_id = 2
ORDER BY title ASC;

SELECT * 
FROM members
ORDER BY name DESC
LIMIT 2;

SELECT * 
FROM loans
WHERE member_id = 1 AND return_date IS NULL;
