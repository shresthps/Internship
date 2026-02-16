INSERT INTO authors (name) VALUES 
('J.K. Rowling'),
('George Orwell'),
('Jane Austen');

INSERT INTO books (title, author_id) VALUES
('Harry Potter', 1),
('1984', 2),
('Pride and Prejudice', 3),
('Animal Farm', 2);

INSERT INTO members (name, email) VALUES
('Alice Johnson', 'alice@email.com'),
('Bob Smith', NULL),
('Charlie Brown', 'charlie@email.com');

INSERT INTO loans (book_id, member_id, loan_date, return_date) VALUES
(1, 1, '2026-02-01', NULL),
(2, 2, '2026-02-05', '2026-02-10');

UPDATE members
SET email = 'bob@email.com'
WHERE member_id = 2;

UPDATE loans
SET return_date = '2026-02-15'
WHERE loan_id = 1;

DELETE FROM books
WHERE book_id = 4;
