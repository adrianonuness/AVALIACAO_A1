# AVALIACAO_A1

Nessa avaliação, foi solicitado que seja feito 4 tipos de programas, sendo cobrado as seguintes estruturas:
-
* ESTRUTUTAS CONDICIONAIS:
* ESTRUTURAS DE REPETIÇÃO:
* LISTAS
* DICIONÁRIOS

O QUE FOI FEITO EM CADA UM:
-
# 1. ESTRUTURAS CONDICIONAIS:

Eu resolvi elaborar um jogo simples que eu já estava testando: pedra, papel, tesoura. Como o jogo funciona com condições de escolha
para que o usuário vença ou perca, achei que seria perfeito usá-lo para suprir a estrutura cobrada.

O código começa importando a biblioteca random, que permite que o computador escolha aleatoriamente entre “pedra”, “papel” e “tesoura”, 
opções que são armazenadas em uma lista. Em seguida, um loop while True é usado para manter o jogo rodando continuamente. A cada rodada, o usuário
digita sua escolha, enquanto o computador escolhe uma opção da lista de forma aleatória. A entrada do usuário é convertida para letras minúsculas
usando .lower() para evitar erros caso ele digite com maiúsculas.
Se o usuário digitar algo diferente das opções válidas e não pedir para sair, o programa informa que a opção é inválida.
Caso ele digite “sair”, o jogo é encerrado. Depois, o código compara as escolhas: se forem iguais, ocorre um empate; se o usuário estiver em uma das combinações vencedoras, o programa informa que ele venceu; em qualquer outro caso, o computador é declarado vencedor.

# 2. ESTRUTURAS DE REPETIÇÃO:

Nesse eu segui a sugestão de tarefa, que era desenvolver um contador de 1 a 100 com for e outro com while, exibindo apenas números pares.

O código apresenta duas formas de exibir apenas os números pares de 1 a 100. Na primeira parte, usando o laço for, é utilizado um range(2, 101, 2), que começa em 2, vai até 100 e avança de 2 em 2, garantindo que só números pares sejam impressos. Cada valor gerado pelo range é exibido com um print(i).

Na segunda parte, o mesmo objetivo é alcançado com um laço while. Primeiro, o contador é iniciado com o valor 2. Enquanto esse contador for menor ou igual a 100, o programa verifica se ele é par usando contador % 2 == 0, o que confirma se o número tem resto zero quando dividido por 2. Se for par, ele é exibido. Após cada repetição, o contador é incrementado com contador += 1 até atingir o valor 100.

# 3. LISTAS:

A sugestão foi criar um programa que receba nomes de alunos e armazene em uma lista, permitindo exibir todos os nomes ao final.

O programa começa criando uma lista vazia chamada alunos, que servirá para armazenar os nomes digitados pelo usuário. Em seguida, utiliza um loop while True, que mantém o programa pedindo novos nomes continuamente até que uma condição de parada aconteça. A cada repetição, o usuário digita um nome; caso ele simplesmente pressione Enter sem escrever nada, o programa executa o break, encerrando o loop. Sempre que um nome válido é digitado, ele é adicionado à lista utilizando o método .append(). Ao final, o programa imprime a mensagem “Lista dos alunos informados:” seguida da lista completa com todos os nomes cadastrados.

# 4. DICIONÁRIOS:

E por fim, nesse último a sugestão foi desenvolver um sistema simples de cadastro de produtos com nome e preço, armazenando em dicionário.

O programa começa criando um dicionário vazio chamado produtos, que será usado para armazenar cada item cadastrado no formato nome: preço. Em seguida, um loop while True é usado para permitir que o usuário cadastre vários produtos continuamente. A cada passagem do loop, o usuário digita o nome do produto. Se apenas pressionar Enter, o break é acionado e o cadastro é encerrado. Caso um nome válido seja informado, o programa solicita o preço do produto e o converte para número com float(). Em seguida, o nome e o preço são armazenados dentro do dicionário por meio da atribuição produtos[nome] = preco. A cada cadastro concluído, uma mensagem confirma a operação. Ao final do loop, o programa exibe todos os produtos cadastrados imprimindo o dicionário completo.
