# Jest para iniciantes - Testes Unitários

## Ele tem cara de malvadão, temperamento de malvadão, sente o bad smell a kilometros de distância...

![image](https://user-images.githubusercontent.com/109379404/218550620-b6e3ba73-5b0d-49ef-b96c-a5b79a46968e.png)

## mas na verdade, ele é o Good Doctor

![image](https://user-images.githubusercontent.com/109379404/218551273-3a956590-0b9f-49b3-8745-c11df45b06b9.png)

### O melhor jeito de aprender é ensinar!!!

Inicio meu texto, com a melhor das intensões. Sou Elvira Bruno, ex aluna Back end, Reprograma, turma On 19, e tive muita dificudade em entender TESTES.
Espero ajudar as colegas que tiveram ou terão as mesmas dificuldades.

![image](https://user-images.githubusercontent.com/109379404/218554841-31b3ef85-6d92-45cc-84f6-94c482e3c672.png)

Lest´s Bora!

#### TESTES UNITÁRIOS

O que são testes?<br />
Teste são os resultados da análise da API.<br />
Por exemplo, para sabermos se nosso nível de insulina está OK, devemos realisar um teste de Glicose, onde o resultado tem que ser entre 80 e 100.<br />
Se ocorre alguma alteração, devemos consultar um médico (DEV) e tomar as providências necessarias.<br />
Assim acontece no resultado do teste, no nosso caso a ferramenta Jest.
<br />
<br />**Porque devo usar os teste?**<br />
ERROS acontecem com frequência e para termos a certeza de que tudo está certinho, seguro e saudável devemos escrever testes.<br />
<br />Os erros mais comuns são:
* Falta de atenção
* Falha na comunicação do time
* Versões de bibliotecas e frameworks desatualizados

**Devemos sempre nos atentar aos princípios**
* QUALIDADE - ter um código limpo e funcional 
* CONFIANÇA - confiar na equipe e no código
* TEMPO - economia de tempo e dinheiro

**Pensando em Testes:**
* 1º Analise de Requisitos  (levantamento de autorizações e solicitações)
* 2º Plano de testes (definição de estrutura, ferramentas e nível em que iremos chegar)
* 3º Caso de teste (mapa de comportamento esperado, cenários de stress do código)
* 4º Ambiente  de teste (DEV, homologação com todas as partes envolvidas e aplicação)
* 5º Implementação (Quando está tudo OK, bora rodar)

**Pirâmide de testes:**<br />
Os testes unitários estão na base da pirâmide de teste, e a ferramenta aqui aplicada está ligada a esse nível num ambiente DEV, o restante dessa pirâmide, trataremos nos próximos artigos.<br />
A pirâmide se compôem em 3 níveis:<br />
**TESTES UNITÁRIOS** ( testes curtos e isolados, Analisa função ou método, Rápido e de baixo custo *ConsoleLog*)
*NÃO GARANTE UMA INTEGRAÇÃO PERFEITA DOS MÓDULOS<br />
**INTEGRAÇÃO** (testes de rotas e requisições, se comunica facilmente com módulos e elimina bugs e alterações de código, maior custo e mais demorado *MongoDB*)
*NÃO ANALISA TODO O FLUXO DA APLICAÇÃO<br />
**E2E** (chamado de Ponta a Ponta, Teste de alto nível, analisa TODOS os módulos e staks)
*MUITO LENTO E DE CUSTO ELEVADO<br />

**Agora que já sei os porquê´s, bora instalar nosso Jest.**

Sua API está prontinha? Tudo rodando legalzinho?

**Como instalar o Jest?**<br />
Abra um terminal no seu VS Code

Digite o comando:
npm install --save-dev jest

Adicione a seguinte seção ao seu package.json:
{
  "scripts": {
    "test": "jest"
  }
}

Exemplo:
Vamos começar por escrever um teste para uma função hipotética que soma dois números.
Primeiro, crie um arquivo exemplo.js:

function exemplo(a, b) {
  return a + b;
}
module.exports = exemplo;

Em seguida, crie um arquivo chamado exemplo.test.js. Este aquivo irá guardar o nosso teste real:

const exemplo = require('./exemplo');

test('adds 1 + 2 to equal 3', () => {
  expect(exemplo(1, 2)).toBe(3);
});


**Como rodar o Jest?**

Por fim, execute no terminal do VS Code: npm run test e o Jest irá imprimir a seguinte mensagem:

PASS  ./exemplo.test.js
✓ adds 1 + 2 to equal 3 (5ms)

**Como ler o resultado do Jest?**<br />
O Bom mora aqui, o Jest mostra a falha, caminho de onde ela está o erro e possível alteração pra conserto.
Tudo de maneira bem fácil e colorida, tipo vermelho para erro e verde para sucesso.

Conclusão:
Jest é uma beleza, uma SUPER ferramenta que deve andar sempre de mãos dadas com o bom profissional.

Agradecimento:<br />
A toda equipe Reprograma, a professora Sra. Louise Costa, a minha amiga Greice Pereira Giacomelli, a professora Sra. Tereza Oliveira e a todas as Devas da minha turma.<br />
Agradeço a Grande Deusa por me manter num caminho reto. Desejo a todos que chegaram até aqui muita saúde e prosperidade. Que assim se faça!




