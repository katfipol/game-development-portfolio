p align="center">
  <a href="https://katfipol.github.io/game-development-portfolio/juegos/myeconomy/">
    <img src="../../assets/capturas/myeconomy.png" alt="Captura de MyEconomy: ciudad financiera con banco, tienda, trabajo, hogar y meta de ahorro" width="100%">
  </a>
</p>

<h1 align="center">MyEconomy: Semana Financiera</h1>

<p align="center">
  <em>Siete dÃ­as para organizar tus ingresos, cubrir necesidades y construir un ahorro responsable.</em>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white" alt="HTML5">
  <img src="https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white" alt="CSS3">
  <img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=111111" alt="JavaScript">
  <img src="https://img.shields.io/badge/GÃ©nero-SimulaciÃ³n-8758C7?style=for-the-badge" alt="GÃ©nero simulaciÃ³n">
  <img src="https://img.shields.io/badge/Estado-Funcional-20B26B?style=for-the-badge" alt="Estado funcional">
</p>

<p align="center">
  <a href="https://katfipol.github.io/game-development-portfolio/juegos/myeconomy/"><strong>JUGAR EN EL NAVEGADOR</strong></a>
  &nbsp;&nbsp;|&nbsp;&nbsp;
  <a href="index.html"><strong>VER CÃ“DIGO</strong></a>
  &nbsp;&nbsp;|&nbsp;&nbsp;
  <a href="../../README.md"><strong>VOLVER AL PORTAFOLIO</strong></a>
</p>

---

## DescripciÃ³n

**MyEconomy: Semana Financiera** es un videojuego educativo de simulaciÃ³n y estrategia casual. El jugador administra la economÃ­a de un joven durante siete dÃ­as: recibe ingresos, paga gastos obligatorios, recoge monedas, utiliza el banco y decide cuÃ¡nto ahorrar o gastar.

El proyecto transforma conceptos financieros en decisiones jugables. No basta con acumular dinero: el resultado final tambiÃ©n considera la salud financiera y la responsabilidad demostrada durante la semana.

## Ficha del proyecto

| Elemento | InformaciÃ³n |
|---|---|
| Asignatura | Game Development |
| Tema de la prÃ¡ctica | Game Design Document (GDD) |
| GÃ©nero | SimulaciÃ³n y estrategia casual con elementos de aventura |
| Tema central | Uso responsable del dinero |
| PÃºblico objetivo | JÃ³venes de 18 a 25 aÃ±os |
| DuraciÃ³n | Siete dÃ­as dentro del juego |
| Plataforma | Navegador web |
| Modalidad | Un jugador |
| Perspectiva | Ciudad 2D con profundidad visual |
| Integrantes | Melani Quintela Aguilar y JosÃ© MartÃ­n LeaÃ±o Mercado |

## Problema y propÃ³sito

La prÃ¡ctica plantea el caso de la cooperativa **Ahorro Joven**, cuyas charlas sobre administraciÃ³n del dinero no producen suficiente participaciÃ³n ni aprendizaje duradero. La propuesta consiste en sustituir la explicaciÃ³n pasiva por una experiencia donde cada decisiÃ³n tenga una consecuencia visible.

MyEconomy permite practicar tres ideas esenciales:

- Diferenciar necesidades y deseos.
- Reservar dinero antes de realizar compras personales.
- Evaluar cÃ³mo las decisiones pequeÃ±as afectan una meta de varios dÃ­as.

## Concepto definido en el GDD

El jugador controla a un joven que atraviesa situaciones econÃ³micas cotidianas. Durante el recorrido puede generar ingresos, recolectar monedas, cubrir necesidades, utilizar servicios bancarios y elegir entre compras Ãºtiles o impulsivas.

El objetivo es completar la semana con las obligaciones pagadas, una situaciÃ³n financiera estable y la mayor cantidad de ahorro responsable posible.

## Ciclo principal de juego

```mermaid
flowchart TD
    A[Comenzar el dÃ­a] --> B[Cobrar el sueldo]
    B --> C[Explorar y recoger monedas]
    C --> D[Pagar gastos obligatorios]
    D --> E{Administrar el dinero restante}
    E -->|Ahorrar| F[Depositar en el banco]
    E -->|Comprar| G[Evaluar utilidad y consecuencias]
    F --> H[Revisar balance]
    G --> H
    H --> I{Â¿Es el dÃ­a 7?}
    I -->|No| A
    I -->|SÃ­| J[EvaluaciÃ³n financiera final]
```

## EconomÃ­a de la partida

| Concepto | Valor |
|---|---:|
| Dinero inicial | Bs 700 |
| Sueldo diario | Bs 80 |
| Cobros permitidos | Uno por dÃ­a |
| Meta semanal de ahorro | Bs 500 |
| Monedas disponibles | Cinco por dÃ­a |
| Valor de cada moneda | Bs 5 |
| DuraciÃ³n | Siete dÃ­as |

### Gastos obligatorios diarios

| Gasto | Importe |
|---|---:|
| Vivienda | Bs 45 |
| Servicios | Bs 15 |
| AlimentaciÃ³n | Bs 20 |
| Transporte | Bs 10 |
| **Total diario** | **Bs 90** |

No es posible avanzar al siguiente dÃ­a mientras exista algÃºn gasto obligatorio pendiente.

## Lugares interactivos

| Lugar | FunciÃ³n |
|---|---|
| Banco | Depositar dinero en el ahorro o retirar una cantidad guardada |
| Tienda | Comparar y adquirir compras personales |
| Trabajo | Cobrar el sueldo una sola vez durante el dÃ­a |
| Hogar | Consultar dinero, ahorro, obligaciones, placer, estrÃ©s y monedas |
| Meta | Revisar el progreso hacia el objetivo de Bs 500 |

Los edificios poseen siluetas diferenciadas y accesos visibles. TambiÃ©n se puede interactuar mediante los botones laterales para facilitar la navegaciÃ³n.

## Compras y decisiones

| Producto | Precio | Tipo | Consecuencia principal |
|---|---:|---|---|
| Auriculares premium | Bs 140 | Impulsiva | Aumenta el placer, pero reduce la salud financiera |
| Videojuego | Bs 95 | Impulsiva | Aumenta el placer y reduce el margen disponible |
| Curso corto | Bs 70 | Inteligente | Mejora la salud financiera y la reputaciÃ³n |
| Regalo sentimental | Bs 60 | Inteligente | Aporta placer con un impacto financiero controlado |

El juego no presenta todos los gustos como incorrectos. La evaluaciÃ³n considera el equilibrio entre disfrute, ahorro y cumplimiento de responsabilidades.

## Indicadores

- **Dinero disponible:** recursos que pueden utilizarse inmediatamente.
- **Ahorro:** dinero separado mediante el banco.
- **Salud financiera:** estabilidad producida por las decisiones econÃ³micas.
- **Placer:** satisfacciÃ³n obtenida durante la semana.
- **EstrÃ©s:** presiÃ³n generada por el paso de los dÃ­as y algunas compras.
- **ReputaciÃ³n:** clasificaciÃ³n de A a D segÃºn las decisiones tomadas.
- **Historial:** registro de ingresos, pagos, depÃ³sitos y compras.

## EvaluaciÃ³n final

Al cerrar correctamente el sÃ©ptimo dÃ­a, el juego calcula una puntuaciÃ³n sobre 100:

| Componente | Peso |
|---|---:|
| Cumplimiento de la meta de ahorro | 35 % |
| Salud financiera | 35 % |
| Responsabilidad de las decisiones | 30 % |

La responsabilidad disminuye con las compras impulsivas y aumenta con las decisiones inteligentes. Todos los valores se limitan a un rango vÃ¡lido antes de calcular el resultado.

| PuntuaciÃ³n | Resultado |
|---:|---|
| 85â€“100 | Semana excelente |
| 70â€“84 | Semana responsable |
| 55â€“69 | Semana equilibrada |
| 40â€“54 | Semana complicada |
| 0â€“39 | Semana de riesgo |

AdemÃ¡s de la calificaciÃ³n, la pantalla final presenta el dinero, el ahorro, la salud financiera, los gastos obligatorios, los gastos personales y la cantidad de decisiones impulsivas.

## Reglas principales

1. La partida comienza con Bs 700.
2. El sueldo de Bs 80 solo puede cobrarse una vez por dÃ­a.
3. Cada jornada genera cinco monedas nuevas en posiciones variables.
4. Todos los gastos obligatorios deben pagarse antes de avanzar.
5. El banco separa el ahorro del dinero disponible.
6. Una compra solo se completa si existe dinero suficiente.
7. Las decisiones modifican indicadores y quedan registradas.
8. La evaluaciÃ³n se habilita despuÃ©s de completar las obligaciones del dÃ­a siete.

## Controles

| Entrada | AcciÃ³n |
|---|---|
| `W` `A` `S` `D` | Mover al personaje |
| Flechas | Movimiento alternativo |
| `E` | Interactuar con un edificio cercano |
| Clic | Abrir edificios o recoger monedas |
| Botones de interfaz | Pagar, ahorrar, comprar, guardar y avanzar |

## DiseÃ±o de la ciudad

La interfaz combina una ciudad colorida con paneles financieros de alto contraste. Cada espacio se reconoce por su arquitectura:

- El banco utiliza fachada institucional, columnas y sÃ­mbolo monetario.
- La tienda presenta escaparate, toldo y seÃ±alizaciÃ³n comercial.
- El trabajo se representa como un edificio de oficinas.
- El hogar tiene techo, chimenea, ventanas y jardÃ­n.
- La meta se identifica como un punto independiente de progreso.

La avenida dispone de carriles definidos y los vehÃ­culos circulan Ãºnicamente por la carretera. El personaje y los edificios cuentan con colisiones para evitar que el jugador atraviese las construcciones.

## TecnologÃ­as utilizadas

| TecnologÃ­a | AplicaciÃ³n en el proyecto |
|---|---|
| HTML5 | Estructura de la interfaz, paneles, modales y controles |
| CSS3 | DiseÃ±o adaptable, colores, sombras, tarjetas y jerarquÃ­a visual |
| JavaScript | EconomÃ­a, reglas, dÃ­as, compras, indicadores y evaluaciÃ³n |
| Canvas 2D | Ciudad, edificios, personaje, monedas, vehÃ­culos y colisiones |
| LocalStorage | Guardado y recuperaciÃ³n del progreso de la semana |

El videojuego se encuentra integrado en un Ãºnico archivo `index.html` y no requiere dependencias externas.

## OrganizaciÃ³n tÃ©cnica

```text
myeconomy/
â”œâ”€â”€ index.html   # Juego, estilos, ciudad y sistema econÃ³mico
â””â”€â”€ README.md    # DocumentaciÃ³n individual del proyecto
```

El estado de la partida concentra el dÃ­a, dinero, ahorro, indicadores, gastos pagados, posiciÃ³n del jugador, monedas, compras, historial y progreso. Las funciones de la interfaz actualizan esos datos y guardan la partida localmente.

## RelaciÃ³n con el GDD

| Componente del GDD | ImplementaciÃ³n observable | Estado |
|---|---|---|
| Concepto y premisa | AdministraciÃ³n de ingresos, gastos, ahorro y compras cotidianas | Cumplido |
| GÃ©nero | SimulaciÃ³n financiera con exploraciÃ³n y decisiones | Cumplido |
| Objetivo | Completar siete dÃ­as con estabilidad y ahorro | Cumplido |
| MecÃ¡nica principal | Recolectar y decidir entre pagar, ahorrar o gastar | Cumplido |
| Reglas | Ingresos limitados, obligaciones, banco y consecuencias | Cumplido |
| ProgresiÃ³n | Jornadas sucesivas con pagos, monedas y presiÃ³n acumulada | Cumplido |
| Personaje | Avatar controlable dentro de la ciudad | Cumplido |
| Arte y estilo visual | Ciudad 2D moderna, colorida y legible | Cumplido |
| PÃºblico objetivo | Situaciones financieras dirigidas a jÃ³venes | Cumplido |
| Victoria o resultado negativo | Cinco categorÃ­as de evaluaciÃ³n al finalizar la semana | Cumplido |

## ValidaciÃ³n de la prÃ¡ctica

La tabla entregada registra **â€œSÃ­â€ en todos los criterios de validaciÃ³n**:

- El prototipo funciona sin errores tÃ©cnicos.
- La mecÃ¡nica coincide con la descrita en el GDD.
- La presentaciÃ³n mantiene la propuesta de la infografÃ­a.
- Es posible alcanzar la condiciÃ³n favorable y el resultado financiero negativo.
- La experiencia enseÃ±a a utilizar el dinero responsablemente.

La observaciÃ³n original fue positiva. Antes de publicar el documento final se reformularÃ¡ con una redacciÃ³n acadÃ©mica mÃ¡s precisa.

## EvoluciÃ³n del prototipo

| Ãrea | Mejora incorporada |
|---|---|
| DuraciÃ³n | Semana completa de siete dÃ­as con cierre y evaluaciÃ³n |
| Balance | Bs 700 iniciales, sueldo diario limitado y gastos obligatorios |
| InteracciÃ³n | Edificios accesibles por proximidad, clic o botones |
| Ciudad | Construcciones reconocibles, zonas verdes y avenida definida |
| Movimiento | Colisiones con edificios y fuente central |
| VehÃ­culos | Recorrido restringido a los carriles de la avenida |
| Aprendizaje | SeparaciÃ³n entre necesidades, ahorro y decisiones personales |
| Persistencia | Guardado del progreso mediante LocalStorage |
| Resultado | EvaluaciÃ³n ponderada con cinco categorÃ­as financieras |

## Uso de inteligencia artificial

La prÃ¡ctica permite utilizar herramientas de IA siempre que el equipo comprenda y pueda defender tÃ©cnicamente los resultados. **ChatGPT** fue la herramienta principal de apoyo para convertir el GDD en un prototipo, programar la economÃ­a, construir la ciudad y realizar correcciones funcionales y visuales.

El equipo definiÃ³ y revisÃ³ los montos, reglas, decisiones, condiciones de avance, arquitectura de la ciudad y sistema de evaluaciÃ³n. La IA se presenta como una herramienta de apoyo dentro de un proceso dirigido y validado por los estudiantes.

<details>
<summary><strong>Prompt reconstruido del proceso</strong></summary>

> Desarrolla en un Ãºnico archivo HTML un videojuego educativo llamado MyEconomy. Debe ser una simulaciÃ³n financiera de siete dÃ­as en una ciudad 2D colorida. El jugador comienza con Bs 700, cobra un sueldo de Bs 80 una sola vez por dÃ­a y debe pagar diariamente vivienda, servicios, alimentaciÃ³n y transporte antes de avanzar. Incluye cinco monedas de Bs 5 por jornada, un banco para depositar y retirar ahorro, una meta de Bs 500, una tienda con decisiones Ãºtiles e impulsivas, indicadores de dinero, ahorro, salud financiera, placer, estrÃ©s y reputaciÃ³n, ademÃ¡s de guardado con LocalStorage. Permite moverse con WASD o flechas, interactuar con E o clic y evita que el personaje atraviese edificios. DiseÃ±a construcciones reconocibles, una carretera con autos restringidos a sus carriles y una evaluaciÃ³n final ponderada al terminar el dÃ­a siete.

Este texto es una **reconstrucciÃ³n basada en el GDD y en las mejoras solicitadas**; no corresponde a una copia literal del prompt original.

</details>

## Pruebas recomendadas

- [ ] Confirmar que el sueldo solo pueda cobrarse una vez por dÃ­a.
- [ ] Intentar avanzar sin pagar las obligaciones.
- [ ] Depositar y retirar cantidades vÃ¡lidas e invÃ¡lidas.
- [ ] Comprobar compras con dinero suficiente e insuficiente.
- [ ] Recoger las cinco monedas y verificar su regeneraciÃ³n diaria.
- [ ] Guardar, recargar la pÃ¡gina y recuperar el progreso.
- [ ] Completar una semana responsable y otra de riesgo.
- [ ] Verificar colisiones y recorrido de los vehÃ­culos.

## Aprendizajes

- Utilizar un GDD como guÃ­a antes y durante la programaciÃ³n.
- Convertir reglas escritas en condiciones verificables.
- DiseÃ±ar un ciclo de juego basado en ingresos, obligaciones y decisiones.
- Equilibrar varios indicadores en una evaluaciÃ³n final.
- Implementar persistencia mediante LocalStorage.
- Construir una ciudad interactiva y sus colisiones con Canvas 2D.
- Comunicar educaciÃ³n financiera mediante consecuencias jugables.

## EjecuciÃ³n local

1. Descarga o clona el repositorio.
2. Abre la carpeta `juegos/myeconomy/`.
3. Ejecuta `index.html` en un navegador moderno.

No requiere instalaciÃ³n, servidor ni paquetes externos.

---

<p align="center">
  <a href="https://katfipol.github.io/game-development-portfolio/juegos/myeconomy/"><strong>Jugar ahora</strong></a>
  &nbsp;&nbsp;|&nbsp;&nbsp;
  <a href="../../README.md"><strong>Explorar los seis videojuegos</strong></a>
</p>
