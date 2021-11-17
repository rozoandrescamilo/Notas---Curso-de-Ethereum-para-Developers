# Notas del Curso de Ethereum para Developers

Profesor Gustavo Grillasca

![](https://static.platzi.com/media/avatars/Platzi-f730e65b-e92b-44d3-81c0-5c59c4dc4658.png) ![](https://static.platzi.com/media/learningpath/badges/29fa8885-7536-44ba-8aea-7b32c8e39cc8.jpg) ![](https://static.platzi.com/media/achievements/piezas-ethereum-developers_badge-2bb9aed8-f119-429b-b925-7ca075749d3b.png)

## Tabla de Contenidos

- [Introducción a Ethereum](#introducción-a-ethereum)
  - [Componentes de Ethereum](#componentes-de-ethereum)
  - [La moneda ETH y GAS](#la-moneda-eth-y-gas) 
  - [Etapas de desarrollo y actualizaciones programadas](#la-moneda-eth-y-gas) 
- [Criptografía](#criptografía)
  - [¿Qué es la criptografía asimétrica?](#qué-es-la-criptografía-asimétrica)
  - [Wallets](#wallets) 
- [Principales aplicaciones](#principales-aplicaciones)
  - [Smart Contracts](#smart-contracts)
  - [DeFi](#defi) 
  - [NFT](#nft)
  - [Aplicaciones Descentralizadas](#aplicaciones-descentralizadas)
- [Mecanismos de consenso](#mecanismos-de-consenso)
  - [Proof-of-Work, Proof-of-Stake y sistemas híbridos](#proof-of-Work-proof-of-stake-y-sistemas-híbridos)
  - [Ethash y Casper](#ethash-y-casper)
  - [Forks](#forks)
  - [EIP y solucines de escalado](#eip-y-solucines-de-escalado)

# Introducción a Ethereum

**Ethereum** es una plataforma para ejecutar contratos inteligentes a través de una **Máquina Virtual** que aplica los cambios al sistema.  Ethereum es una "Open Blockchain" que utiliza una cadena de bloques para sincronizar y guardar los cambios que ocurren al estado del sistema, y ​​utiliza una criptomoneda llamada Ether (ETH) para medir y restringir los costos de ejecución.

Whitepaper de Ethereum: https://ethereum.org/en/whitepaper/

> **Open Blockchains** Abiertas a todos, públicas, neutrales, descentralizadas, globales y resistentes a la censura.  **Andreas Antonopoulos**

Ethereum se inventó para brindar un ambiente de trabajo determinado y seguro donde poder programar aplicaciones descentralizadas.  Esto sin necesidad de construir la infraestructura base de algoritmos de consenso y redes de persona a persona para cada nueva aplicación.

**Historia de Ethereum** 

1. Publicación del White Paper por Vitalik Buterin (2013).  
Un programador de 19 años desarrolla la idea general.  
2. Publicación del Yellow Paper del Dr. Gavin Wood (2014).  
Experto en C ++ Gavin se convierte en co-fundador y CTO.  
3. Preventa en Julio 2014. Una de las ICOS más exitosas de la historia.  
4. Frontera el 30 de julio de 2015. La primera de 4 etapas de desarrollo programadas.

Las 4 etapas programadas en el desarrollo de Ethereum:

1. Frontier (2015)
2. Homestead (2016)
3. Metropolis (2017)
4. Serenity (Ethereum 2.0)

[![1](https://github.com/hackmilo/Notas---Curso-de-Ethereum-para-Developers/blob/main/img/1.png?raw=true "1")](https://github.com/hackmilo/Notas---Curso-de-Ethereum-para-Developers/blob/main/img/1.png?raw=true "1")

## Componentes de Ethereum

Componentes Principales:

- **Red P2P:** Esta red hace referencia a un mecanismo de transferencia de igual a igual o persona a persona, sobre la cual no existe ningún ente central y de lo contrario se maneja la información de manera descentralizada y segura.

- **Algoritmo de consenso(Nakamoto):** Ethereum al igual que bitcoin poseen un mecanismo de consenso basado en una prueba de trabajo o proof of work(PoW), presentada en sus inicios por Satoshi Nakamoto el creador de bitcoin. De esta manera Satoshi logro pactar un acuerdo o un consenso entre los nodos, para decidir cual nodo es el encargado de generar un nuevo bloque y actualizar la blockchain, ya que no existe un ente central.

- **Ether:** Es la moneda propia de Ethereum, esta corre sobre la primera capa de la blockchain de Ethereum haciendola su moneda principal. El verdadero objetivo de esta moneda es servir como herramienta para poder construir la red de aplicaciones descentralizadas que corren dentro de Ethereum.

> Nota: Ether no es lo mismo que Ethereum, Ether es la moneda, y Ethereum es la red.

- **Ethereum Virtual Machine (EVM):** La maquina virtual de Ethereum es la principal encargada de leer y ejecutar la logica de los contratos inteligentes o Smart Contracts escritos en el lenguaje Solidity, para que la red blockchain pueda incluir e interpretar esta lógica. Cada uno de los nodos en su interior poseen esta maquina virtual.

- **Algoritmo criptográfico de seguridad (Ethash):** Es el algoritmo encargado de cifrar la información manejada en la blockchain de Ethereum. Los mineros utilizan este algoritmo para poder crear nuevos bloques.

- **Clientes (Geth, Parity):** Estos clientes son paquetes que instalas en tu computador para poder correr un nodo dentro de este y poder conectarte a la red blockchain de Ethereum.

Conceptos relevantes:

- **Clientes/Nodos:** Los clientes son los encargados de empaquetar el sistema sobre el cual se puede ejecutar un nodo en la red BlockChain. Cuando instalas en tu computador este cliente, automáticamente te conviertes en un nodo participante en la red de Ethereum.

- **Wallets:** Las wallets o billeteras son aplicaciones que nos permiten administrar nuestras cuentas de Ethereum o de cualquier otra red, para poder interactuar con otras personas que también sean parte de esta red. Además de poder controlar nuestros fondos y activos.

- **Smart Contracts:** Son los programas que nos permiten comunicarnos con la blockchain a partir de ciertas condiciones especificadas dentro de el contrato inteligente. Estos contratos se ejecutan dentro de la EVM para ser analizados y posteriormente implementados en la blockchain.

- **Web3:** Es una nueva web descentralizada sobre la cual no necesariamente va a existir un ente central, si no que de lo contrario, al ser una red descentralizada o P2P vamos a hacer nosotros mismos los usuarios los encargados tomar decisiones autónomas sin necesidad de recurrir o de pedir información a un ente central.

## La moneda ETH y GAS

**¿Qué es el ETH?**  

Ether (ETH) es la moneda nativa de la red Ethereum.  Sirve para hacer transferencias de valor, para pagar a los mineros, para correr programas y como mecanismo de seguridad contra errores en la EVM a través del GAS.

**¿Qué es el GAS en Ethereum?**

El GAS es una cantidad de ETH necesaria para interactuar con la red de Ethereum, y que sirve como gasolina para alimentar la EVM.

## Etapas de desarrollo y actualizaciones programadas

Las 4 etapas programadas en el desarrollo de Ethereum:

1. Frontier (2015)
2. Homestead (2016)
3. Metropolis (2017)
4. Serenity (Ethereum 2.0) Transición de PoW a PoS

# Criptografía

> **La criptografía** es la práctica y el estudio de métodos para proteger información a través de codificar mensajes.

## ¿Qué es la criptografía asimétrica?

La criptografía asimétrica es uno de los tipos de criptografía informática y una de las técnicas de criptografía más potentes diseñadas en base al uso de una fórmula matemática muy compleja para crear un par de claves: la clave privada y la clave pública. A través de estas claves se establece un canal de comunicación seguro entre las partes, en el que tanto el emisor como el receptor deben usar criptografía asimétrica con un mismo algoritmo definido, que les permitirá crear un juego de claves único e irrepetible para cada uno.

[![2](https://github.com/hackmilo/Notas---Prework-para-Desarrollo-de-Aplicaciones-Blockchain/blob/main/img/2.png?raw=true "2")](https://github.com/hackmilo/Notas---Prework-para-Desarrollo-de-Aplicaciones-Blockchain/blob/main/img/2.png?raw=true "2")

**Funciones Hash**

Las funciones hash son funciones que permiten llevar un contenido del dominio al rango de la función en tiempo polinomial. No obstante, invertir el hash es matemáticamente muy complejo y no viable. Es un método de integridad de la información.

[![3](https://github.com/hackmilo/Notas---Curso-de-Ethereum-para-Developers/blob/main/img/3.png?raw=true "3")](https://github.com/hackmilo/Notas---Curso-de-Ethereum-para-Developers/blob/main/img/3.png?raw=true "3")

Una función Hash es una función en la que tu puedes meter un texto y a través de aplicarle esta función te va a dar un resultado de una cadena de caracteres de un tamaño determinado, independientemente del tamaño del texto inicial.

A una llave privada, es decir un texto del tamaño que sea (En nuestro caso las doce palabras de una wallet) le aplicamos la función hash y esta nos devuelve una cadena de caracteres que es la llave pública.

Esta llave pública ó dirección la podemos publicar y decir a cualquiera, es como decir, que es la dirección de nuestro casillero de correos, ahí la gente puede meter dinero, nft, información, etc, pero solo que el tenga la llave privada puede acceder a los mismos, abrir el casillero.

## Wallets

Su función principal es proteger y administrar las privates keys, para que tu solo puedas validar tu identidad y hacer transacciones de valor dentro de la red.

> Your Keys, your coins, not your Keys, not your coins.

**Conceptos importantes:**

- **Accounts:**
  Entidades que tienen un balance en ETH y que pueden enviar transacciones.

- **Transacciones:**
  Una instrucción controlada por una cuenta que cambia el estado del sistema.

- **Firmas Digitales**
  Es una cadena de caracteres producida a partir de un texto con el HASH de una private key.

- **Tokens**
  Es un tipo de moneda o activo con utilidad o distinción que puede ser rastreado y transferido.

# Principales aplicaciones

## Smart Contracts

Es un programa o protocolo que se ejecuta de forma automática y descentralizada dentro de una blockchain, y sirve para controlar una acción o documentar un evento de acuerdo a los parámetros del código que lo componen.  

El objetivo de los SC es evitar la necesidad de confiar en un tercero para desintermediar los procesos y así abaratar costos, reducir tiempos de operación y minimizar fraudes.

[![4](https://github.com/hackmilo/Notas---Curso-de-Ethereum-para-Developers/blob/main/img/4.png?raw=true "4")](https://github.com/hackmilo/Notas---Curso-de-Ethereum-para-Developers/blob/main/img/4.png?raw=true "4")

## DeFi

> Descentralized Finance = DeFi

DeFi es la abreviatura de finanzas descentralizadas que incluyen activos digitales, protocolos, contratos inteligentes y dApps construidos en blockchain.

Podemos pensar en DeFi como un ecosistema financiero abierto donde se pueden construir varias herramientas y servicios financieros pequeños de manera descentralizada.

Estas se pueden combinar, modificar e integrar de acuerdo con sus necesidades.

Proyectos y aplicaciones con más relevancia:

- Decentralized Exchanges (DEX) 
- Stable Coins 
- Préstamos 
- Seguros 
- Derivados (contratos) 
- Margin Trade 
- Oráculos

## NFT

> Non Fungible Token - NFT

Es un token no fungible, una unidad de data que certifica un bien digital, esta propiedad lo hace único e irrepetible, por esta razón se puede aplicar esta tecnología en diferentes áreas como la medicina, el arte, los Meta versos, educación, inmuebles y eventos.

[![5](https://github.com/hackmilo/Notas---Curso-de-Ethereum-para-Developers/blob/main/img/5.png?raw=true "5")](https://github.com/hackmilo/Notas---Curso-de-Ethereum-para-Developers/blob/main/img/5.png?raw=true "5")

Proocolos relacionados:

- **ERC-20 (Ethereum Request for Comments)**
Fue el primer token utilizado para implementar funcionalidades usando blockchain de Ethereum.

- **ERC-721**
Tokens intercambiables únicos y no fungibles.

- **ERC-155**
Permite tokens fungibles y no fungibles.

## Aplicaciones Descentralizadas

Son aplicaciones descentralizadas que utilizan ‘blockchain’ para que los usuarios se relacionen directamente entre ellos y cierren acuerdos sin que exista una entidad central que gestione el servicio.

[![6](https://github.com/hackmilo/Notas---Curso-de-Ethereum-para-Developers/blob/main/img/6.png?raw=true "6")](https://github.com/hackmilo/Notas---Curso-de-Ethereum-para-Developers/blob/main/img/6.png?raw=true "6")

# Mecanismos de consenso

## Proof-of-Work, Proof-of-Stake y sistemas híbridos

> La revolución será descentralizada.

**Algoritmos de consenso:** 

Mecanismos para generar acuerdos entre distintos actores distribuidos ante la posibilidad de errores, información incompleta o en presencia de adversarios.

#### Proof of Work (PoW)

Proof of Work es un protocolo en el que su principal objetivo es la protección frente a los ataques distribuidos de denegación de servicio (DDoS). Este protocolo tiene grandes niveles de seguridad si la red esta formada por miles de mineros. De hecho, mientras más mineros, más segura es la red.

Las validaciones en la red se producen mediante un algoritmo de consenso llamado Prueba de Trabajo, que hasta la fecha ha demostrado ser eficiente manteniendo la red completamente segura, pero que al parecer no ha sido lo suficientemente amigable con el gasto energético.

#### Proof of Stake (PoS)

Proof of Stake (PoS) o Prueba de Participación, es un protocolo de consenso creado para reemplazar al conocido Proof of Work aportando una mejor seguridad y escalabilidad a las redes que lo implementen.

Es un proceso completamente distinto al conocido protocolo de Prueba de Trabajo (PoW). Donde cada uno de sus nodos realizan un arduo trabajo de cómputo para resolver acertijos criptográficos. Lo que significa que PoW, a diferencia de PoS, necesita de grandes cantidades de energía y equipo especializado para realizar sus operaciones. En PoS, por el contrario, esto no es necesario. En PoS el proceso es mucho más sencillo y energéticamente amigable. Son estas razones por la que muchos proyectos blockchain en la actualidad se interesan por este nuevo protocolo.

[![7](https://github.com/hackmilo/Notas---Curso-de-Ethereum-para-Developers/blob/main/img/7.png?raw=true "7")](https://github.com/hackmilo/Notas---Curso-de-Ethereum-para-Developers/blob/main/img/7.png?raw=true "7")

## Ethash y Casper

**Ethash:**

Ethash es el algoritmo PoW planeado para Ethereum 1.0. Es la última versión de Dagger-Hashimoto, aunque ya no se puede llamar así ya que muchas de las características originales de ambos algoritmos han cambiado drásticamente en el último mes de investigación y desarrollo.

Es el algoritmo que hace posible el funcionamiento de la minería en Ethereum. Un algoritmo de elevada calidad y que usa algunas técnicas informáticas muy elaboradas para garantizar la mayor seguridad posible.
Es altamente dependiente de operaciones en memoria RAM, consumiendo grandes cantidades de ancho de banda. El algoritmo es amigable con las GPU y Ofrece una excelente capacidad de verificación para cliente ligeros.

**Casper:**

Ethereum 2.0 (Serenity): de PoW a PoS

En este tipo de algoritmo los mineros serán reemplazados por validadores. Entonces el consenso se logrará a través del voto de los validadores. Cómo en cualquier algoritmo basado en PoS, el voto de cada validador dependerá del cantidad de Ethers depositados, es decir, de su participación.

Está diseñado para funcionar en un sistema sin confianza y ser más tolerante a fallas bizantinas. Esto significa que utiliza un proceso mediante el cual se puede castigar a los validadores maliciosos. Es decir, si un validador actúa de manera malintencionada será castigado de inmediato y se reducirá todo lo que está en juego. Lo mismo pasa si los validadores tienen tiempos de inactividad muy largos con su nodo. El descuido o la pereza les hará perder su apuesta. 

## Forks

- **Hardfork:** Es el momento en que se bifurca la red porque se crea otra moneda que no es compatible con las reglas anteriores. Por ejemplo, alguien puede crear una red Blockchain con un nuevo Bitcoin, pero pone como límite no 21millones sino 80millones, esto posible, solo que ahora no va ser parte de la red original de Bitcoin porque no cumple con las reglas originales ni la van a sostener esos mineros. Es otra Blockchain completamente distinta.

- **SoftFork:** Es cuando una red Blockchain o en el ejemplo de Bitcoin recibe una actualización, pero NO necesariamente se crea otra moneda y continúa siendo compatible con versiones anteriores.

- **Fork o Bifurcación:** Es la moneda es resultado de un Hardfork.

- **Snapshot:** Es el momento en el que se hace esa copia o división de la red, guardando toda la información de las transacciones y saldos hasta ese momento de la blockchain.

- **Ethereum Classic:** es un Fork (bifurcación) de Ethereum

**Dato curioso:** Un contrato de ethereum fue hackeado y se robaron millones de dólares. Algunos no aceptaron el error y otros dijeron “el codigo es ley” por lo que se tiene que respetar aún con el hackeo. Ethereum classic son aquellos que respetaron el código con todo y su error, ethereum es el fork de aquellos que no aceptaron el error cometido y crearon su propia cadena en donde esos fondos no fueron robados nunca.

[![8](https://github.com/hackmilo/Notas---Curso-de-Ethereum-para-Developers/blob/main/img/8.jpg?raw=true "8")](https://github.com/hackmilo/Notas---Curso-de-Ethereum-para-Developers/blob/main/img/8.jpg?raw=true "8")

## EIP y solucines de escalado

> EIP: Ethereum Improve Proposal - Protocolos para mejorar la red al hacer una propuesta por escrito, que los miembros puedan revisar y aportar, y lentamente ir traduciendo la propuesta escrita a un bloque programado que ejecute el cambio en la red con el mayor consenso posible.

Ethereum 2.0 busca:
- Cambio de PoW a PoS.
- Seguridad.
- Escalado. Que se puedan ejecutar más transacciones por segundo.
 
Para mejorarlo se proponen soluciones de Segunda Capa (L2) como:

- Sharding -> Fragmentar una base de Datos o motor de búsqueda para aligerar la concentración de recursos y facilitar funciones. Básicamente dividir la cadena principal en pequeñas cadenas, para que estas procesen transacciones, sin cargar todo el peso del procesamiento de transacciones a la cadena principal
- The Beacon Chain -> Una cadena paralela a la cadena de Ethereum que trabaja ya con PoS.
- Polygon (MATC)
- Raiden Network (LN)
- xdai(sidechain)
- Optimism (OVM Rollups)
- zkSync (scaleble skRollups)

