---

### Ejercicio colaborativo: "Muro de Principios"

#### Objetivo General

Practicar el flujo colaborativo en Git (ramas, issues, PRs, revisiones) contribuyendo a un sitio web simple que recoja principios de buenas prácticas en desarrollo.

---

### Estructura del Repositorio

* `/index.html` → donde cada coder agregará su principio con un `<h1>`
* `/style.css` → donde cada coder estilizará su `h1` con su `id`
* `README.md` → con instrucciones del flujo de trabajo

---

### Flujo de Trabajo para Cada Coder

1. **Clonar el repositorio**
   ```bash
   git clone https://github.com/Riwi-io-Medellin/muro-colaborativo-html-css.git
   cd muro-colaborativo-html-css
   ```

2. **Crear una rama a partir de `main`**
   ```bash
   git checkout main
   git pull origin main
   git checkout -b feature/coder-N-elemento    # Reemplaza N con tu número de coder
   ```

3. **Editar `index.html` y `style.css`**
   ```bash
   # Edita los archivos con tu editor preferido
   code index.html style.css    # Si usas VS Code
   # O usa el editor que prefieras
   ```

4. **Hacer commit con mensaje claro y referencia al issue**
   ```bash
   git add index.html style.css
   git commit -m "feat: agregar elemento HTML para coder N - closes #N"
   ```

5. **Hacer push a la rama remota**
   ```bash
   git push origin feature/coder-N-elemento
   ```

6. **Crear un Pull Request (PR)**
   ```bash
   # Ve a GitHub y crea el PR desde tu rama a main
   # Título sugerido: "feat: Elemento HTML Coder N"
   # Descripción: Explica brevemente los cambios realizados
   ```

7. **Solicitar revisión a un compañero**
   ```bash
   # En GitHub:
   # 1. Click en 'Reviewers' en el PR
   # 2. Selecciona a un compañero para review
   ```

8. **Esperar aprobación y fusión del PR**
   ```bash
   # Espera los comentarios del reviewer
   # Realiza cambios si son solicitados:
   git add .
   git commit -m "fix: ajustes solicitados en review"
   git push origin feature/coder-N-elemento
   ```

9. **Actualizar `main` local antes de comenzar otra tarea**
   ```bash
   git checkout main
   git pull origin main
   ```

---

### Reglas del Ejercicio

* **No modificar líneas de otros coders**
* **No trabajar sobre `main` directamente**
* **Commits claros y vinculados a issues**
* **Cada coder solo trabaja su ticket**
* **El CSS debe afectar solo su propio `id`**

---