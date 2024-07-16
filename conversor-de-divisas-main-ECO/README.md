# 💶💷 Conversor de Divisas 💵💴 
![Badge en Desarollo](https://img.shields.io/badge/STATUS-FINALIZADO-violet)
<img align="right" alt="License MIT" src="https://img.shields.io/badge/LICENSE-MIT-green" /> <br/><br/>
<img alt="html5" src="https://img.shields.io/badge/-HTML5-E34F26?style=flat-square&logo=html5&logoColor=white" />
<img alt="css3" src="https://img.shields.io/badge/-CSS3-1572B6?style=flat-square&logo=css3&logoColor=white" />
<img alt="javascript" src="https://img.shields.io/badge/-JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black" />
<br/><br/>
[![Imagen del conversor de divisas](https://github.com/CrisCorreaS/conversor-de-divisas/blob/main/img/visualizaci%C3%B3n/conversor-vista.png)](https://criscorreas.github.io/conversor-de-divisas/)

Este conversor de divisas online ha sido creado por **[Cristina Correa](https://www.linkedin.com/in/cristina-correa-segade/)**

## 👀 Vista Previa

### ➡️ **Demo desplegada en GitHub Pages:** **[Haz click aquí](https://criscorreas.github.io/conversor-de-divisas/)**

#### Vista del conversor de divisas
![Vista previa del conversor de divisas](https://github.com/CrisCorreaS/conversor-de-divisas/blob/main/img/visualizaci%C3%B3n/conversor-vista.png)

### Funcionalidades:
 1️⃣ **Validación del importe**:
  - Valida que se haya introducido un importe antes de hacer la conversión. Si no es así aparece un mensaje de aviso de error.
    
 ![Vista previa de las funcionalidades del conversor](https://github.com/CrisCorreaS/conversor-de-divisas/blob/main/video/feature1.gif)

 2️⃣ **Conversión de divisas con información**:
  - Permite a los usuarios convertir euros, dólares estadounidenses, canadienses y australianos, libras y yenes. Además, da información sobre las equivalencias de las monedas en tiempo real.
    
 ![Vista previa de las funcionalidades del conversor](https://github.com/CrisCorreaS/conversor-de-divisas/blob/main/video/feature2.gif)

3️⃣ **Conversión inversa instantánea**:
 - En un solo click, puedes hacer la conversión contraria sin ningún problema.
   
 ![Vista previa de las funcionalidades del conversor](https://github.com/CrisCorreaS/conversor-de-divisas/blob/main/video/feature3.gif)

## 🌱 Características

- **Interfaz**: Diseño sencillo y adaptable, con una estética monocromática que garantiza una experiencia visual uniforme en cualquier dispositivo.
- **Conversión de Divisas**: Permite al usuario convertir entre seis divisas populares en tiempo real: euros (EUR), dólares estadounidenses (USD), dólares canadienses (CAD), dólares australianos (AUD), yenes (JPY) y libras esterlinas (GBP).
- **Interactividad**: Facilita al usuario la conversión bidireccional entre cualquier par de divisas seleccionado con un simple clic.
- **Actualización Automática**: Las tasas de cambio se actualizan automáticamente a partir de la API Open Source, garantizando la precisión y la actualización en tiempo real de las conversiones.
- **Conexión a una API Open Source**: Conexión con el objeto XMLHttpRequest a una [API Open Source del Banco Nacional de Polonia](https://api.nbp.pl/) que devuelve datos en formato xml.
 
## 🛠️ Tecnologías Utilizadas

- HTML
- CSS
- JavaScript
- [API Open Source](https://api.nbp.pl/api/exchangerates/tables/c/?format=xml)

## 🤖 API
- Al acceder a la [API del Banco Nacional de Polonia (NBP)](https://api.nbp.pl/), obtenemos información sobre el mercado de divisas y otras tasas de cambio gracias a esta institución financiera. La API está diseñada para proporcionar información sobre las tasas de cambio actuales. La respuesta está en formato XML pero también se puede configurar para devolver un objeto JSON, en mi caso he elegido utilizar el formato XML porque era lo que se me pedía en el ejercicio. Un ejemplo de la llamada a la API sería haciendo "https://api.nbp.pl/api/exchangerates/tables/c/?format=xml" lo cual nos devuelve:
 ```
<ArrayOfExchangeRatesTable xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance">
   <ExchangeRatesTable>
      <Table>C</Table>
      <No>038/C/NBP/2024</No>
      <TradingDate>2024-02-21</TradingDate>
      <EffectiveDate>2024-02-22</EffectiveDate>
      <Rates>
         <Rate>
           <Currency>dolar amerykański</Currency>
           <Code>USD</Code>
           <Bid>3.9589</Bid>
           <Ask>4.0389</Ask>
         </Rate>
         <Rate>
           <Currency>dolar australijski</Currency>
           <Code>AUD</Code>
           <Bid>2.5937</Bid>
           <Ask>2.6461</Ask>
         </Rate>
         ...
      </Rates>
   </ExchangeRatesTable>
</ArrayOfExchangeRatesTable>
 ```
> [!WARNING]
> Al ser una API del NBP, la información está en polaco y las tags en inglés. En general no nos afecta para nada excepto para el nombre de la divisa.

## 🔎💡 Información
> [!IMPORTANT]
> - Este es un proyecto para principiantes. No se requieren conocimientos avanzados de HTML, CSS o JavaScript, pero sí saber cómo hacer conexiones a apis con el objeto XMLHttpRequest.
> - Está desarrollado utilizando JavaScript Vanilla, así que no se utiliza ningún framework. Sin embargo, si estás buscando un poco más de desafío, ¡siéntete libre de explorar la posibilidad de integrar un framework!
> - **Nivel de dificultad del proyecto:** 🔴⭕⭕⭕⭕⭕⭕⭕⭕⭕ (1 sobre 10)

> [!TIP]
> A la hora de desarrollar el proyecto, te pueden venir bien los siguientes recursos:
> - [API de Obtención de Divisas](https://api.nbp.pl/)
> - CSS
>    - [Manz.Dev Lenguaje CSS](https://lenguajecss.com/css/)
> - JavaScript:
>    - [Manz.Dev Lenguaje Javascript](https://lenguajejs.com/javascript/)
>    - [JavaScript MDN Documentation](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
>    - [XHR: XMLHttpRequest - Manz](https://lenguajejs.com/javascript/peticiones-http/xhr/)
> - Font Awesome
>    - [Font Awesome Get Started](https://fontawesome.com/docs/web/setup/get-started)
>    - [Font Awesome Documentation](https://fontawesome.com/v5/docs/web/reference-icons/)

## 📓 Cómo Usar

1. Descarga o clona este repositorio en tu máquina local.
2. Abre el archivo `index.html` en tu navegador web.

¡Y eso es todo! Ahora cualquier persona puede usar un conversor de divisas desde un dispositivo.

## ✨ Contribuciones

¡Las contribuciones son bienvenidas! Si deseas mejorar el conversor de divisas existente, como agregar más contenido o mejorar el diseño, no dudes en enviar tus pull requests. También puedes sugerir nuevas funcionalidades o brindar retroalimentación para hacer que este proyecto sea aún mejor.

## 🎯 Propósito del Proyecto

Este proyecto forma parte de una tarea de la asignatura de "Desarrollo Web en Entorno Cliente" y tiene como objetivo principal el aprendizaje de tecnologías para mejorar en el plano del desarrollo. Es un proyecto que está inspirado en el [conversor de divisas de xe.com](https://www.xe.com/es/currencyconverter/)
