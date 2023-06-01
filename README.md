# PSET1

#### Aluno: Gabriel Thomazi Rosa
#### Turma: CC3m

### Questão 1: 

  Se eu passar essa imagem pelo filtro de inversão, o output será apenas a inversão dos pixels originais. Sendo o valor máximo de um pixel em escala cinza 255, posso pegar cada pixel e subtrair de 255, 
  dessa forma eu iria encontrar o valor inverso. Entao a nova imagem teria a mesma largura e altura, porem os pixels[226, 166, 119,55].
  
### Questão 2: 
![alt text](https://github.com/Thomazi/pset1_abrantes/blob/main/imagem_invertida.png)

### Questão 3: 

  imagem de entrada = i, kernel = k, para aplicar k em i resulta em uma nova imagem O, mas com altura e largura iguais a i.  
  mas com os pixels que sao calculados de acordo com as regras descritas por k.  
  os pixels na posição (x, y) na imagem resultante, que é O
  									                                       x,y  
  com O 0,0   sendo o canto superior esquerdo.  
      

  ox,y = 80 * 0.00 + 53 * (-0.07) + 99 * 0.00 +  
	  129 * (-0.45) + 127 * 1.20 + 148 * (-0.25)+  
	  175 * 0.00 + 174 * (-0.12) + 193 * 0.00  

  Ox,y = 32.76  

  calculei utilizando a fórmula entregue:  

  Ox,y =Ix−1,y−1 × k0,0 + Ix,y−1 × k1,0 + Ix+1,y−1 × k2,0+  
  Ix−1,y × k0,1 + Ix,y × k1,1 + Ix+1,y × k2,1+   
  Ix−1,y+1 × k0,2 + Ix,y+1 × k1,2 + Ix+1,y+1 × k2,2  

  sendo ox,y a imagem resultante, eu apenas substitui os dados da fórmula pelo de kernel e o da imagem fornecida.  
  Por exemplo, na imagem inicial a posição x-1, y-1 indica o canto superior esquerdo, então, peguei o pixel da posição da imagem, que é 80 e multipliquei com o pixel da mesma posição no kernel entregue,  
  que era 0.00. Repetindo isso para todos os pixels e realizando a multiplicação e a soma encontrei o valor 32.76 da imagem resultante.  
  
### Questão 4: 
  ![alt_text](https://github.com/Thomazi/pset1_abrantes/blob/main/imagem_kernel.png)
 
### Questão 5: 
  
  ![alt text](https://github.com/Thomazi/pset1_abrantes/blob/main/gatinho_blur.png)  
  ![alt text](https://github.com/Thomazi/pset1_abrantes/blob/main/cobra.png)
  
  Não é possível realizar a operação de nitidez usando uma única correlação com um kernel adequado.
  A fórmula Sx,y = round(2Ix,y - Bx,y) indica que o valor da imagem nítida é obtido subtraindo duas versões diferentes da imagem. E a multiplicação por 2 que vem antes da subtração indica que a imagem original
  precisa ser amplificada antes da subtração. Logo, nao tem um unico kernel que possa ser usado para calcular toda a imagem nítida com uma única correlação, seria necessario realizar a operação de nitidez usando
  a subtração de uma versão borrada da imagem original.
  
### Questão 6:

O karnel x, é usado para calcular a derivada aproximada em relação ao eixo x. Ele calcula a diferença de um pixel pro outro na horizontal e destaca as bordas verticais na imagem.
ja o kernel y, é usado para calcular a derivada mais aproximada em relação ao eixo y. E calcula a diferença de um pixel para o outro na direção vertical, destacando as bordas horizontais.

![alt text](https://github.com/Thomazi/pset1_abrantes/blob/main/construcao.png)
  



