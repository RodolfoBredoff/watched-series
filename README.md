<h1 align="center">Watched series</h1>

# Instruções de uso

- Instalar componentes [npm i]


[Back-end](http://localhost:5000/ "Back-end na porta 5000")
<br />
[Front-end](http://localhost:3000/ "Front-end na porta 3000")

```
CREATE TABLE movies(
    id INT PRIMARY KEY AUTO_INCREMENT,
    type INT NOT NULL,
    name VARCHAR(30) NOT NULL,
    total_ep INT,
    atual_ep INT,
    last_view DATE DEFAULT CURRENT_TIMESTAMP
)
```

```
INSERT INTO 
    movies(`id`, `type`, `name`, `total_ep`, `atual_ep`, `last_view`) 
VALUES 
    (1, 0, 'Peaky Blinders', 5, 1, current_timestamp())
```

```
INSERT INTO 
    movies(id, type, name, total_ep, last_view) 
VALUES 
    (2, 1, 'Vikings', NULL, current_timestamp())
```

```
UPDATE 
    `movies` 
SET 
    `last_view` = '2022-03-22' 
WHERE
    `movies`.`id` = 1;
```

```
DELETE FROM
    movies 
WHERE 
    id = 2
```
# watched-series
