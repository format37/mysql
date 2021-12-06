# docker mysql server
#### Installation
```
git clone https://github.com/format37/mysql.git
cd mysql
mkdir db
mkdir db/data
sh compose.sh
```
#### Client example
[example.ipynb](https://github.com/format37/mysql/blob/main/example.ipynb)
#### Access denied for user 'root'
If u met this error, update user settings inside mysql. Connect over terminal into your container.
```
mysql -u root --password=root
use mysql
SELECT CURRENT_USER();
SET PASSWORD = 'root';
```
