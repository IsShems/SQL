--DROP DATABASE Artopia;
CREATE DATABASE Artopia;
GO

USE Artopia;
GO

CREATE TABLE PeopleData (
	Id integer IDENTITY(1,1) PRIMARY KEY,
	[Name] nvarchar(15) NOT NULL,
	[Surname] nvarchar(15) NOT NULL,
    [NickName] nvarchar(15) NOT NULL,
    [Password] nvarchar(15) NOT NULL,
    [Email] nvarchar(15) NOT NULL,
    [Birth]  DATETIME NOT NULL,
    [PhoneNumber] char(10),
	[Adress] nvarchar(30) NOT NULL,
    [IsSeller] char(1) NOT NULL,
    [Card_] integer NOT NULL,
    [Product] integer NOT NULL
);
GO

CREATE TABLE Card_ (
	Id integer IDENTITY(1,1) PRIMARY KEY,
	[Number] nvarchar(20) NOT NULL,
	[Validity] char(4),
	[Name] nvarchar(15) NOT NULL,
	[Surname] nvarchar(15) NOT NULL,
    [CVV] char(3),
	CONSTRAINT FK_Card_Id FOREIGN KEY (Id) REFERENCES Card_(Id)
);

CREATE TABLE Product (
	Id integer IDENTITY(1,1) PRIMARY KEY,
	[Name] nvarchar(15) NOT NULL,
	[Description] nvarchar(150) NOT NULL,
    [Category] char(3),
    [Price] char(1000),
    [Rating]  int NOT NULL,
    [Favorite] char(1000), --number of people that click favorite
	[Review] integer NOT NULL, 
	CONSTRAINT FK_ProductId FOREIGN KEY (Id) REFERENCES Product(Id)
);

CREATE TABLE Review (
	Id integer IDENTITY(1,1) PRIMARY KEY,
	[Comment] nvarchar(150) NOT NULL,
    [Rating]  int NOT NULL,
	CONSTRAINT FK_ReviewId FOREIGN KEY (Id) REFERENCES Review(Id)
);

GO

INSERT INTO PeopleData ([Name], Surname, NickName, [Password], Email, Birth, PhoneNumber, Adress, IsSeller, Card_, Product)
VALUES ('Shems', 'Ismayilova', 'IsShems', '123', 'ishems@list.ru', 18-05-2004, 0702315006, 'Somewhere', 1, 1, 1);

--test
SELECT [Name]
FROM PeopleData;
SELECT *
FROM Card_;
SELECT *
FROM Product;
SELECT *
FROM Review;
