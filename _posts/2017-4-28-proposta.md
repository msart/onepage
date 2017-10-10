---
layout: post
title:  "Proposta"
date:   2017-02-31 00:00:00 +0200
---

## Aluno: Pedro Marcondes
## Supervisores: Carolina Brum e Marcelo Queiroz
## Tema: Uso de sensores para estimar o ângulo de uma articulação
 * &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Um instrumento aumentado é um instrumento tradicional cuja capacidades são amplificadas com o uso de sensores, tipos de produção de som e/ou diferentes formas de interação entre instrumento e instrumentista.
 * &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; O objetivo do trabalho é conseguir estimar de uma maneira confiável o ângulo de uma articulação(entre o braço e antebraço especificamente)  para ser aplicado no contexto de mapeamento de movimentos de instrumentistas para o campo de instrumentos aumentados.
 * &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Buscamos alternativas para refinar algoritmos usados atualmente, como o uso de quatérnions para representação das rotações, a fim de evitar problemas e limitações relacionados com as representações por eixos ou Euler(eixos constantemente variando e “Gimbal Lock”)[1], técnicas como o método de gradiente descendente[2] e Gauss-Newton[2] que quando aplicadas a este problema conseguiram reduzir o custo computacional, como em [4][6].

## Motivação
 * &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; O “tracking” de movimentos possui uma área muito vasta de aplicações, se estendendo desde a medicina, no uso de braços robóticos para a execução de cirurgias, até o cinema, onde se usa o mapeamento do movimento de atores para criação de efeitos especiais, animações, etc. Neste trabalho em especial a motivação final é artística, aumentar o instrumento.

## Objetivos
 * &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; O primeiro objetivo é conseguir estimar o ângulo entre o braço e antebraço de um músico com o uso de sensores. Para esse trabalho serão utilizados acelerômetros, giroscópios e magnetômetros.
 * &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;  Depois pretendemos aplicar essa estimação no baixo elétrico afim de usar a angulação da articulação mencionada como controlador de efeito no som produzido pelo instrumento, desenvolvendo assim um baixo aumentado.

## Atividades
 * &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; A primeira parte compreenderá os estudos teóricos. Esses estudos serão focados em entender sensores e seu uso no universo musical[3], algoritmos que usam sensores para estimar orientação, ângulo, etc, como em [4][5][6] e algumas técnicas utilizadas nesse campo, como o Kalman Filter [7]
 * &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Pretendemos implementar um sistema que seja capaz de fazer essa estimação de maneira confiável e eficiente computacionalmente.
 * &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;  Após concluída essa fase do desenvolvimento usaremos esse sistema para desenvolver o baixo aumentado.

| Atividade              	| Abr 	| Mai 	| Jun 	| Jul 	| Ago 	| Set 	| Out 	| Nov 	|
|---------------------------|-------|-------|-------|-------|-------|-------|-------|-------|
| Estudo teórico         	|  X  	|  X  	|  X  	|  X  	|     	|     	|     	|     	|
| Implementação          	|     	|     	|  X  	|  X  	|  X  	|  X  	|     	|     	|
| Avaliação do Sistema   	|     	|     	|     	|     	|  X  	|  X  	|     	|     	|
| Aumentar o Instrumento 	|     	|     	|     	|     	|     	|  X  	|  X  	|     	|
| Monografia             	|     	|     	|     	|     	|  X  	|  X  	|  X  	|  X  	|
| Pôster                 	|     	|     	|     	|     	|     	|     	|  X  	|  X  	|
| Apresentação           	|     	|     	|     	|     	|     	|     	|     	|  X  	|

## Referências
* [1]HANSON, Andrew J. _Visualizing quaternions_. In: ACM SIGGRAPH 2005 Courses. ACM. 2005. p. 1.
* [2]BERTSEKAS, Dimitri P. _Nonlinear programming. Belmont: Athena scientific_.1999.
* [3]MEDEIROS, Carolina Brum; WANDERLEY, Marcelo M. _A comprehensive review of sensors and instrumentation methods in devices for musical expression_. Sensors, v. 14, n. 8, p. 13556-13591, 2014.
* [4]COMOTTI, Daniele; ERMIDORE, Michele. _Quaternion based Extended Kalman Filter for a 9DOF IMU_.2011.
* [5]DUMITRU, Nicolae; GRECU, Luminita; GRECU, Valentin. _Analysis of Human Arm Joints and Extension of the Study to Robot Manipulator_. Proceedings of the International MultiConferennce of Engineers and Compute Scientists 2009 Vol 2.
* [6]MARINS, João Luís, et al. _An extended Kalman filter for quaternion-based orientation estimation using MARG sensors_. Intelligent Robots and Systems, 2001. Proceedings. 2001 IEEE/RSJ International Conference on. Vol. 4. IEEE, 2001.
* [7]WELCH, Greg; BISHOP, Gary. An introduction to the Kalman filter. 1995.

## Source Code
* https://github.com/msart/Joint-angles-estimation-with-9dof-sensors

