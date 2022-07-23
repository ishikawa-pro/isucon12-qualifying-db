## tables
```
+--------------------+
| Tables_in_isuports |
+--------------------+
| id_generator       |
| tenant             |
| visit_history      |
+--------------------+
```

##  columns

### id_generateor
```
+-------+---------+------+-----+---------+----------------+
| Field | Type    | Null | Key | Default | Extra          |
+-------+---------+------+-----+---------+----------------+
| id    | bigint  | NO   | PRI | NULL    | auto_increment |
| stub  | char(1) | NO   | UNI |         |                |
+-------+---------+------+-----+---------+----------------+
```

### tenant
```
+--------------+--------------+------+-----+---------+----------------+
| Field        | Type         | Null | Key | Default | Extra          |
+--------------+--------------+------+-----+---------+----------------+
| id           | bigint       | NO   | PRI | NULL    | auto_increment |
| name         | varchar(255) | NO   | UNI | NULL    |                |
| display_name | varchar(255) | NO   |     | NULL    |                |
| created_at   | bigint       | NO   |     | NULL    |                |
| updated_at   | bigint       | NO   |     | NULL    |                |
+--------------+--------------+------+-----+---------+----------------+
```

### visit_history
```
+----------------+-----------------+------+-----+---------+-------+
| Field          | Type            | Null | Key | Default | Extra |
+----------------+-----------------+------+-----+---------+-------+
| player_id      | varchar(255)    | NO   |     | NULL    |       |
| tenant_id      | bigint unsigned | NO   | MUL | NULL    |       |
| competition_id | varchar(255)    | NO   |     | NULL    |       |
| created_at     | bigint          | NO   |     | NULL    |       |
| updated_at     | bigint          | NO   |     | NULL    |       |
+----------------+-----------------+------+-----+---------+-------+
```
