---
layout: post
title:  "Proposta"
date:   2017-03-31 00:00:00 +0200
---

## Aluno: Pedro Marcondes
## Supervisores: Carolina Brum e Marcelo Queiroz
## Tema: Uso de sensores para estimar o ângulo de uma articulação
 * &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Um instrumento aumentado é um instrumento tradicional cuja capacidades são amplificadas com o uso de sensores, tipos de produção de som e/ou diferentes formas de interação entre instrumento e instrumentista.
 * &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; O objetivo do trabalho é conseguir estimar de uma maneira confiável o ângulo de uma articulação(entre o braço e antebraço especificamente)  para ser aplicado no contexto de mapeamento de movimentos de instrumentistas para o campo de instrumentos aumentados.
 * &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Buscamos alternativas para refinar algoritmos usados atualmente, como o uso de quatérnions para representação das rotações, a fim de evitar problemas e limitações relacionados com as representações por eixos ou Euler(eixos constantemente variando e “Gimbal Lock”), técnicas como o método de gradiente descendente e Gauss-Newton que conseguiram diminuir o custo computacional.

## Motivação
 * &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; O "tracking" de movimentos possui uma área muito vasta de aplicações, se extendendo desde a medicina até o cinema. Nesse trabalho em especial a motivação final é artística, aumentar o instrumento.

## Objetivos
 * &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; O primeiro objetivo é conseguir estimar o ângulo entre o braço e antebraço com o uso de sensores.
 * &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Depois pretendemos aplicar no baixo elétrico afim de usar a angulação da articulação mencionada como controlador de efeito no som produzido pelo instrumento, desenvolvendo assim um baixo aumentado.

## Atividades
 * &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Primeira parte será o estudo teórico. Esse estudos serão focados em entender sensores e seu uso no universo musical[1], algorítmos que usam sensores para estimar orientação, ângulo, etc, como em [2][3][4] e algumas técnicas utilizadas nesse campo, como o Kalman Filter [5]
 * &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Pretendemos implementar um sistema que seja capaz de fazer essa estimação com melhor performance
 * &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Após concluído essa fase do desenvolvimento usaremos esse sistema para aumentar o baixo.

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
* [1]MEDEIROS, Carolina Brum; WANDERLEY, Marcelo M. A comprehensive review of sensors and instrumentation methods in devices for musical expression. Sensors, v. 14, n. 8, p. 13556-13591, 2014.
* [2]COMOTTI, Daniele; ERMIDORE, Michele. _Quaternion based Extended Kalman Filter for a 9DOF IMU_.2011.
* [3]DUMITRU, Nicolae; GRECU, Luminita; GRECU, Valentin. _Analysis of Human Arm Joints and Extension of the Study to Robot Manipulator_. Proceedings of the International MultiConferennce of Engineers and Compute Scientists 2009 Vol 2.
* [4]MARINS, João Luís, et al. _An extended Kalman filter for quaternion-based orientation estimation using MARG sensors_. Intelligent Robots and Systems, 2001. Proceedings. 2001 IEEE/RSJ International Conference on. Vol. 4. IEEE, 2001.
* [5]WELCH, Greg; BISHOP, Gary. An introduction to the Kalman filter. 1995.

