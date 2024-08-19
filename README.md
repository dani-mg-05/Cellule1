<p align="center">
   <h1 align="center">Cellule1</h1>
</p>

<p align="center">
  Este proyecto pretende introducirnos a la seguridad web
</p>
<p align="center">
  Tendremos que encontrar algunos archivos en diferentes páginas web explotando sus vulnerabilidades
</p>

---

## Procedimiento
### ex00
<p align="justify">
  En primer lugar, entramos en el siguiente enlace.
</p>

```
http://cybersec.42madrid.com:3317/
```

<br>

<p align="justify">
  Al entrar, nos encontramos lo siguiente.
</p>

![image](https://github.com/user-attachments/assets/e0c48fc9-2291-401e-8c03-d804a0915b5c)

<br>

<p align="justify">
  Si pulsamos en <b>PISTA//HINT</b>, se nos muestra lo siguiente.
</p>

![image](https://github.com/user-attachments/assets/40847056-8aee-47a3-8bca-ec68b3d48620)

<br>

<p align="justify">
  Si miramos la URL, como nos dice el mensaje, vemos lo siguiente.
</p>

```
http://cybersec.42madrid.com:3317/content/hint.html
```

<br>

<p align="justify">
  Con esta información, podemos deducir que si modificamos la URL, en algún punto encontraremos el archivo que estamos buscando.
</p>
<p align="justify">
  Si quitamos <b>hint.html</b>, llegamos a la siguiente página.
</p>

![image](https://github.com/user-attachments/assets/e403bccc-bb12-4538-b621-a7db6e94b745)

<br>

<p align="justify">
  Ahí, nos fijamos en el directorio flag, que si entramos, nos encontramos lo siguiente.
</p>

![image](https://github.com/user-attachments/assets/ca835922-586a-4597-a19e-152d6d27f08f)

<br>

<p align="justify">
  Hemos encontrado el archivo, si lo abrimos, encontramos la solución del ejercicio.
</p>

```
42BCN{f1r5tFl4gG00dJ08}
```

<br>

---

### ex01
<p align="justify">
  Ahora, debemos entrar en el siguiente enlace.
</p>

```
http://cybersec.42madrid.com:3318/
```

<br>

<p align="justify">
  Al entrar, nos encontramos lo siguiente.
</p>

![image](https://github.com/user-attachments/assets/b8276a82-89f3-4819-b1a3-ddad16f384a0)

<br>

<p align="justify">
  Para encontrar el archivo, debemos utilizar técnicas de <i>fuzzing</i>. Gracias a herramientas como <a href="https://github.com/ffuf/ffuf">ffuf</a>, podemos encontrar rutas ocultas dentro de la URL. Por ejemplo, podemos buscar una <a href="https://github.com/maverickNerd/wordlists">lista de palabras comunes</a> y utilizarla con la herramienta que hemos mencionado anteriormente de la siguiente manera.
</p>

![image](https://github.com/user-attachments/assets/90ffce4f-462b-4476-832d-14868fce2aed)

<br>

<p align="justify">
  De entre todos los resultados obtenidos, el único que nos lleva a la solución es <b>admin</b>. Esto quiere decir, que debemos utilizar la siguiente URL.
</p>

```
http://cybersec.42madrid.com:3318/admin/
```

<br>

<p align="justify">
  Al entrar, nos encontramos lo siguiente.
</p>

![image](https://github.com/user-attachments/assets/2a8b486c-34c6-4694-82f4-6e17f6672795)

<br>

<p align="justify">
  Hemos encontrado el archivo, si lo abrimos, encontramos la solución del ejercicio.
</p>

```
42BCN{m1ghtN33dT08ru73f0rc350m3t1m3s;)}
```

<br>

---

### ex02
<p align="justify">
  En este ejercicio, debemos entrar en el siguiente enlace.
</p>

```
http://cybersec.42madrid.com:3319/
```

<br>

<p align="justify">
  Al entrar, nos encontramos lo siguiente.
</p>

![image](https://github.com/user-attachments/assets/830aa8a2-292f-43d1-8f1a-eb2a0176d76c)

<br>

<p align="justify">
  Para encontrar el archivo, debemos utilizar un <i>path transversal</i>. Esto quiere decir, que es tan fácil como poner lo siguiente en el buscador que nos proporcionan.
</p>

![image](https://github.com/user-attachments/assets/e51ad247-c8f3-4c98-b41d-9df104a69bfe)

<br>

<p align="justify">
  Al hacerlo, se nos mostrará la solución.
</p>

```
42BCN{p47h7r4v3rs4l1s7h3w4y}
```

<br>

---

### ex03
<p align="justify">
  Para finalizar, debemos entrar en el siguiente enlace.
</p>

```
http://cybersec.42madrid.com:3320/
```

<br>

<p align="justify">
  Al entrar, nos encontramos lo siguiente.
</p>

![image](https://github.com/user-attachments/assets/46bc9d3f-f9df-4d6f-8dd0-740a7e9cbb86)

<br>

<p align="justify">
  Para encontrar el archivo, debemos utilizar una <i>inyección SQL</i>. Esto se puede llevar a cabo de diferentes maneras. Sin embargo, la forma más sencilla se realiza escribiendo lo siguiente (con un espacio final, después de <b>--</b>).
</p>

![image](https://github.com/user-attachments/assets/e9ae3e38-9c13-46e1-92ed-e0d40169af03)

<br>

<p align="justify">
  Al introducirlo, se nos mostrará la solución.
</p>

```
42BCN{welcomeHackerto42}
```
