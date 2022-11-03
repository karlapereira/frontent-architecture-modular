# [frontent-architecture-modular]
Exemplo de arquitetura modular com flux no front-end, no módulo Arquitetura de Front-End (2022) no curso de pós-graduação Arquitetura de Software Distribuído Latu Sensu - PUC MINAS

# Arquitetura
- Modular: Arquitetura para projetos que estão sempre em evolução e crescimento, agnóstica a frameworks e aplicável todas stacks.
- Flux: 
    - Action: São coleções de métodos que são chamadas pelas nossas Views, que enviam ações para o Dispatcher contendo payloads, que serão entregues aos Stores.
    - Dispatcher: É o componente que gerencia basicamente todo o processo da nossa aplicação. O ponto central são os métodos Register e Dispatch, que são triggers de eventos entre a ação que disparou o evento e as stores registradas. Ele simplesmente recebe a Action e propaga para as stores que irá identificá-la e disparar um evento caso registrado.
    - Stores: São os locais onde ficam armazenados a lógica e estado da aplicação, que tem call-backs registrados para o Dispatcher.
    - (Controller) Views: Responsáveis por permitir que o usuário interaja com a aplicação e por mostrar a ele o estado atual dela.

![image](https://user-images.githubusercontent.com/25828944/199854599-55c06047-e444-4ab7-9adb-0ccf8fa340d3.png)

Url: [https://facebook.github.io/flux/docs/in-depth-overview]
