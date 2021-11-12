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
  - [Wallets](#wallets)

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