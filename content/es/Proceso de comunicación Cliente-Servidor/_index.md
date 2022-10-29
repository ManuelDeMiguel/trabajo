---
title: "Proceso de comunicación Cliente/Servidor"
date: 2022-10-28T16:33:52+02:00
draft: false
weight: 2
---

## ¿Qué ocuerre en el Proceso Cliente/Servidor?
El proceso comienza cuando el **Cliente** le realiza una petición de un recurso al **Servidor**. Este último, realizara una petición interna al **Proceso** que el **Cliente** ha solicitado para poder conectarlos. El **Proceso** respondera al **Servidor** y, finalmente, el **Servidor** pone en disposición el recurso solicitado por el **Cliente**.

##### Grafico ilustrativo
```mermaid
  graph LR;
      A[Cliente]--Pregunta-->B[Servidor];
      B--Pregunta-->D[Proceso];
      D--Responde-->B;
      B--Responde-->A;
```

