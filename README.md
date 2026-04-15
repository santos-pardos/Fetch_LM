
# Fetch

## Links
```
https://pokeapi.co/
```
```
https://rapidapi.com/hub
```
```
https://jsonplaceholder.typicode.com/
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
Host aws-ec2
    HostName ec2-44-229-243-8.us-west-2.compute.amazonaws.com
    User ec2-user
    IdentityFile c:\Temp\labsuser.pem
```

```
Change permissions in the Labuser.pem and config files
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
