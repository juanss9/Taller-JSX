# Taller-JSX

Ejercicio 1

<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8">
    <meta name="author" content="Juan Pablo Sepúlveda Salinas">
    <meta name="description" content="Ejercicios JSX">
    <title></title>
  </head>
  <body>
    <div id="root">
      <!--Render code React-js-->
    </div>

    <!-- Cargar React. -->
    <!-- Nota: cuando se despliegue, reemplazar "development.js" con "production.min.js". -->
    <script src="https://unpkg.com/react@16/umd/react.development.js"></script>
    <script src="https://unpkg.com/react-dom@16/umd/react-dom.development.js"></script>
    <script src="https://unpkg.com/babel-standalone@6/babel.min.js"></script>
    <!-- Cargamos nuestro componente de React. -->
    <script type="text/babel">
// Ejercicio 1
const data = {
            title_1: "Plato de la semana",
            title_2: "Berenjenas fritas",
            paragraph_1: "Comensales: 4 personas",
            paragraph_2: "Tiempo de preparación: 10 minutos",
            paragraph_3: "Tiempo de cocción: 12 minutos",
            title_3: "Ingredientes:",
            line_1: "4 Berenjenas.",
            line_2: "Sal.",
            line_3: "Pimienta.",
            line_4: "4 cuhcaradas de harina y aceite.",
            title_4: "Preparación",
            line_5: "Lavar las berenjenas,",
            line_6: "Cortarlas en rodajas.",
            line_7: "Espolvorearlas con sal.",
            line_8: "Dejar que suelten el agua durante 30 minutos.",
            line_9: "Enharinarlas, ponerlas a freir durante 5 minutos en aceite bien caliente.",


         } 


const element = (
        <div>
            <h1>{data.title_1}</h1>
            <h2>{data.title_2}</h2>
            <p>{data.paragraph_1}</p>
            <p>{data.paragraph_2}</p>
            <p>{data.paragraph_3}</p>
            <h3>{data.title_3}</h3>
            <p>{data.line_1}<br/>
            {data.line_2} <br/>
            {data.line_3}<br/>
            {data.line_4}</p>
            <h3>{data.title_4}</h3>
            <p>{data.line_5}<br/>
            {data.line_6}<br/>
            {data.line_7}<br/>
            {data.line_8}</p>

         </div>
        );


        // Renderiamos o pintamos
        ReactDOM.render(
            element,
            document.getElementById('root')
        );
    </script>
  </body>
</html>

Ejercicio 2

<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8">
    <meta name="author" content="Juan Pablo Sepúlveda Salinas">
    <meta name="description" content="Ejercicios JSX">
    <title></title>
  </head>
  <body>
    <div id="root">
      <!--Render code React-js-->
    </div>

    <!-- Cargar React. -->
    <!-- Nota: cuando se despliegue, reemplazar "development.js" con "production.min.js". -->
    <script src="https://unpkg.com/react@16/umd/react.development.js"></script>
    <script src="https://unpkg.com/react-dom@16/umd/react-dom.development.js"></script>
    <script src="https://unpkg.com/babel-standalone@6/babel.min.js"></script>
    <!-- Cargamos nuestro componente de React. -->
    <script type="text/babel">

// Ejercicio 2
const data = {
            title_1: "Página inicial de Juan Tuesta",
            title_2: "Enlaces favoritos:",
            paragraph_1: "Bienvenido a mi página personal. Soy un alumno de la Universidad de Deusto y esta es mi página inicial, con la lista de mis enlaces favoritos y otra información de interés",
            paragraph_2: "Internet",
            paragraph_3: "Google",
            paragraph_4: "Aldea global",
            paragraph_5: "Manual de HTML",
            paragraph_6: "Juan Tuesta, Universidad de Deusto, marzo 2002.",
        }
        const titulo_x = <h1>{data.title_1}</h1>;
        const subtitulo_x = <h2>{data.title_2}</h2>;
        const parrafo_x = <p>{data.paragraph_1}</p>;
        const parrafo_2x = <p>{data.paragraph_2}</p>;
        const parrafo_3x = <p>{data.paragraph_3}</p>;
        const parrafo_4x = <p>{data.paragraph_4}</p>;
        const parrafo_5x = <p>{data.paragraph_5}</p>;
        const parrafo_6x = <p class="p1">{data.paragraph_6}</p>;

        const element = (
            <div>
                {titulo_x}
                {parrafo_x}
                {subtitulo_x}
                <ol>
                    <li>{parrafo_2x}</li>
                    <li>{parrafo_3x}</li>
                    <li>{parrafo_4x}</li>
                    <li>{parrafo_5x}</li>
                </ol>
                {parrafo_6x}
            </div>
        );

        // Renderiamos o pintamos
        ReactDOM.render(
            element,
            document.getElementById('root')
        );
    </script>
</body>

</html>

Ejercicio 3

<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8">
    <meta name="author" content="Juan Pablo Sepúlveda Salinas">
    <meta name="description" content="Ejercicios JSX">
    <title></title>
  </head>
  <body>
    <div id="root">
      <!--Render code React-js-->
    </div>

    <!-- Cargar React. -->
    <!-- Nota: cuando se despliegue, reemplazar "development.js" con "production.min.js". -->
    <script src="https://unpkg.com/react@16/umd/react.development.js"></script>
    <script src="https://unpkg.com/react-dom@16/umd/react-dom.development.js"></script>
    <script src="https://unpkg.com/babel-standalone@6/babel.min.js"></script>
    <!-- Cargamos nuestro componente de React. -->
    <script type="text/babel">
// nota cada codigo que veas documentado de aca para abajo
// seran diferentes formas de realizarlo con jsx los coloco para
// que podamos probar y mirar diferentes formas de como podriamos realizarlos
// los 12 ejercicios

// Ejercicio 3
const data = {
            title_1: "Página inicial de Juan Tuesta",
            title_2: "Enlaces favoritos:",
            paragraph_1: "Bienvenido a mi página personal. Soy un alumno de la Universidad de Deusto y esta es mi página inicial, con la lista de mis enlaces favoritos y otra información de interés",
            paragraph_2: "Internet",
            paragraph_3: "Google",
            paragraph_4: "Aldea global",
            paragraph_5: "Manual de HTML",
            paragraph_6: "Juan Tuesta, Universidad de Deusto, marzo 2002.",
        }
        const titulox = <h1>{data.title_1}</h1>;
        const subtitulox = <h2>{data.title_2}</h2>;
        const parrafox = <p>{data.paragraph_1}</p>;
        const parrafo2x = <p>{data.paragraph_2}</p>;
        const parrafo3x = <p>{data.paragraph_3}</p>;
        const parrafo4x = <p>{data.paragraph_4}</p>;
        const parrafo5x = <p>{data.paragraph_5}</p>;
        const parrafo6x = <p class="p1">{data.paragraph_6}</p>;

        const element = (
            <div>
                {titulox}
                {parrafox}
                {subtitulox}
                <ol>
                    <li>{parrafo2x}</li>
                    <li><a href="taller8.html">{parrafo3x}</a></li>
                    <li>{parrafo4x}</li>
                    <li><a href="taller8.html">{parrafo5x}</a></li>
                </ol>
                {parrafo6x}
            </div>
        );

        // Renderiamos o pintamos
        ReactDOM.render(
            element,
            document.getElementById('root')
        );
    </script>
</body>

</html>

Ejercicio 4

<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8">
    <meta name="author" content="Juan Pablo Sepúlveda Salinas">
    <meta name="description" content="Ejercicios JSX">
    <title></title>
  </head>
  <body>
    <div id="root">
      <!--Render code React-js-->
    </div>

    <!-- Cargar React. -->
    <!-- Nota: cuando se despliegue, reemplazar "development.js" con "production.min.js". -->
    <script src="https://unpkg.com/react@16/umd/react.development.js"></script>
    <script src="https://unpkg.com/react-dom@16/umd/react-dom.development.js"></script>
    <script src="https://unpkg.com/babel-standalone@6/babel.min.js"></script>
    <!-- Cargamos nuestro componente de React. -->
    <script type="text/babel">
// nota cada codigo que veas documentado de aca para abajo
// seran diferentes formas de realizarlo con jsx los coloco para
// que podamos probar y mirar diferentes formas de como podriamos realizarlos
// los 12 ejercicios

// Ejercicio 4
const data = {
            title_1: "Página inicial de Juan Tuesta",
            title_2: "Enlaces favoritos:",
            paragraph_1: "Bienvenido a mi página personal. Soy un alumno de la Universidad de Deusto y esta es mi página inicial, con la lista de mis enlaces favoritos y otra información de interés",
            paragraph_2: "Páginas personales",
            paragraph_3: "Páginas de referencia",
            paragraph_4: "Portales",
            paragraph_5: "Medios de comunicación",
            paragraph_6: "Charkes F.Golfarb",
            paragraph_7: "Lou Burnard",
            paragraph_8: "Tim Berners-Lee",
            paragraph_9: "Juan Tuesta, Universidad de Deusto, marzo 2002.",
        }
        const titulox1 = <h1>{data.title_1}</h1>;
        const subtitulox1 = <h2>{data.title_2}</h2>;
        const parrafox1 = <p>{data.paragraph_1}</p>;
        const parrafox2 = <p>{data.paragraph_2}</p>;
        const parrafox3 = <p>{data.paragraph_3}</p>;
        const parrafox4 = <p>{data.paragraph_4}</p>;
        const parrafox5 = <p>{data.paragraph_5}</p>;
        const parrafox6 = <p>{data.paragraph_6}</p>;
        const parrafox7 = <p>{data.paragraph_7}</p>;
        const parrafox8 = <p>{data.paragraph_8}</p>;
        const parrafox9 = <p class="p1">{data.paragraph_9}</p>;

        const element = (
            <div>
                {titulox1}
                {parrafox1}
                {subtitulox1}
                <ol>
                    <li>{parrafox2}</li>
                    <ul>
                        <li>{parrafox6}</li>
                        <li>{parrafox7}</li>
                        <li>{parrafox8}</li>
                    </ul>
                    <li>{parrafox3}</li>
                    <li>{parrafox4}</li>
                    <li>{parrafox5}</li>
                </ol>
                {parrafox9}
            </div>
        );

        // Renderiamos o pintamos
        ReactDOM.render(
            element,
            document.getElementById('root')
        );
    </script>
</body>

</html>

Ejercicio 5

<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8">
    <meta name="author" content="Juan Pablo Sepúlveda Salinas">
    <meta name="description" content="Ejercicios JSX">
    <title></title>
  </head>
  <body>
    <div id="root">
      <!--Render code React-js-->
    </div>

    <!-- Cargar React. -->
    <!-- Nota: cuando se despliegue, reemplazar "development.js" con "production.min.js". -->
    <script src="https://unpkg.com/react@16/umd/react.development.js"></script>
    <script src="https://unpkg.com/react-dom@16/umd/react-dom.development.js"></script>
    <script src="https://unpkg.com/babel-standalone@6/babel.min.js"></script>
    <!-- Cargamos nuestro componente de React. -->
    <script type="text/babel">
// nota cada codigo que veas documentado de aca para abajo
// seran diferentes formas de realizarlo con jsx los coloco para
// que podamos probar y mirar diferentes formas de como podriamos realizarlos
// los 12 ejercicios

// Ejercicio 5
const data = {
            title_1: "Página inicial de Juan Tuesta",
            title_2: "Enlaces favoritos",
            title_3: "Páginas personales",
            title_4: "Páginas de referencia",
            title_5: "Portales",
            title_6: "Publicaciones",
            paragraph_1: "Bienvenido a mi página personal. Soy un alumno de la Universidad de Deusto y esta es mi página inicial, con la lista de mis enlaces favoritos y otra información de interés",
            paragraph_2: "Juan Tuesta, Universidad de Deusto, marzo 2002.",
            paragraph_3: "Páginas personales",
            paragraph_4: "Páginas de referencia",
            paragraph_5: "Portales",
            paragraph_6: "Publicaciones",
            paragraph_7: "Documentalistas",
            paragraph_8: "Historiadores",
            paragraph_9: "Lingüistas",
            paragraph_10: "Traductores",
            paragraph_11: "Bibliotecas universitarias",
            paragraph_12: "Centros de documentación",
            paragraph_13: "Museos de arte contemporáneo",
            paragraph_14: "Medios de comunicación",
            paragraph_15: "Inicia",
            paragraph_16: "Telépolis",
            paragraph_17: "Ciudades",
            paragraph_18: "Terra",
            paragraph_19: "Ciberp@ís",
            paragraph_20: "Diario Tecnologías de la Información",
            paragraph_21: "The Standard",
            paragraph_22: "Infoworld",
            paragraph_23: "Wired",
            paragraph_24: "Charkes F.Golfarb",
            paragraph_25: "Lou Burnard",
            paragraph_26: "Tim Berners-Lee",
        }
        const titulo1 = <h1>{data.title_1}</h1>;
        const subtitulo1 = <h2>{data.title_2}</h2>;
        const subtitulo2 = <h2>{data.title_3}</h2>;
        const subtitulo3 = <h2>{data.title_4}</h2>;
        const subtitulo4 = <h2>{data.title_5}</h2>;
        const subtitulo5 = <h2>{data.title_6}</h2>;
        const parrafo1 = <p>{data.paragraph_1}</p>;
        const parrafo2 = <p class="p1">{data.paragraph_2}</p>;
        const parrafo3 = <p>{data.paragraph_3}</p>;
        const parrafo4 = <p>{data.paragraph_4}</p>;
        const parrafo5 = <p>{data.paragraph_5}</p>;
        const parrafo6 = <p>{data.paragraph_6}</p>;
        const parrafo7 = <p>{data.paragraph_7}</p>;
        const parrafo8 = <p>{data.paragraph_8}</p>;
        const parrafo9 = <p>{data.paragraph_9}</p>;
        const parrafo10 = <p>{data.paragraph_10}</p>;
        const parrafo11 = <p>{data.paragraph_11}</p>;
        const parrafo12 = <p>{data.paragraph_12}</p>;
        const parrafo13 = <p>{data.paragraph_13}</p>;
        const parrafo14 = <p>{data.paragraph_14}</p>;
        const parrafo15 = <p>{data.paragraph_15}</p>;
        const parrafo16 = <p>{data.paragraph_16}</p>;
        const parrafo17 = <p>{data.paragraph_17}</p>;
        const parrafo18 = <p>{data.paragraph_18}</p>;
        const parrafo19 = <p>{data.paragraph_19}</p>;
        const parrafo20 = <p>{data.paragraph_20}</p>;
        const parrafo21 = <p>{data.paragraph_21}</p>;
        const parrafo22 = <p>{data.paragraph_22}</p>;
        const parrafo23 = <p>{data.paragraph_23}</p>;
        const parrafo24 = <p>{data.paragraph_24}</p>;
        const parrafo25 = <p>{data.paragraph_25}</p>;
        const parrafo26 = <p>{data.paragraph_26}</p>;

        const element = (
            <div>
                {titulo1}
                {parrafo1}
                {subtitulo1}
                <ol>
                    <li><a href="ejercicio5.html">{parrafo3}</a></li>
                    <li>{parrafo4}</li>
                    <li>{parrafo5}</li>
                    <li>{parrafo6}</li>
                </ol>
                <hr></hr>

                {subtitulo2}
                <ol>
                    <li>{parrafo7}</li>
                    <ul>
                        <li>{parrafo24}</li>
                        <li>{parrafo25}</li>
                        <li>{parrafo26}</li>
                    </ul>
                    <li>{parrafo8}</li>
                    <li>{parrafo9}</li>
                    <li>{parrafo10}</li>
                </ol>
                <hr></hr>

                {subtitulo3}
                <ol>
                    <li>{parrafo11}</li>
                    <li>{parrafo12}</li>
                    <li>{parrafo13}</li>
                    <li>{parrafo14}</li>
                </ol>
                <hr></hr>

                {subtitulo4}
                <ol>
                    <li>{parrafo15}</li>
                    <li>{parrafo16}</li>
                    <li>{parrafo17}</li>
                    <li>{parrafo18}</li>
                </ol>
                <hr></hr>

                {subtitulo5}
                <ol>
                    <li>{parrafo19}</li>
                    <li>{parrafo20}</li>
                    <li>{parrafo21}</li>
                    <li>{parrafo22}</li>
                    <li>{parrafo23}</li>
                </ol>
                <hr></hr>

                {parrafo2}

            </div>
        );

        // Renderiamos o pintamos
        ReactDOM.render(
            element,
            document.getElementById('root')
        );
    </script>
</body>

</html>

Ejercicio 6

<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8">
    <meta name="author" content="Juan Pablo Sepúlveda Salinas">
    <meta name="description" content="Ejercicios JSX">
    <title></title>
  </head>
  <body>
    <div id="root">
      <!--Render code React-js-->
    </div>

    <!-- Cargar React. -->
    <!-- Nota: cuando se despliegue, reemplazar "development.js" con "production.min.js". -->
    <script src="https://unpkg.com/react@16/umd/react.development.js"></script>
    <script src="https://unpkg.com/react-dom@16/umd/react-dom.development.js"></script>
    <script src="https://unpkg.com/babel-standalone@6/babel.min.js"></script>
    <!-- Cargamos nuestro componente de React. -->
    <script type="text/babel">

// Ejercicio 6

const data = {
            title_1: "Next University",
            title_2: "Programas de Tecnología",
            title_3: "Desarrollador Web",
            title_4: "Android",
            title_5: "Programa de Negocio",
            title_6: "Mercadeo Digital",

        }

        const element = (
            <div>
                <h1>El Noticiero {data.title_1}</h1>
                <h2>{data.title_2}</h2>
                <h3>{data.title_3}</h3>
                <p><b>{data.title_1}</b> lanza su programa de formación <b>"{data.title_3}"</b> con la facilidad de cpacitar a personas en las tendencias actuales
                    sobre tecnologias, en caso de desarrollo web, se basa temas relacionados con implementacion de Front-End con tecnologias y Frameworks, tales
                    como: <i>HTML, CSS, JavaScript, Bootstrap, entre otros.</i></p>
                <h3>{data.title_4}</h3>
                <p>En <b>{data.line_1}</b> te ofrecemos el programa <b>{data.title_4}</b> que te da las herramientas necesarias para diseñar e implementar
                    aplicaciones {data.title_4} para dispositivos móviles, partiendo de un conocimiento basico de <i>Java</i>, utilizando el entorno de desarrollo de
                    <i>{data.title_4} Studio</i>. Aprenderás los aspectos fundamentales para crear aplicaiones {data.title_4} interactivas, dinámicas y exitosas
                    utilizando técnicas para el manejo de los recursos, datros, segundos planos, localizacion, sensores, animaciones, gráficos, multimedia y monetización.</p>
                <h2>{data.title_5}</h2>
                <h3>{data.title_6}</h3>
                <p><b><i>{data.title_1}</i></b> coloca a tu disposición el programa de <b>"{data.title_6}"</b>. Sabias que...{data.title_6} o Digital Marketing
                    es mucho mas que hacer y publicar anuncios. Se trata del consumidor y la estrategia de negocio.
                    Estos son los puntos de partida para que cualquier acción de {data.title_6} <i>sea exitosa y optimice la inversión.</i>
                    Este certificado, es un programa completo y práctico que permite entender al consumidor, la industria, la competencia y los retos del negocio propio;
                    para crear e implementar estrategias a la medida, en diferentes plataformas y medios digitales. Por supuesto, monitoreando los resultados para tomar
                    decisiones en tiempo real.</p>
            </div>
        );


        // Renderiamos o pintamos
        ReactDOM.render(
            element,
            document.getElementById('root')
        );
    </script>
</body>

</html>

Ejercicio 7

<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8">
    <meta name="author" content="Juan Pablo Sepúlveda Salinas">
    <meta name="description" content="Ejercicios JSX">
    <title></title>
  </head>
  <body>
    <div id="root">
      <!--Render code React-js-->
    </div>

    <!-- Cargar React. -->
    <!-- Nota: cuando se despliegue, reemplazar "development.js" con "production.min.js". -->
    <script src="https://unpkg.com/react@16/umd/react.development.js"></script>
    <script src="https://unpkg.com/react-dom@16/umd/react-dom.development.js"></script>
    <script src="https://unpkg.com/babel-standalone@6/babel.min.js"></script>
    <!-- Cargamos nuestro componente de React. -->
    <script type="text/babel">

// Ejercicio 7
const data = {
            title_1: "Destinos Turísticos",
            pais_1:
                <ol>
                    <li><i>Buenos Aires</i></li>
                    <li><i>Bariloche</i></li>
                </ol>,
            pais_2:
                <ol>
                    <li><i>Rio de Janeiro</i></li>
                    <li><i>Brasilia</i></li>
                </ol>,
            pais_3:
                <ol>
                    <li><i>Santiago</i></li>
                    <li><i>Valparaiso</i></li>
                </ol>,
            pais_4:
                <ol>
                    <li><i>Bogotá</i></li>
                    <li><i>Cartagena de Indias</i></li>
                </ol>,
            pais_5:
                <ol>
                    <li><i>New York</i></li>
                    <li><i>San Francisco</i></li>
                </ol>,
            pais_6:
                <ol>
                    <li><i>Cancún</i></li>
                    <li><i>Acapulco</i></li>
                </ol>,
            pais_7:
                <ol>
                    <li><i>Lima</i></li>
                    <li><i>Cuzco</i></li>
                </ol>,
            pais_8:
                <ol>
                    <li><i>Margarita</i></li>
                    <li><i>Mérida</i></li>
                </ol>,
        }

        const element = (
            <div>
                <h1>{data.title_1}</h1>
                <ol>
                    <li><b>Argentina</b>
                        {data.pais_1}</li>
                    <li><b>Brasil</b>
                        {data.pais_2}</li>
                    <li><b>Chile</b>
                        {data.pais_3}</li>
                    <li><b>Colombia</b>
                        {data.pais_4}</li>
                    <li><b>Estados Unidos</b>
                        {data.pais_5}</li>
                    <li><b>México</b>
                        {data.pais_6}</li>
                    <li><b>Perú</b>
                        {data.pais_7}</li>
                    <li><b>Venezuela</b>
                        {data.pais_8}</li>
                </ol>

            </div>
        );


        // Renderiamos o pintamos
        ReactDOM.render(
            element,
            document.getElementById('root')
        );
    </script>
</body>

</html>

Ejercicio 8

<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8">
    <meta name="author" content="Juan Pablo Sepúlveda Salinas">
    <meta name="description" content="Ejercicios JSX">
    <title></title>
  </head>
  <body>
    <div id="root">
      <!--Render code React-js-->
    </div>

    <!-- Cargar React. -->
    <!-- Nota: cuando se despliegue, reemplazar "development.js" con "production.min.js". -->
    <script src="https://unpkg.com/react@16/umd/react.development.js"></script>
    <script src="https://unpkg.com/react-dom@16/umd/react-dom.development.js"></script>
    <script src="https://unpkg.com/babel-standalone@6/babel.min.js"></script>
    <!-- Cargamos nuestro componente de React. -->
    <script type="text/babel">
    
// Ejercicio 8
const data = {
            titulo: "Tu concierto",
            parrafo: "Bienvenido a este blog de conciertos",
        }

        const titulito = <h1 class="title">{data.titulo}</h1>;
        const parrafato = <p>{data.parrafo}</p>;


        const element = (
            <div>
                <img src="./elements/personas-celebrando.jpg" width="150" align="left" />
                {titulito}
                <br /><br /><br />
                {parrafato}
                <img src="./elements/concierto.jpg" />
            </div>
        );

        // Renderiamos o pintamos
        ReactDOM.render(
            element,
            document.getElementById('root')
        );
    </script>
</body>

</html>

Ejercicio 9

<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8">
    <meta name="author" content="Juan Pablo Sepúlveda Salinas">
    <meta name="description" content="Ejercicios JSX">
    <title></title>
  </head>
  <body>
    <div id="root">
      <!--Render code React-js-->
    </div>

    <!-- Cargar React. -->
    <!-- Nota: cuando se despliegue, reemplazar "development.js" con "production.min.js". -->
    <script src="https://unpkg.com/react@16/umd/react.development.js"></script>
    <script src="https://unpkg.com/react-dom@16/umd/react-dom.development.js"></script>
    <script src="https://unpkg.com/babel-standalone@6/babel.min.js"></script>
    <!-- Cargamos nuestro componente de React. -->
    <script type="text/babel">
    
// Ejercicio 10
const datos = {

titulo1: "Recetas.com",
img: "./elements/chef.jpg",
menu1: "Recetas Principales   ",
barra: "|",
menu2: " Postres latinos",
parrafo1: "Bienvenidos a nuestro sitio Web sobre gastronomia latina, te invitamos a preparar nuestras recetas",
titulo2: "Nuevas Recetas",
parrafo2: "**Arroz Criollo*",
parrafo3: "Tiempo de preparación: ",
parrafo4: "45 minutos",
parrafo5: "Numero de porciones",
parrafo6: "4",
parrafo7: "Ingredientes",
v1: "Salsa de tomate",
v2: "2 cucharadas de aceite 14gr",
v3: "1 cebolla larga picada 45gr",
v4: "2 dientes de ajo finamente picado 3gr",
v5: "1 pimentón rojo picado en cuadritos 60gr",
v6: "1 taza de arroz blanco 225gr",
v7: "1 taza de maíz desgranado 79gr",
v8: "150gr de pechuga de pollo cocinado y desmechado",
v9: "Sal al gusto",
parrafo8: "Preparación",
v10: "Calentar en una olla el aceite, sofreir la cebolla junto con el ajo, el pimentin por 3 minutos",
v11: "Adicionar el arroz y continua sofriendo para que se dore.",
v12: "Agregar el pollo, el maiz desgranado y las verduras.",
v13: "Mezclar todo, rectificar sal y dejar cocinar hasta que seque.",
v14: "Bajar el fuego, tapar la olla y continuar la cocción por 25 minutos más.",
parrafo9: "Esta rica receta fue proporcionada por Maria Paula.",
}

const element = (
<div>
    <h1> {<img src={datos.img} width="150" />} {datos.titulo1}</h1>
    <h3><a href="">{datos.menu1}</a>  {datos.barra}  <a href=""> {datos.menu2}</a></h3>
    <br />
    <p>{datos.parrafo1}</p>
    <h1>{datos.titulo2}</h1>
    <h2>{datos.parrafo2}</h2>
    <p>{datos.parrafo3} <b>{datos.parrafo4}</b> {datos.parrafo5} <b>{datos.parrafo6}</b> </p>
    <h2>{datos.parrafo7}</h2>
    <ul>
        <li><b>{datos.v1}</b></li>
        <br></br>
        <li><b>{datos.v2}</b></li>
        <br></br>
        <li><b>{datos.v3}</b></li>
        <br></br>
        <li><b>{datos.v4}</b></li>
        <br></br>
        <li><b>{datos.v5}</b></li>
        <br></br>
        <li><b>{datos.v6}</b></li>
        <br></br>
        <li><b>{datos.v7}</b></li>
        <br></br>
        <li><b>{datos.v8}</b></li>
        <br></br>
        <li><b>{datos.v9}</b></li>
    </ul>
    <h2>{datos.parrafo8}</h2>
    <ol>
        <li>{datos.v10}</li>
        <br></br>
        <li>{datos.v11}</li>
        <br></br>
        <li>{datos.v12}</li>
        <br></br>
        <li>{datos.v13}</li>
        <br></br>
        <li>{datos.v14}</li>
    </ol>
    <p>{datos.parrafo9}</p>
</div>
);

// Renderiamos o pintamos
ReactDOM.render(
element,
document.getElementById('root')
);
</script>
</body>

</html>

Ejercicio 10

<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8">
    <meta name="author" content="Juan Pablo Sepúlveda Salinas">
    <meta name="description" content="Ejercicios JSX">
    <title></title>
  </head>
  <body>
    <div id="root">
      <!--Render code React-js-->
    </div>

    <!-- Cargar React. -->
    <!-- Nota: cuando se despliegue, reemplazar "development.js" con "production.min.js". -->
    <script src="https://unpkg.com/react@16/umd/react.development.js"></script>
    <script src="https://unpkg.com/react-dom@16/umd/react-dom.development.js"></script>
    <script src="https://unpkg.com/babel-standalone@6/babel.min.js"></script>
    <!-- Cargamos nuestro componente de React. -->
    <script type="text/babel">
    
// Ejercicio 10
const datos = {

titulo1: "Recetas.com",
img: "./elements/chef.jpg",
menu1: "Recetas Principales   ",
barra: "|",
menu2: " Postres latinos",
parrafo1: "Bienvenidos a nuestro sitio Web sobre gastronomia latina, te invitamos a preparar nuestras recetas",
titulo2: "Nuevas Recetas",
parrafo2: "**Arroz Criollo*",
parrafo3: "Tiempo de preparación: ",
parrafo4: "45 minutos",
parrafo5: "Numero de porciones",
parrafo6: "4",
parrafo7: "Ingredientes",
v1: "Salsa de tomate",
v2: "2 cucharadas de aceite 14gr",
v3: "1 cebolla larga picada 45gr",
v4: "2 dientes de ajo finamente picado 3gr",
v5: "1 pimentón rojo picado en cuadritos 60gr",
v6: "1 taza de arroz blanco 225gr",
v7: "1 taza de maíz desgranado 79gr",
v8: "150gr de pechuga de pollo cocinado y desmechado",
v9: "Sal al gusto",
parrafo8: "Preparación",
v10: "Calentar en una olla el aceite, sofreir la cebolla junto con el ajo, el pimentin por 3 minutos",
v11: "Adicionar el arroz y continua sofriendo para que se dore.",
v12: "Agregar el pollo, el maiz desgranado y las verduras.",
v13: "Mezclar todo, rectificar sal y dejar cocinar hasta que seque.",
v14: "Bajar el fuego, tapar la olla y continuar la cocción por 25 minutos más.",
parrafo9: "Esta rica receta fue proporcionada por Maria Paula.",
}

const element = (
<div>
    <h1> {<img src={datos.img} width="150" />} {datos.titulo1}</h1>
    <h3><a href="">{datos.menu1}</a>  {datos.barra}  <a href=""> {datos.menu2}</a></h3>
    <br />
    <p>{datos.parrafo1}</p>
    <h1>{datos.titulo2}</h1>
    <h2>{datos.parrafo2}</h2>
    <p>{datos.parrafo3} <b>{datos.parrafo4}</b> {datos.parrafo5} <b>{datos.parrafo6}</b> </p>
    <h2>{datos.parrafo7}</h2>
    <ul>
        <li><b>{datos.v1}</b></li>
        <br></br>
        <li><b>{datos.v2}</b></li>
        <br></br>
        <li><b>{datos.v3}</b></li>
        <br></br>
        <li><b>{datos.v4}</b></li>
        <br></br>
        <li><b>{datos.v5}</b></li>
        <br></br>
        <li><b>{datos.v6}</b></li>
        <br></br>
        <li><b>{datos.v7}</b></li>
        <br></br>
        <li><b>{datos.v8}</b></li>
        <br></br>
        <li><b>{datos.v9}</b></li>
    </ul>
    <h2>{datos.parrafo8}</h2>
    <ol>
        <li>{datos.v10}</li>
        <br></br>
        <li>{datos.v11}</li>
        <br></br>
        <li>{datos.v12}</li>
        <br></br>
        <li>{datos.v13}</li>
        <br></br>
        <li>{datos.v14}</li>
    </ol>
    <p>{datos.parrafo9}</p>
</div>
);

// Renderiamos o pintamos
ReactDOM.render(
element,
document.getElementById('root')
);
</script>
</body>

</html>

Ejercicio 11

<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8">
    <meta name="author" content="Juan Pablo Sepúlveda Salinas">
    <meta name="description" content="Ejercicios JSX">
    <title></title>
  </head>
  <body>
    <div id="root">
      <!--Render code React-js-->
    </div>

    <!-- Cargar React. -->
    <!-- Nota: cuando se despliegue, reemplazar "development.js" con "production.min.js". -->
    <script src="https://unpkg.com/react@16/umd/react.development.js"></script>
    <script src="https://unpkg.com/react-dom@16/umd/react-dom.development.js"></script>
    <script src="https://unpkg.com/babel-standalone@6/babel.min.js"></script>
    <!-- Cargamos nuestro componente de React. -->
    <script type="text/babel">

// Ejercicio 11
const data = {

titulo1: "Registro en nuestra tienda",
nombre: "Nombre de usuario:",
email: "Email:",
edad: "Edad:",
genero: "Género:",
recomendado: "Recomendado por:",
comentarios: "Comentarios:",
acepto: "Acepto terminos y condiciones:"

}

const element = (
<div>
    <h1>{data.titulo1}</h1>
    <p>{data.nombre}</p>
    <input type="text" placeholder="Ej: Juan Pablo" ></input>
    <br />
    <p>{data.email}</p>
    <input type="text" placeholder="Ej: jpsepulveda81345@umanizales.edu.com" ></input>
    <br />
    <p>{data.edad}</p>
    <input type="text" placeholder="Ej: 27" ></input>
    <br />
    <p>{data.genero}</p>
    <input type="radio" value="Masculino" name="Genero" /> Masculino
    <br />
    <input type="radio" value="Femenino" name="Genero" /> Femenino
    <br />
    <p>{data.recomendado}</p>
    <select value={data.recomendado}>
        <option value="A">Google</option>
        <option value="B">Amazon</option>
        <option value="C">Facebook</option>
    </select>
    <br />
    <p>{data.comentarios}</p>
    <textarea rows={4} cols={50} type="textarea"
        name="textValue"
    />
    <br />
    <p>{data.acepto}</p>
    <input type="checkbox" />
    <br />
    <input type="submit" value="Registrar" />
</div>
);


// Renderiamos o pintamos
ReactDOM.render(
element,
document.getElementById('root')
);
</script>
</body>

</html>

Ejercicio 12

<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8">
    <meta name="author" content="Juan Pablo Sepúlveda Salinas">
    <meta name="description" content="Ejercicios JSX">
    <title></title>
  </head>
  <body>
    <div id="root">
      <!--Render code React-js-->
    </div>

    <!-- Cargar React. -->
    <!-- Nota: cuando se despliegue, reemplazar "development.js" con "production.min.js". -->
    <script src="https://unpkg.com/react@16/umd/react.development.js"></script>
    <script src="https://unpkg.com/react-dom@16/umd/react-dom.development.js"></script>
    <script src="https://unpkg.com/babel-standalone@6/babel.min.js"></script>
    <!-- Cargamos nuestro componente de React. -->
    <script type="text/babel">

// Ejercicio 12
const data = {

titulo: "Título en encabezado",
descrip: "Descripción del audio",
audio: "./elements/regal-repeat.mp3",
drechos: "Derechos Reservados (Pie)",

}

const element = (
<div>
    <h1>{data.titulo}</h1>
    <p>{data.descrip}</p>
    <br />
    <audio controlsList="nodownload" controls>
        <source src={data.audio} type="audio/mpeg" />
    </audio>
    <br />
    <br />
    <p>{data.drechos}</p>
</div>
);

// Renderiamos o pintamos
ReactDOM.render(
element,
document.getElementById('root')
);
</script>
</body>

</html>

Ejercicio 13

<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8">
    <meta name="author" content="Juan Pablo Sepúlveda Salinas">
    <meta name="description" content="Ejercicios JSX">
    <title></title>
  </head>
  <body>
    <div id="root">
      <!--Render code React-js-->
    </div>

    <!-- Cargar React. -->
    <!-- Nota: cuando se despliegue, reemplazar "development.js" con "production.min.js". -->
    <script src="https://unpkg.com/react@16/umd/react.development.js"></script>
    <script src="https://unpkg.com/react-dom@16/umd/react-dom.development.js"></script>
    <script src="https://unpkg.com/babel-standalone@6/babel.min.js"></script>
    <!-- Cargamos nuestro componente de React. -->
    <script type="text/babel">

// Ejercicio 13

const t1=<h1>Titulo de encabezado</h1>
    const p1=<p>Este es un parrafo</p>
    const video=<iframe width="560" height="315" src="https://www.youtube.com/watch?v=Z8zAKYLZBqc" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
    const p2=<p>Derechos Reservados(pie)</p>

const element=(
    <div>
        {t1}
        {p1}
        {video}
        {p2}
        </div>
)

    ReactDOM.render(element,document.getElementById("root"))
    </script>

</body>
</html>
