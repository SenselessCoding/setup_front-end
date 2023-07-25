# setup_front-end
Just a generic frontend / backend configuration 

### XAMPP for DB

- Install [XAMPP](https://sourceforge.net/projects/xampp/files/) *(if you don't have any specifications, use the default setup-wizard settings)*
- For MyAdmin you need to start `Apache` and `MySQL`  
  ![xampp_start](https://github.com/SenselessCoding/setup_front-end/assets/139842164/e130dba7-9780-4f14-bd8b-ec591516701f)
- Open [PhpMyAdmin](http://localhost/phpmyadmin) (localhost/phpmyadmin)
- You can create/import your DB now. It's recommended to use smt like MySqlWorkbench or Datagrip for its usability, <br>anyhow for default proof-of-concept stuff like this you can neglect those
  
---
### MySQL-Workbench
- Install [MySQL-Workbench](https://dev.mysql.com/downloads/workbench/)
- Give the connection a name(f.e:my_db_connector)
- Host is localhost(127.0.0.1), Port 3306(like shown in XAMPP)
- User is root and password is empty

  Either create your DB manually or do it with an ERM
- Click `File` - `New Model` - Modify `DB name` if wanted - Click `Add Diagram`
- Once you are done you can click `Database` - `Forward Engineer`
- Keep the basic values in the wizard, make sure connect is correct
---

### Fleet

  - Your backend should be set now, for a simple web-application we use good ol' ``PHP``
  - Use a editor of your choice, I will be using [Fleet](https://www.jetbrains.com/de-de/fleet/download/#section=windows).

### Workspace prep

- Find your xampp folder
```
D:\xampp\htdocs
```
and completly wipe it.

- In your editor, use this folder to display elements on you page
  ![workspace](https://github.com/SenselessCoding/setup_front-end/assets/139842164/7c9290ab-7065-4aa3-a876-59493d26bb41)

- If you want to test the page, create a `index.php` file and paste following in
```php
<?php
phpinfo();
?>
```
