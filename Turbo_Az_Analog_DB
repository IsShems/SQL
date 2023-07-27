--DROP DATABASE TurboAz;
CREATE DATABASE TurboAz;
GO

--DROP TABLE Cars
--GO
--DROP TABLE Showrooms
--GO
--DROP TABLE BodyTypes
--GO
--DROP TABLE Cities
--GO
--DROP TABLE Colors
--GO
--DROP TABLE WheelDriveTypes
--GO
--DROP TABLE FuelType
--GO
--DROP TABLE TranspissionTypes
--GO

USE TurboAz;
GO

CREATE TABLE Cars (
	Id integer IDENTITY(1,1) PRIMARY KEY,
	[Name] nvarchar(15) NOT NULL,
	[Make] nvarchar(15) NOT NULL,
    [Model] nvarchar(15) NOT NULL,
    [Year]  DATETIME NOT NULL,
    [VIN] nvarchar(15) NOT NULL,
    [Mileage] integer NOT NULL,
    [EngineVolume] integer NOT NULL,
    [HorsePower] integer NOT NULL,
    [PassengerCount] integer NOT NULL,
    [Price] integer NOT NULL,
    [PhoneNumber] char(7),
    [BodyTypeId] integer NOT NULL, 
    [CityId] integer NOT NULL, 
    [ColorId] integer NOT NULL, 
    [WheelDriveTypeId] integer NOT NULL,
    [FuelTypeId] integer NOT NULL,
    [TransmissionTypeId] integer NOT NULL

);
GO

CREATE TABLE Showrooms (
	Id integer IDENTITY(1,1) PRIMARY KEY,
	[Name] nvarchar(20) NOT NULL,
	[PhoneNumber] char(7),
	[Address] nvarchar(30) NOT NULL,
	CONSTRAINT FK_ShowRoomId FOREIGN KEY (Id) REFERENCES Showrooms(Id)
);


CREATE TABLE BodyTypes (
	Id integer IDENTITY(1,1) PRIMARY KEY,
	[Bodies] nvarchar(15) NOT NULL,
	CONSTRAINT FK_BodyTypeId FOREIGN KEY (Id) REFERENCES BodyTypes(Id)
);

CREATE TABLE Cities (
	Id integer IDENTITY(1,1) PRIMARY KEY,
	[city] nvarchar(15) NOT NULL,
	CONSTRAINT FK_CityId FOREIGN KEY (Id) REFERENCES Cities(Id)
);

CREATE TABLE Colors (
	Id integer IDENTITY(1,1) PRIMARY KEY,
	[color] nvarchar(15) NOT NULL,
	CONSTRAINT FK_ColorId FOREIGN KEY (Id) REFERENCES Colors(Id)
);

CREATE TABLE WheelDriveTypes (
	Id integer IDENTITY(1,1) PRIMARY KEY,
	[WheelDriveType] nvarchar(15) NOT NULL,
	CONSTRAINT FK_WheelDriveTypeId FOREIGN KEY (Id) REFERENCES WheelDriveTypes(Id)
);

CREATE TABLE FuelType (
	Id integer IDENTITY(1,1) PRIMARY KEY,
	[FuelType] nvarchar(15) NOT NULL,
	CONSTRAINT FK_FuelTypeId FOREIGN KEY (Id) REFERENCES FuelType(Id)
);

CREATE TABLE TranspissionTypes (
	Id integer IDENTITY(1,1) PRIMARY KEY,
	[TranspissionType] nvarchar(15) NOT NULL,
	CONSTRAINT FK_TranspissionTypeId FOREIGN KEY (Id) REFERENCES TranspissionTypes (Id)
);

GO

--test
SELECT *
FROM Cars;
SELECT *
FROM Showrooms;
SELECT *
FROM BodyTypes;
SELECT *
FROM Cities;
SELECT *
FROM Colors;
SELECT *
FROM WheelDriveTypes;
SELECT *
FROM FuelType;
SELECT *
FROM TranspissionTypes;

