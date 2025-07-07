# Fonte de Tensão Ajustável - USP - 2025
## Projeto desenvolvido para a disciplina de Eletrônica para Computadores
## Tabela de Componentes:
| Componente | Quantidade | Preço (R$) |
| -----------|:----------:|-----:|
| Transformador 24V | 1 | emprestado|
| Diodo 1N4007 | 4 | 0,20 * 4 = 0,80 |
| Diodo Zener 1N4743 | 1 | 0,50 |
| LED vermelho S530-L | 1 | 0,50 |
| Resistor 1k Ohms LGE | 1 | 0,07 |
| Resistor 100 Ohms ROHS | 1| 0,07 |
| Resistor 120 Ohms ROHS | 1| 0,07|
| Resistor 2.2k Ohms ROHS | 2| 0,07 * 2 = 0,14|
| Capacitor 1 mF X35V | 1 | 2,00|
| Potenciômetro 10k B-16 | 1 | 7,00 |
| Transistor NPN BC337-40 | 1 | 0,70|
| Total | | 11.85 |

## Componentes:
- **Transformador**: primeiro componente do circuito após a fonte de corrente alternada (tomada). Será responsável por reduzir de 127v a ddp proveninete da tomada para o valor desejado pela projeto (3-12v). O transformador escolhido é capaz de abaixar a tensão de 110 volts para 12 volts.
_Obs.: o transformador apenas altera o valor da diferença de potencial entre seus terminais, não alterando de corrente alternada para corrente contínua._

- **Diodo**: permite que a corrente elétrica siga uma única direção 
  <br> **Ponte de diodo**: utilizada para que o circuito seja abastecido com a corrente em ambos ciclos da corrente alternada.

- **Fusível**: dispositivo de segurança que impede a passagem de correntes muito alta, protegendo os dispositivos do circuito em eventuais picos de corrente.

- **Varistor**: dispositivo de segurança que, em conjunto com o fusível, protege contra sobre tensão da rede.

- **Capacitor**: armazena a carga durante os ciclos da corrente alternada, liberando corrente quando a tensão interna é maior que a tensão vinda da fonte. Descarrega quando ocorre a inversão de ciclo. O capacitor foi escolhido para um ripple de 10%, calculando chegamos à um valor de 458uF(1000uF), foi escolhido o valor comercial próximo de 470uF. (nosso n estão batendo)

- **Diodo Zener**: regulador de tensão máxima. Somente conduz corrente quando a tensão que chegar alcança a tensão nominal do diodo, que no caso deste projeto, será 12v. Se a tensão for menor do que 12v, o Diodo não conduz e, portanto, não interfere no circuito, se for maior, deixará a corrente passar, mantendo a tensão em 12v naquele ponto. Informalmente, o diodo Zener “trava” o valor da tensão em 12v, que é exatamente o valor de tensão máximo que queremos na saída da nossa fonte.

- **Resistores**: complementam o circuito de forma a limitar a corrente e impedindo que a corrente do circuito ultrapasse os valores limites dos componentes. OBS.: nas imagens a resistência depois do potenciômetro é de 4.4k ohms, apesar de estar escrito 5.4k. O circuito no falstad via link contém as informações corretas.

- **Potenciômetro**: *resistor* variável que permitirá o controle do valor da tensão resultante entre 3 e 12 volts.

- **Transistor**: utilizado para permitir a passagem da corrente de forma ajustável.

## Imagem do circuito
![alt text](https://github.com/DaniloSStocco/FonteAjustavelUSP/blob/main/imagens/imagemCircuitoFalstad.png "Imagem do circuito no falstad")

## Link para circuito no Falstad
https://tinyurl.com/ytld4qlu

## Imagem Esquemática da PCB
![alt text](https://github.com/DaniloSStocco/FonteAjustavelUSP/blob/main/imagens/esquematica.png "Imagem do circuito esquemático")


## Imagem PCB
![alt text](https://github.com/DaniloSStocco/FonteAjustavelUSP/blob/main/imagens/PCBeagle.png "Imagem do circuito no PCB no Eagle")

## Vídeo no Youtube
https://youtube.com/shorts/0OYnWFA0fto?si=zNpCkuGSwgYqhvWx

## Foto do circuito
![alt text](https://github.com/DaniloSStocco/FonteAjustavelUSP/blob/main/imagens/circuitocima.heic "Foto do circuito por cima")
![alt text](https://github.com/DaniloSStocco/FonteAjustavelUSP/blob/main/imagens/circuitolado1.heic "Foto do circuito por um lado")
![alt text](https://github.com/DaniloSStocco/FonteAjustavelUSP/blob/main/imagens/circuitolado2.heic "Foto do circuito por outro lado")

## Alunos
- Danilo Salmen Stocco
- Diogo Salmen Stocco
- Felipe Carlos Savoia Glücksman
- Rafael Senger

