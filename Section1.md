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