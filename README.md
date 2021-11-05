                                      O que é turtle?
    Turtle é uma biblioteca que é usada no python para desenhos mais em tempo real, para ficar mais "bonitinho".
Essa ferramenta de desenho, introduzida pelo professor nas aulas de "Turtle Confusion", usa o sistema do canvas e 
o sistema de ordenadas de "x" e "y" em que originam o centro da tela do usuário, e através desse sistema vamos ro-
dar as tartarugas. 
    Todas tartarugas iniciam no centro do nosso sistema de ordenadas e podem ser movimentadas com os comandos "right(n)",
"left(n)" e "forward(n)", todos com referêncial novo estando na tartaruga para andar a quantidade de pixeis "n". Além 
disso, temos módulos bases do turtle, o próprio ".circle(n)" que faz um desenho do círculo com "n" sendo o seu raio.
    Mas, sempre digo tartarugas, por que tartarugas?? O símbolo da caneta no turtle, padrão, é uma pequena tartatuga
que sai desenhando por aí o que você pedir! Mas se você não é fã de tartarugas, podemos mudar para seta ".shape("arrow")", 
círculo".shape("circle")", quadrado ".shape("square")".. ou até não deixar nada marcado como a caneta e deixar um espaço 
em branco".shape("blank")".
    Com isso feito, podemos mudar a cor das suas linhas com o comando ".pencolor("cor")", com cor com a primeira letra em
maiúsculo. (link das cores no final da apresentação)

    Ok! Temos uma base para assim irmos "testar" um código e apresentar mais alguns comandos essenciais!!
{
    #cada código turtle tem de começar com o import, para importarmos a biblioteca#
import turtle

caneta = turtle.Turtle() #definição da caneta

caneta.shape("turtle") #escolhemos assim o formato da caneta como uma tartaruga

caneta.fillcolor("Green") #a cor da minha tartaruga vai ser verde

caneta.speed (5) #altera a velocidade da nossa tartaruga para podermos ver bem ela!

tela = turtle.Screen() #determinamos a tela 

tela.bgcolor("Cyan") #mudamos a cor da tela de fundo para um ciano; bg = background = tela de fundo


for step in range(0, 90): #desenha o círculo em 3 voltas
    caneta.forward(10) #anda 10 pixeis pra frente
    caneta.left(4) #anda 4 pixeis pra cima

    if step % 10 == 0: #a cada 20 passos, vamos marcar a tartaruga no desenho
        caneta.stamp() #assim marcamos a tartaruga!

turtle.done() #código feito, vamos testar??
}

Obs.: para usar no VsCode, no windows, usar o comando "Pip3 install turtle" para poder começar a brincar com ele.
link para as cores: https://trinket.io/docs/colors
