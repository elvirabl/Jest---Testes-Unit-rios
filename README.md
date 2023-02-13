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

O que são testes?

Porque devo usar os testes?

O que são testes unitários?

Agora que já sei os porquê´s, bora instalar nosso Jest.

Sua API está prontinha? Tudo rodando Gostozinho?

Como instalar o Jest?
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


Como rodar o Jest?

Por fim, execute no terminal do VS Code: npm run test e o Jest irá imprimir a seguinte mensagem:

PASS  ./exemplo.test.js
✓ adds 1 + 2 to equal 3 (5ms)

Como ler o resultado do Jest?

Conclusão:
Jest é uma beleza, uma SUPER ferramenta que deve andar sempre de mãos dadas com o bom profissional.

Agradecimento:
A toda equipe Reprograma, a professora Sra. Louise Costa, a minha amiga Greice Pereira Giacomelli, a todas as Devas da minha turma.
Agradeço a Grande Deusa por me manter num caminho reto. Desejo a todos que chegaram até aqui muita saúde e prosperidade. Que assim se faça!




