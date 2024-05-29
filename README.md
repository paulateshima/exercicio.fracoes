# Exercício Frações (Lógica de Programação)

Acabei de conversar com uma professora de matemática do ensino fundamental. Ela me disse que os alunos estão com dificuldades de aprender frações por falta de exercícios. Para ensinar o conceito de uma fração, são utilizados desenhos parecidos com abaixo:

![image](https://github.com/paulateshima/exercicio.fracoes/assets/170154538/d4aee6b7-5ab6-4cc4-97fa-598a8e08a32e)

Para conseguirmos reproduzir a imagem com o exemplo da professora, vamos verificar algumas dicas e requisitos para construirmos nosso código:

Escreva uma função desenhaQuadrado, que recebe x, y, o tamanho e a cor. Cada quadrado desenhado deve utilizar um stroke.

```
function desenhaQuadrado(x, y, tamanho, cor) {
    // aqui precisamos usar fillRect, strokeRect, etc 
}
```

Ah, não custa nada explicar rapidamente como desenhar um texto. Para tal existe a função fillText(), que recebe o texto e as coordenadas no ponto em que deve aparecer:

```
pincel.font='20px Georgia';
pincel.fillStyle='black';
pincel.fillText("Qual é a fração?", 50, 30);
```

Assim até podemos criar uma segunda função para desenhar o texto:

```
function desenhaTexto(texto, x , y) {
    var tela = document.querySelector('canvas');
    var pincel = tela.getContext('2d');

    pincel.font='20px Georgia';
    pincel.fillStyle='black';
    pincel.fillText(texto, x, y);    
}

desenhaTexto("Qual é a fração?", 50, 30);
```
Com base no modelo de desenho e as dicas de código acima, vamos ajudar a professora?

