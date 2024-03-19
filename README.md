# Creación de Backend
## Instrucciones
Clonar repositorio
```
git clone https://github.com/ElOpti/backend_jasg.git
```
## Creación de la base de datos
```
create database apliweb;
```
```
create table tbl_usuario (
	email varchar(100) primary key,
	password varchar(250) not null,
	role varchar(20) not null
);
```
```
insert into tbl_usuario(email, password, role) values ('artugamer8@gmail.com', 'admin','admin');
```
## Peticiones
### Login (Post)
#### URL
```
http://localhost:3000
```
### Estructura
```
{
    "email":"artugamer8@gmail.com",
    "password":"admin"
}
```
### Get
#### URL
```
http://localhost:3000/usuario
```
### Post
#### Estructura
```
{
    "email":"lolo@gmail.com",
    "password":"admin",
    "role":"admin"
}
```
### Put
#### Estructura
```
{
    "email":"artugamer8@gmail.com",
    "password":"admin"
}
```
### Delete
#### Estructura
```
{
    "email":"lolo@gmail.com"
}
```
