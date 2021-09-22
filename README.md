![portada](https://user-images.githubusercontent.com/68760595/134392773-062fbd52-c21d-4641-b7e9-f4d596fe6ff9.png)


## Clave SSH

1. Crear clave SSH -> desde terminal:

```
ssh-keygen

```
  *elegir contraseña*

![keygen](https://user-images.githubusercontent.com/68760595/134391907-ee2869a5-fef3-4225-9a45-565e1cdc9838.png)

2. Acceder a SSH (desde raíz):

```
cd .ssh

```
```
ls

```
 *aparece clave privada:*
 
 id_rsa
 
 *y clave pública:*
 
 id_rsa.pub
 
 ![ls](https://user-images.githubusercontent.com/68760595/134392348-0aaa61d6-05d4-44d6-87d9-83de31fefe60.png)

3. Examinar contenido clave pública:
```
cat id_rsa.pub

```

4. En Github:

*Settings -> SSH and keys -> new SSH key*

![new](https://user-images.githubusercontent.com/68760595/134393410-3753d290-7fd2-401a-b2e6-2e6c5112c02d.png)

5. Pegar la clave pública:

**desde ssh-rsa...**

**...hasta nombre usuario**

Add key

6. Iniciar agente -> desde terminal:

```
eval $(ssh-agent -s)

```

*Agregar clave:*

```
ssh-add

```
**Crear repositorio para probar autentificación SSH

![prueba](https://user-images.githubusercontent.com/68760595/134398227-084d8ffd-7861-4bbf-be13-fca177a4d8da.png)



