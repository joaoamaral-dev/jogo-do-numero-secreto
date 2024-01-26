# Jogo do Número Secreto

Projeto desenvolvido como parte dos cursos de Lógica de Programação com JavaScript da Alura.

**Link para o Jogo:** [Jogo do Número Secreto](https://jogo-rho-lovat.vercel.app/)

## Descrição

O "Jogo do Número Secreto" é uma aplicação simples desenvolvida em JavaScript que desafia o usuário a adivinhar um número secreto dentro de um intervalo predefinido.

## Funcionalidades Destacadas

- **Transcrição de Texto para Áudio:** Utiliza a biblioteca `responsiveVoice` para transcrever o texto exibido na tela para áudio, proporcionando uma experiência inclusiva.

- **DOM (Document Object Model):** Manipulação eficiente do DOM para exibição dinâmica de mensagens na interface do jogo.

## Como Jogar

1. Acesse o [Jogo do Número Secreto](https://jogo-rho-lovat.vercel.app/).
2. Escolha um número entre 01 e 10.
3. Receba feedbacks sobre a relação do seu chute com o número secreto.
4. Continue tentando até acertar o número secreto.

## Trecho de Código Relevante

```javascript
// Trecho de código relevante para a geração do número aleatório e exibição de texto
let listaDeNumerosSorteados = [];
let numeroLimite = 10;
let numeroSecreto = gerarNumeroAleatorio();
let tentativas = 1;

// ... (código omitido para brevidade)

function exibirTextoNaTela(tag, texto) {
  let campo = document.querySelector(tag);
  campo.innerHTML = texto;
  responsiveVoice.speak(texto, "Brazilian Portuguese Female", { rate: 1.2 });
}

// ... (código omitido para brevidade)
```

## Como Contribuir

Se deseja contribuir para a melhoria do jogo, siga estas etapas:

1. Faça um fork do repositório.
2. Crie uma branch para suas alterações.
3. Faça suas alterações.
4. Abra um pull request.

## Licença

Este projeto está licenciado sob a [Licença MIT](LICENSE).
