(Ex: list of cities)

What kind of thing are we storing?

What props does it have?

What are the prop types?

Database:
    cities
        columns | name country pop area
        types | string string int int

CREATE TABLE cities (
    name VARCHAR(50),
    country VARCHAR(50),
    population INTEGER,
    area INTEGER
)