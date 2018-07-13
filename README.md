# Robô lutador de sumô

Projeto desenvolvido para a competição [SumốCup](http://www.lasec.feelt.ufu.br/sumocup) realizada em outubro de 2017 na Universidade Federal de Uberlândia e organizada pelo [LASEC](http://www.lasec.feelt.ufu.br/).

Esta competição tem por obetivo, como na luta entre humanos, jogar o adversário para fora do dojô de forma autonoma ou então apenas ser o ultimo a sair do dojô. Abaixo alguns exemplos:

![](img/Sumo001.gif)

As imagens mostradas acima são de uma categoria acima à do sumô e com um nível mais avançado de competitividade.  

## Sobre o projeto

Este projeto possui conceitos bem simples de programação em linguagem .ino juntamente com a IDE do [arduino](https://www.arduino.cc/en/Main/Software) e usa a logica condicional para o seu sistema de controle.

## Materiais utilizados

* Arduino UNO R3
* Micro motor com caixa de redução 1000 rpm
* Sensores de refletância
* Sensor ultrassom
* Drive ponte H l298
* Jumpers
* Protoboard
* Push Buttons

## Estrégia utilizada

Sua lógica de controle foi pensada para ao inicio do round o robô vá até ao centro do dojô e lá começar a procurar pelo adversário. Foram criadas três funções neste código, a função **procura** a função **ataque** e a função **voltar ao campo**.

Na função **procura** o robô se dirige ao centro do dojo, como citado acima e procura o adversário rodando no seu própio eixo, quando o advesário é encontrado, pelo sensor ultrassom, a função **ataque** é chamada e o robô empurra-o com toda a força para fora do dojo. Caso o robo saia do centro, por ser empurrado ou para atacar, a função **voltar ao campo** é chamada, ela impede que o robô saia do dojo.

## hardware

Este projeto foi concebido Basicamente de materiais reciclados, os dois andares do chassi foram feitos de compensado de madeira, o suporte para a roda traseira ,a chamada "roda boba" e para o sensor traseiro foi improvisada de uma tampa de garrafa PET. Para aumentar a tração das rodas utilizamos pulseiras elásticas, uma solução improvisada de ultima hora.

Abaixo podemos ver uma foto do robô já montado:

![](img/sumo02.jpg)

## Resultados

![](img/Gyniu_vs_Colmeia.gif)

Em um contexto geral o robô conseguiu cumprir com a maioria dos seus objetivos de forma autônoma, não saiu do dojô sozinho e conseguiu vencer algumas lutas. O principal desafio apresentado foi com relação à altura do robô, por conta da limitação de área imposta pela competição e pelo fato de os hardwares utilizados ocuparem uma àrea relativamente grande, a altura em que o robô ficou o deixou muito instável com relação movimentos bruscos acarretando assim algumas quedas.   

Neste [link](https://www.youtube.com/watch?v=NO75CmzcxgI&list=PLWZrpNc7OyMwNlyV_De-JO6rOj_Rl_izD&t=0s&index=2) têm alguns videos da competição.

##licenses

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details

```
"THE BEERWARE LICENSE" (Revision 42):
Italo Fernandes, Mario Borges and Luiz Henrique wrote this code.
As long as you retain this notice, you can do whatever you want with this stuff.
If we meet someday, and you think this stuff is worth it, you can buy us a beer in return.
```

## Authors

* **Mario Borges** - https://github.com/alpinista06

* **Jabora** - https://github.com/jabora

* **Guilherme Balduino** - https://github.com/guibalduino
