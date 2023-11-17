## Entendendo o cubo , teoria básica.
    Os centros do cubo nunca mudam, ou seja as peças que estão no meio do cubo são "fixas", você consegue movimentar todas as outras para que elas possam chegar até a pedra do meio. 
    E essas peças sendo fixas, tem uma "ordem".
    Ex.: O centro branco tem o centro amarelo como "contrário", o  centro verde tem o centro azul e o vermelho tem o centro laranja.

O script abaixo vai ti ensinar/ajudar a montar o cubo por camadas.

    DICA IMPORTANTE. EVITE DE MEXER O CUBO DEMASIADO...


# 1 - Cruz margarida (cruz branca com o meio amarelo)
    Aqui você precisa colocar as pedras brancas de forma a montar uma cruz no amarelo. 
    Não tem um passo a passo especifico, só treino . Utilize a dica de deixar o cubo estável, tente resolver essa parte projetando a pedra amarela para cima e o fundo branco. Nao mexa a base (fundo branco).


# 2 - Cruz branca.
    Após resolver o passo um, vamos transpor as peças para base branca. 
    A peça que está no topo 'branca' tem uma lateral colorida. Verifique a lateral e rotacione o cubo ate essa lateral encontrar seu meio.
    Ex. Topo branco/lateral vermelha. 
        - rotacione o topo ate chegar lateral vermelha com o centro vermelho.
        - Rotacione essa lateral ajustada duas vezes, ou seja , a parte branca/vermelha que estava encima (no amarelo), vai descer para parte branca em baixo, (na duvida verique, mas mantenha a base branca para baixo)
    ex. Topo branco/lateral verde.
        - rotacione o topo ate chegar lateral verde, com o meio verde
        - rotacione essa lateral ajustada duas vezes.
    
    Faça esse procedimento até ter a cruz BRANCA.


# 3 - Fundo branco.
    Com a cruz branca pronta, vamos fazer o passo de montar o fundo branco e montar a primeira camada(parte de baixo do cubo).
    Nesse passo a temos q localizar uma pedra branca/colorida , que está na terceira camada. Caso nao tenha, você irá precisar colocar a pedra nessas posições. 
    DICA: LEMBRE Q VC PODE ROTACIONAR AS PEÇAS PRONTAS QUE ESTAO EMBAIXO, PORÉM VOLTE AS PARA NAO PERDER SEU PONTO DE PARTIDA E SE PERDER NO CUBO.

    SE pedrabranca/colorida na terceira camada:
        - alinhe a parte colorida com o seu meio colorido (vermelho/vermelho)
        - VIRE O CUBO onde a parte branca fique de frente para você
        SE a parte colorida ficou a esquerda.      
            funcao_esquerda()
            - topo anti-horario
            - esquerda horario
            - topo horario
            - esquerda anti-horario
        se a parte colorida ficou a direita.
            funcao_direita()
            - topo horario
            - direita horario
            - topo anti horario
            - direita anti horario
    Repita o procedimento ate ter o fundo branco, e todas as peças da primeira camadas forem iguais  (3 x vermelhas, 3 x laranjas e etc ...)

# 4 - Segunda camada completa
    Bom agora temos um cubo com o fundo branco completo, e a primeira camada também , além da pedra do meio da primeira camada. Vai faltar completar as laterais da segunda camada.

    Procure no topo e terceira camada , nas peças do meio sem tem alguma opção colorida sem a cor 'amarela', exemplo topo azul e lateral laranja.

    Alinhe a cor lateral com o seu meio (no exemplo ficou laranja/laranja e no topo o azul), posicione essa face/frente para vocÊ.
    Com a face do cubo (frente) virada para você, certifique que a peça que está no topo (exemplo aqui é o azul), tenha o seu lado a direita do cubo ou a esquerda.

    SE for a direita:
        funcao_direita():
        - topo horario
        - direita horario
        - topo anti-horario
        - direita anti-horario
        - topo anti-horario
        - face anti-horario
        - topo anti-horario
        - face horario

    SE for a esquerda:
        funcao_esquerda():
        - topo anti-horario
        - esquerda horario
        - topo horario
        - esquerda anti-horario
        - topo horario
        - face horario
        - topo anti-horario
        - face anti_horario
    
    SE o seu cubo não tem nenhuma face sem a parte amarela, você escolhe uma das funções (funcao_esquerda ou funcao_direita), com isso você irá obter um pedra ideal para realizar os movimentos.

# 5 - Passo cruz amarela topo
    funcao_cruz():
        - Face horario
        - Direita horario
        - Topo horario
        - Direita anti-horario
        - Topo anti-horario
        - Face antihorario
    SE- opção ponto no meio amarelo topo:
        funcao_cruz()
    SE- opção L amarelo topo;
        > Colocar o L ao contrario (imagine um relogio, o L ao contrario deve marcar os ponteiros 9 e 12):
        funcao_cruz()
    SE - opção linha amarela topo;
        > Colocar a linha na horizontal;
        funcao_cruz()

# 6 - Passo topo amarelo completo
    funcao()
        - Direita horario
        - Topo horario
        - Direita anti-horario
        - Topo horario
        - Direita horario
        - Topo duplo horario
        - Direita anti-horario
    >> 7 Possibililidade:
    SE - Posição amarela opostas nas diagonais (exemplo quadrante 1 e quadrante 9):
        > Coloque uma frente amarela da face do cubo virada para você e a outra deve ficar a direita do cubo:
        funcao()
    SE - Posição amarela na mesma linha (exemplo quadrante 1 e quadrante 3):
        > Alinhar a esquerda (quadrante 1 e quadrante 6)
        funcao()
    SE - Posição de dois amarelos na FACE:
        > Utilizar a face com os dois amarelos virados para você
        funcao()
    SE - Posição cruz amarela TOPO, face com duas amarelas e fundos com duas amarelas:
        > usar face onde nao tenha as partes AMARELAS
        funcao()
    SE - Posição cruz amarela topo, face com duas amarelas e e outas espalhadas:
        > usar face onde as duas amarelas estejam a esquerda
        funcao()
    SE - Posiçao peixinho sem pedra amarela na face:
        > Posicione o peixe conforme foto.
        funcao()
    SE - Posição peixinho com pedra amarela na face
        > posicione pedra amarela na face
        funcao()

# 7 - Passo - estruturando para o final (TOPO AMARELO PRONTO).
    SE - POSSIBILIDADE (Duas quinas iguais):
	> Colocar as duas quinas para baixo, e frente face amarela:
	funcao()
	 - Direita horario
	 - Topo antihorario (amarela atras)
	 - Direita horario (as amarelas tendem a separar), 
	 - base dupla horario 
	 - Direita anti horario
	 - Topo horario (tres amarela)
	 - Direita horario
	 - Base dupla horario
	 - direita duplo.

    Assim vamos ter duas quinas iguais para todos os lados, deixarem proximo das cores.(ir passo 8)


    SE - POSSIBILIDADE (Quinas diferentes):
 	> Colocar duas quinas para baixo, onde a frente fica com a face amarela:
	funcao()


# PASSO 8 - FINALIZANDO O CUBO (DUAS POSSIBILIDADE):
    SE - POSSIBILIDADE  (3 MEIOS ERRADOS ):
	> POSICIONE O LADO CORRETO ATRAS DA FACE:
		- FACE DUPLA HORARIA
		- IDENTIFICAR COR DA FACE.
		SE MEIO ESTIVER PARA DIREITA:
		- TOPO HORARIO (OBSERVAR ALINHAMENTO DE COR)
		funcao()
		- ESQUERDA ANTI HORARIO
		- DIREITA ANTI HORARIO
		- FACE DUPLO HORARIO
		- ESQUERDA HORARIO
		- DIREITA HORARIO
		- TOPO HORARIO
		- FACE DUPLO
		
		SE MEIO ESTIVER PARA ESQUERDA:
		- TOPO ANTI HORARIO (ALINHAMENTO DE COR)
		funcao()

    SE - 4 MEIOS ERRADOS.
	funcao()
	cair na primeira possibilidade.