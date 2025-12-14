[index.html](https://github.com/user-attachments/files/24151213/index.html)
<!doctype html>
<html lang="es">
<head>
    <meta charset="utf-8" />
    <meta name="viewport" content="width=device-width,initial-scale=1" />
    <title>Semana 3 — Desarrollo de Aplicaciones</title>
    <style>
        :root{font-family:system-ui,-apple-system,Segoe UI,Roboto,"Helvetica Neue",Arial}
        body{margin:0;padding:2rem;background:#f7f9fc;color:#0b1a2b}
        header{display:flex;justify-content:space-between;align-items:center;margin-bottom:1.5rem}
        h1{font-size:1.25rem;margin:0}
        nav a{margin-left:1rem;color:#0366d6;text-decoration:none}
        main{background:#fff;border-radius:8px;padding:1.25rem;box-shadow:0 1px 2px rgba(11,26,43,.06)}
        .grid{display:grid;grid-template-columns:1fr;gap:.75rem}
        footer{margin-top:1rem;font-size:.85rem;color:#556}
        @media(min-width:700px){.grid{grid-template-columns:1fr 320px}}
    </style>
</head>
<body>
    <header>
        <h1>Semana 3 — Desarrollo de Aplicaciones</h1>
        <nav>
            <a href="#">Inicio</a>
            <a href="#">Ejercicios</a>
            <a href="#">Recursos</a>
        </nav>
    </header>

    <main>
        <div class="grid">
            <section>
                <h2>Instrucciones</h2>
                <p>Este archivo sirve como punto de partida para los ejercicios de la semana 3. Edita el contenido y guarda los cambios.</p>

                <h3>Ejemplo interactivo</h3>
                <p>
                    Introduce tu nombre y pulsa el botón:
                </p>
                <label>
                    Nombre:
                    <input id="name" type="text" placeholder="Tu nombre" />
                </label>
                <button id="greet">Saludar</button>
                <p id="message" aria-live="polite"></p>
            </section>

            <aside>
                <h3>Atajos</h3>
                <ul>
                    <li>Ctrl/Cmd + S — Guardar</li>
                    <li>Ctrl/Cmd + F — Buscar</li>
                    <li>F12 — Abrir DevTools</li>
                </ul>
            </aside>
        </div>
    </main>

    <footer>
        Archivo: /c:/Users/Alejandro Heredia/Desktop/augusto/cuarto semestre/desarroll deaplicaciones/SEMANA3/INDEX.HTML
    </footer>

    <script>
        document.getElementById('greet').addEventListener('click', () => {
            const name = document.getElementById('name').value.trim();
            const msg = name ? `Hola, ${name}! Bienvenido/a.` : 'Hola! Escribe tu nombre arriba.';
            document.getElementById('message').textContent = msg;
        });
    </script>
</body>
</html>
