# Proyecto Amanda 2.0

Este documento tiene como finalidad decribir y documentar a nivel técnico el desarrollo del proyecto Amanda 2.0.

## Tecnologías

El nuevo enfoque del proyecto Amanda tiene como finalidad descentralizar el servicio cognitívo (actualmente [IBM Watson Assistant](https://www.ibm.com/cloud/watson-assistant)) y los canales de comunicación (actualmente Facebook y Gmail) , con la finalidad de dar más valor e importancia a las interacciones que Amanda puede conseguir con los usuarios.

Para lograr dicho enfoque se usaran tecnologías modernas y de rápido crecimiento, a continuación se pasarán a describir las más relevantes:

1. El lenguaje de proposito general en el que estarán escritos todos los servicios del proyecto Amanda 2.0 será [Go](https://golang.org) (Golang), dicho lenguaje es un lenguaje de programación que nacio en el 2009 con la vision de ser muy ágil y sencillo de entender. Actualment Go tiene una gran comunidad en todo el mundo y se perfila como el lenguaje de programación más usado para la web, algunos ejemplos de empresas que lo usan son Google, Docker, Uber, Mercado Libre.
2. La arquitectura de todos los procesos de Amanda estará basada en microservicios contenidos con [Docker](https://www.docker.com/) y orquestados con [Docker Swarm](https://docs.docker.com/engine/swarm) o [Kubernetes](https://kubernetes.io/). Es sabido que actualmente los microservicios permiten una alta escalabilidad en cualquier estadio de un proyecto, y con las herramientas anteriormente mencionadas se garantiza robustez.
3. El acceso a la información histórica de Amanda se realizará mediante una capa en [GraphQL](https://graphql.org/), esta tecnología, propuesta por Facebook, tiene ventajas sobre un [API REST](https://www.wikiwand.com/en/Representational_state_transfer) convencional debido a su orientación basada en grafos y en su modelo descriptivo y "vivo" de la data.
