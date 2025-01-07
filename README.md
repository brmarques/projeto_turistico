# Desafio prático - Local Turístico

## Introdução

Faaaaaaala, dev! Parabéns por chegar até aqui! 💜
Chegou a hora de aplicar toda a teoria que você aprendeu até aqui colocando a mão na massa!
Este é o momento de transformar conhecimento em ação, desenvolvendo um projeto que vai consolidar suas habilidades e te preparar um pouco mais para os desafios reais!

Vamos lá? 🚀

Você vai desenvolver uma página web com informações sobre um determinado local turístico.

## Descrição do desafio

![Thumbnail.png](https://prod-files-secure.s3.us-west-2.amazonaws.com/08f749ff-d06d-49a8-a488-9846e081b224/86c8ae46-7958-4e40-bbaa-7aa3d54f1250/Thumbnail.png)

<aside>
💜 [Acesse o **link** do Figma aqui.](https://www.figma.com/community/file/1384542229391733447/local-turistico)

</aside>

Nessa aplicação você vai trabalhar com:

<aside>
<img src="/icons/checkmark-line_purple.svg" alt="/icons/checkmark-line_purple.svg" width="40px" /> Estrutura HTML;

</aside>

<aside>
<img src="/icons/checkmark-line_purple.svg" alt="/icons/checkmark-line_purple.svg" width="40px" /> Estilizações com CSS;

</aside>

<aside>
<img src="/icons/checkmark-line_purple.svg" alt="/icons/checkmark-line_purple.svg" width="40px" /> Fontes;

</aside>

<aside>
<img src="/icons/checkmark-line_purple.svg" alt="/icons/checkmark-line_purple.svg" width="40px" /> Espaçamentos;

</aside>

<aside>
<img src="/icons/checkmark-line_purple.svg" alt="/icons/checkmark-line_purple.svg" width="40px" /> Imagens;

</aside>

<aside>
<img src="/icons/checkmark-line_purple.svg" alt="/icons/checkmark-line_purple.svg" width="40px" /> Listas desordenadas;

</aside>

<aside>
<img src="/icons/checkmark-line_purple.svg" alt="/icons/checkmark-line_purple.svg" width="40px" /> Alterações das cores dos textos;

</aside>

<aside>
<img src="/icons/checkmark-line_purple.svg" alt="/icons/checkmark-line_purple.svg" width="40px" /> Alterações dos pesos dos textos;

</aside>

## Dicas

Boa parte do que você vai precisar para resolver este desafio foi apresentado em aula e é super normal ter que assistir novamente alguns desses conteúdos enquanto desenvolve o projeto, portanto use bastante as aulas para revisar os conteúdos.

Mas claro que desafios podem apresentar alguns conteúdos ainda não vistos, mas não se preocupe que você pode pesquisar e usar as documentações para te ajudar a resolver seu projeto, bem como também pode tirar dúvidas no fórum.

Caso precise de mais ajuda, criamos essa sessão com algumas dicas e possíveis dúvidas que você pode encontrar neste desafio, mas lembre-se sempre tente resolver o desafio antes de olhar esses pontos. 

### Ajustar tamanho da imagem para ocupar o tamanho do container

Para que a imagem não fique gigante na página e ocupe apenas o tamanho de tela disponível você pode usar a propriedade `width: 100%;`

Ex.:

```css
img {
  border-radius: 28px;  /* Adicionar o arredondamento da borda */
  width: 100%; /* imagem ocupa 100% do tamanho disponível pra ela */
}
```

Criar a linha de divisão (divider)
Existem várias formas de criar e estilizar essa linha

Um exemplo de como pode ser feito:
No HTML você pode criar uma div com class divider (lembrando que pode ser qualquer nome)
<div class="divider"></div>
​
No CSS você pode adicionar os estilos:
.divider {
  width: 100%;
  height: 1px;
  margin: 36px 0;
  background-color: #d9d9d9;
}


Lembrando que se você fez de outra forma não quer dizer que fez errado, como mencionado acima existem várias formas de criar este elemento.

### Adicionar negrito e letras maiúsculas no texto?

Para modificar o peso da fonte você pode usar a propriedade `font-weight`, no caso do negrito pode usar o valor `bold` .

Para transformar o texto em maiúsculo sem ter que digitar todas as letras em maiúsculo, você pode usar a propriedade e valor `text-transform: uppercase;` 

Ex.:

```css
.headline {
  font-size: 16px;
  line-height: 22px;
  font-weight: bold; /* a fonte fica em negrito */
  color: #e1624f;
  text-transform: uppercase; /* a fonte fica com todas as letras em maiúsculo */
}
```

→ [Documentação font-weight](https://developer.mozilla.org/en-US/docs/Web/CSS/font-weight)

→ [Documentação text-transform](https://developer.mozilla.org/en-US/docs/Web/CSS/text-transform)

### Mudar estilo da fonte para itálico

Para mudar o estilo da fonte, você pode usar a propriedade do CSS `font-style`

Ex.:

```css
.subtitle {
  font-size: 16px;
  line-height: 22px;
  font-style: italic; /* Muda estilo da fonte para itálico */
  text-align: center;
  color: #333333;
  margin-top: 24px;
}
```

Lembrando que deve adicionar essa opção quando busca a fonte no Google Fonts

![Captura de Tela 2024-06-17 às 12.40.24.png](https://prod-files-secure.s3.us-west-2.amazonaws.com/08f749ff-d06d-49a8-a488-9846e081b224/d9625129-b656-4c7d-86c3-cc4de96b2862/Captura_de_Tela_2024-06-17_as_12.40.24.png)

```html
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Open+Sans:ital,wght@1,300..800&display=swap" rel="stylesheet">
```

Você pode usar este código para importar a fonte no seu projeto.

### Corrigir imagem distorcida

Em alguns casos quando ajustamos a altura da imagem ela pode ficar um pouco distorcida.

Isso pode acontecer no caso das imagens dessa sessão:

![Captura de Tela 2024-06-17 às 12.43.54.png](https://prod-files-secure.s3.us-west-2.amazonaws.com/08f749ff-d06d-49a8-a488-9846e081b224/e378a218-c849-4b83-9f47-befcf5db345e/Captura_de_Tela_2024-06-17_as_12.43.54.png)

Uma forma de corrigir esse problema é adicionar a propriedade `object-fit` no CSS dessa imagem.

Ex.:

```css
main div img {
  height: 375px;
  object-fit: cover; /* Ajusta a proporção da imagem para caber no container disponível pra ela sem distorcer */
  margin-top: 44px;
}
```

→ [Documentação object-fit](https://developer.mozilla.org/pt-BR/docs/Web/CSS/object-fit)

### Bullet da lista com cor diferente do texto

Se você notar bem, neste desafio vai ver que o bullet da lista tem uma cor diferente da cor do texto.

![Captura de Tela 2024-06-17 às 12.49.19.png](https://prod-files-secure.s3.us-west-2.amazonaws.com/08f749ff-d06d-49a8-a488-9846e081b224/3f7a5e7d-6a23-47c9-ba9d-cf86a78c36a7/Captura_de_Tela_2024-06-17_as_12.49.19.png)

Uma forma de resolver isso é usar o `::marker` que é um pseudo-elemento, mas não se preocupe, você ainda vai aprender sobre isso nos módulos futuros, por hora, pode usar a dica abaixo:

```css
ul li::marker {
  color: #333333;
}
```

→ [Documentação ::marker](https://developer.mozilla.org/en-US/docs/Web/CSS/::marker)

## Entrega

Após concluir os exercícios desse desafio, você deve enviar o link do seu código no GitHub para a plataforma. 

Após concluir o desafio, se você se sentir confortável, o que acha de postar no LinkedIn 
contando como foi a sua experiência compartilhando o seu projeto e o seu aprendizado?
É uma excelente forma de demonstrar seus conhecimentos e atrair novas oportunidades! 👀

E pode marcar a gente, viu? Vai ser incrível acompanhar toda a sua evolução! 💜

---

## Considerações finais

Lembre-se que o intuito de um desafio é te impulsionar, por isso, dependendo do desafio, pode ser que você precise ir além do que foi discutido em sala de aula. 
Mas isso não é algo ruim: ter autonomia para buscar informações extras é uma habilidade muito valiosa e vai ser ótimo pra você treinar ela aqui com a gente!

E lembre-se: **tenha calma**! Enfrentar desafios faz parte do seu processo de aprendizado! 

Se precisar de alguma orientação ou suporte, estamos aqui com você!
Bons estudos e boa prática! 💜
