
# Fetch

## Links
```
https://pokeapi.co/
```
```
https://rapidapi.com/hub
https://rapidapi.com/weatherapi/api/weatherapi-com
```
```
https://jsonplaceholder.typicode.com/
https://jsonplaceholder.typicode.com/users
https://jsonplaceholder.typicode.com/todos/
```
## VS Code
```
Install SSH Remote Plug-in (Microsoft)
```
```
Remote-SSH:Open Configuration File...
/users/santos/.ssh/config
```


```
Host Linux-AWS
    HostName 44.229.243.8
    User ec2-user
    IdentityFile c:\Temp\labsuser.pem
```

```
Change permissions in the Labuser.pem (R) and config (WRX) files. 
(Linux chmod 400. Windows (remove all users, add the windows user)
```
## Apache
```
yum install httpd -y
systemctl start httpd
systemctl enable httpd
```

## Permisos 
```
sudo chown -R $USER:$USER /var/www/html
sudo chmod -R 755 /var/www/html
```
