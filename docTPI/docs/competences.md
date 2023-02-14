# Première compétence

Je sais utiliser un langage de gestion de données relationnelles (SQL). 
Je sais également les appliquées à un langage de programmation (PHP).

### Exemple de requête SQL pour récupérer des données.
```sql
SELECT * FROM users WHERE id = 1
```

### Exemple de reuqête SQL pour modifier des données.
```sql
UPDATE users SET name = 'John' WHERE id = 1
```

### Exemple de requête SQL pour supprimer des données.
```sql
DELETE FROM users WHERE id = 1
```

### Exemple de requête SQL pour créer une base de données.
```sql
CREATE DATABASE IF NOT EXISTS `my_database` DEFAULT CHARACTER SET utf8 COLLATE utf8_general_ci;
```

### Exemple de requête SQL pour créer une table.
```sql
CREATE DATABASE IF NOT EXISTS `my_database` DEFAULT CHARACTER SET utf8 COLLATE utf8_general_ci;
USE `my_database`;

CREATE TABLE IF NOT EXISTS `users` (
  `id` int(11) NOT NULL AUTO_INCREMENT,
  `name` varchar(255) NOT NULL,
  `surname` varchar(255) NOT NULL,
  `sex` varchar(255) NOT NULL,
  PRIMARY KEY (`id`)
) ENGINE=InnoDB DEFAULT CHARSET=utf8;
```

### Exemple de requête PDO pour récupérer des données.
```php
$sql = "SELECT * FROM users WHERE id = 1";
$stmt= $pdo->prepare($sql);
$stmt->execute();
$result = $stmt->fetch();
```

### Exemple de requête PDO pour modifier des données.
```php
$data = [
    'name' => 'John',
    'id' => 1,
];
$sql = "UPDATE users SET name = :name WHERE id = :id";
$stmt= $pdo->prepare($sql);
$stmt->execute($data);
```

### Exemple de requête PDO pour supprimer des données.
```php
$data = [
    'id' => 1,
];
$sql = "DELETE FROM users WHERE id = :id";
$stmt= $pdo->prepare($sql);
$stmt->execute($data);
```

### Exemple de requête PDO pour créer une base de données.
```php
$sql = "CREATE DATABASE IF NOT EXISTS `my_database` DEFAULT CHARACTER SET utf8 COLLATE utf8_general_ci;";
$stmt= $pdo->prepare($sql);
$stmt->execute();
```

### Exemple de requête PDO pour créer une table.
```php
$sql = "CREATE DATABASE IF NOT EXISTS `my_database` DEFAULT CHARACTER SET utf8 COLLATE utf8_general_ci;
USE `my_database`;

CREATE TABLE IF NOT EXISTS `users` (
  `id` int(11) NOT NULL AUTO_INCREMENT,
  `name` varchar(255) NOT NULL,
  `surname` varchar(255) NOT NULL,
  `sex` varchar(255) NOT NULL,
  PRIMARY KEY (`id`)
) ENGINE=InnoDB DEFAULT CHARSET=utf8;";
$stmt= $pdo->prepare($sql);
$stmt->execute();
```

