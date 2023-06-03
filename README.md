# Projeto-interactive-card-metor-

## fotos do projeto![2023-06-03](https://github.com/marcosaureliosl/projeto-interactive-card-metor-/assets/127764997/1c9611fd-af15-49ce-ada1-73ecc713da77)
![2023-06-03 (1)](https://github.com/marcosaureliosl/projeto-interactive-card-metor-/assets/127764997/a13fc6b9-45f0-4b62-a4e8-3af9a41cff40)
![2023-06-03 (2)](https://github.com/marcosaureliosl/projeto-interactive-card-metor-/assets/127764997/59d891fb-d7a6-4b8a-82fc-2fe3b9f6f73e)

##

## O que é o projeto?

È um desafio, criar este formulário interativo de detalhes do cartão e deixá-lo o mais próximo possível do design.

Que pode usar qualquer ferramenta que desejar para ajudá-lo a concluir o desafio. 

O que deve ser capazes de fazer no Projeto?

- Preencha o formulário e veja a atualização dos dados do cartão em tempo real
- Receba mensagens de erro quando o formulário for enviado se:
  - Qualquer campo de entrada está vazio
  - O número do cartão, data de validade ou campos CVC estão no formato errado
- Veja o layout ideal dependendo do tamanho da tela do dispositivo
- Veja os estados de focalização, ativo e foco para elementos interativos na página

# Demo do Projeto

[Clique aqui](https://marcosaureliosl.github.io/projeto-interactive-card-metor-/) para visualizar o desafio.

[Clique aqui](https://github.com/marcosaureliosl) meu GitHub.


# O que aprendi de novo!

```html
<input
  oninput="if (this.value.length > this.maxLength) this.value = this.value.slice(0, this.maxLength);"
  type="number"
  minlength="2"
  maxlength="2"
  placeholder="AA"
  id="card_year"
  required
/>
```

Este código HTML representa um campo de input para o ano de um cartão, com algumas configurações específicas:

- `oninput` é um evento que é acionado quando o valor do campo é alterado. Neste caso, o código associado a esse evento impede que o valor digitado no campo seja maior do que o valor definido em `maxlength`. Se o valor digitado for maior, o código corta o excesso de caracteres.

- `type="number"` define o tipo de input como numérico, o que significa que apenas números são permitidos no campo.

- `minlength="2"` define o tamanho mínimo do valor que pode ser digitado no campo, nesse caso, 2 caracteres.

- `maxlength="2"` define o tamanho máximo do valor que pode ser digitado no campo, também 2 caracteres.

- `placeholder="AA"` define um texto de exemplo que é exibido dentro do campo antes que o usuário digite algum valor. Nesse caso, o exemplo é "AA".

- `id="card_year"` define um identificador único para o campo, que pode ser usado para manipular ou estilizar o campo através de CSS ou JavaScript.

- `required` indica que o campo é obrigatório e deve ser preenchido pelo usuário antes que o formulário seja enviado.

Essas configurações são úteis ao criar um campo de input para o ano de um cartão, garantindo que o valor digitado seja válido e limitado ao tamanho necessário.




`<input>`: Esta é a tag HTML utilizada para criar um elemento de input.

`oninput="if (this.value.length > this.maxLength) this.value = this.value.slice(0, this.maxLength);"`: Este é um atributo de evento chamado "oninput". Ele especifica o código JavaScript a ser executado quando o valor do campo de input é alterado. Neste caso, o código verifica se o comprimento do valor inserido no campo excede o valor definido em "maxlength" (2 caracteres). Se exceder, o código corta o excesso de caracteres e atualiza o valor do campo.

`type="number"`: Este é um atributo que define o tipo de input. Neste caso, o tipo é definido como "number", o que significa que apenas números serão aceitos no campo.

`minlength="2"`: Este é um atributo que define o tamanho mínimo do valor inserido no campo. Aqui, é definido como 2 caracteres, o que significa que o valor precisa ter pelo menos 2 caracteres.

`maxlength="2"`: Este é um atributo que define o tamanho máximo do valor inserido no campo. Aqui, também é definido como 2 caracteres, o que significa que o valor não pode ter mais de 2 caracteres.

`placeholder="AA"`: Este é um atributo que define um texto de exemplo que será exibido no campo antes que o usuário digite algum valor. Neste caso, o exemplo é definido como "AA".

`id="card_year"`: Este é um atributo que atribui um identificador único ao campo de input. Ele pode ser usado para referenciar o campo em JavaScript ou CSS.

`required`: Este é um atributo que indica que o campo é obrigatório e deve ser preenchido antes de enviar o formulário.

Em resumo, esse trecho de código HTML cria um campo de input numérico com um comprimento mínimo e máximo de 2 caracteres. Ele também tem um texto de exemplo ("AA") que desaparece quando o usuário começa a digitar. Além disso, o campo é obrigatório e possui um identificador único chamado "card_year".

##

```css
input::-webkit-inner-spin-button,
input::-webkit-inner-spin-button {
    -webkit-appearance: none;
    margin: 0;
}
input::placeholder {
    font-family: inherit;
    color: var(--Cinza-violáceo-escuro);
}
input:focus {
    outline-color: hsl(249, 99%, 64%);
}
```

Estas são algumas instruções CSS para estilizar elementos de input em um site. O código remove a aparência padrão do botão de incremento/decremento em campos de input numéricos, define o estilo do texto de placeholder e define a cor do contorno do campo quando está em foco.




Os comandos acima servem para estilizar elementos de input em um site utilizando CSS.

A primeira parte do código, `input::-webkit-inner-spin-button`, é usada para remover a aparência padrão do botão de incremento/decremento em campos de input numéricos. Isso significa que o botão que geralmente aparece ao lado de campos numéricos para permitir ao usuário aumentar ou diminuir o valor não será exibido.

Em seguida, `input::placeholder` é usado para definir o estilo do texto de placeholder, que é o texto que aparece dentro do campo de input antes do usuário digitar algum conteúdo. Nesse caso, o código define que o texto de placeholder deve ter a mesma fonte do restante do conteúdo da página e ter uma cor específica chamada "Cinza-violáceo-escuro".

Por fim, `input:focus` é utilizado para definir o estilo do campo de input quando está em foco, ou seja, quando o usuário clica ou seleciona o campo para digitar algum conteúdo. Nesse caso, o código define que a cor do contorno do campo em foco será uma cor específica determinada pela função `hsl(249, 99%, 64%)`, que representa um tom de azul vívido.

Esses comandos ajudam a personalizar a aparência e o comportamento dos campos de input em um site, proporcionando uma experiência visual mais consistente e agradável para o usuário.

## MInhas Dificuldades 

De novo reforço a parte do JavaScript, realmente é muito complexo e confesso que nessa também tive bastante dificuldade, mais busquei não ser tão geneirico e tentei ser muito fiel ao desafio solicitado.

## Agradecimentos 

Agradecer a todos que sempre estão contribuindo, com ideias e sugestões, e estao sempre me acompanhando nesta jornada

## Meus contatos

Você pode saber mais sobre mim e entrar em contato através do meu site pessoal: [Linkendin](https://www.linkedin.com/in/marcosaureliosl/).

Fique à vontade para entrar em contato comigo através do Twitter: [@MarcosA168484](https://twitter.com/MarcosA168484).

