(Ex: list of cities)

What kind of thing are we storing?

What props does it have?

What are the prop types?

Database:
    cities
        columns | name country pop area
        types | string string int int

CREATE TABLE cities (
    name VARCHAR(50), - this creates a name column with a type of string with a 50 char limit
    country VARCHAR(50), - this is another coloumn just like the name
    population INTEGER, - this is a column for the population and the type is a Integer
    area INTEGER - this is the same as the population
)

Keywords are in all caps and Idetifiers are in all lower case

Integer is a number without a decimal within a negative to positive 2 billion

INSERT INTO cities (name, country, population, area) - like the model
VALUES
('Tokyo', 'Japan', 38505000, 8223),
('Shanghai', 'China', 20935999, 3042); adding multiple

SELECT * FROM cities; - getting all the cities

SELECT name FROM cities; - getting all the names of cites

SELECT name, population / area AS population_density
FROM cities; - doing some math, not so hard

SELECT name || ', ' || country AS Location FROM cities;

SELECT UPPER(CONCAT(name, ', ', country)) AS location FROM cities;

(SELECT name, area FROM cities WHERE area > 4000;)

SELECT
    name,
    area
FROM
    cities,
WHERE 
    area NOT IN (3000) AND name = 'Delhi;

Not read from left to right
