# Comandos para subir el repositorio a GitHub

Descarga y descomprime la carpeta `rojas-post1-u3` que te entregué (contiene `README.md`,
`Informe_Rojas_Rey_Post1_U3.pdf` y la carpeta `capturas/`). Luego, en una terminal, ubícate
dentro de esa carpeta y ejecuta lo siguiente.

## 1. Inicializar y conectar con GitHub

```bash
cd rojas-post1-u3
git init
git remote add origin https://github.com/juandi12334/rojas-post1-u3.git
git branch -M main
```

## 2. Commits de la Parte 1 (mínimo 3)

```bash
git add README.md capturas/CP1_registros.jpeg
git commit -m "Agrega estructura inicial y Checkpoint 1: estado de registros"

git add capturas/CP2_volcado_memoria.png capturas/CP3_ensamblado_desensamblado.png capturas/verificacion/verif_u_ADD_AXBX_paso10.png capturas/verificacion/verif_ensamblado_suma.png
git commit -m "Completa Checkpoint 2 (volcado de memoria) y Checkpoint 3 (ensamblado y desensamblado)"

git add capturas/CP4_memoria_direccionamiento.png README.md
git commit -m "Completa Checkpoint 4 y decisiones tecnicas de la Parte 1 (verificacion no destructiva y direccionamiento)"
```

## 3. Commits de la Parte 2 (mínimo 3)

```bash
git add capturas/CP1_traza_suma.png capturas/verificacion/verif_ensamblado_loop.png
git commit -m "Agrega estructura inicial de la Parte 2"

git add capturas/CP2_traza_loop.png capturas/verificacion/verif_D100L0D_analisis_bytes.png
git commit -m "Completa traza suma (CP1) y traza loop (CP2)"

git add capturas/CP3_traza_dec_jnz.png capturas/verificacion/verif_ensamblado_decjnz.png README.md Informe_Rojas_Rey_Post1_U3.pdf COMANDOS_GIT.md
git commit -m "Completa bucle DEC/JNZ y decisiones tecnicas (CP3)"
```

## 4. Subir todo a GitHub

```bash
git push -u origin main
```

Si te pide iniciar sesión, usa tu usuario de GitHub y, en vez de la contraseña, un
Personal Access Token (GitHub ya no acepta la contraseña normal por línea de comandos).
Si no tienes uno, en GitHub ve a Settings → Developer settings → Personal access tokens →
Generate new token, y úsalo como si fuera la contraseña.

## 5. Verificar

Entra a `https://github.com/juandi12334/rojas-post1-u3` y confirma que aparecen:
- El `README.md` renderizado con las tablas.
- La carpeta `capturas/` con los 7 archivos oficiales.
- El PDF `Informe_Rojas_Rey_Post1_U3.pdf`.
- Al menos 6 commits en el historial.

Cuando esté subido, copia la URL del repositorio y súbela a NPLAD UFPS antes de la fecha límite.
