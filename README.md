# Calculadora de Estatística

Calculadora de **tamanho da amostra** e **intervalo de confiança** feita para a disciplina de Estatística Aplicada.

É uma página só (`index.html`), com HTML, CSS e JavaScript puros: sem frameworks e sem instalação. Para usar, basta abrir o arquivo no navegador.

## Abas

1. **Tamanho da amostra – Média**: n = (zα/2 · σ / Em)²
2. **Tamanho da amostra – Proporção**: n = zα/2² · p(1 − p) / Ep² (com a opção "p desconhecido", que usa 50%)
3. **Intervalo de confiança – Média**: Em = zα/2 · σ / √n e IC = (x̄ − Em ; x̄ + Em)
4. **Intervalo de confiança – Proporção**: Ep = zα/2 · √(p(1 − p) / n) e IC = (p − Ep ; p + Ep), com comparação opcional com um padrão aceitável
5. **Diminuir o erro**: novo erro, novo tamanho da amostra e quanto a amostra precisa aumentar

Cada aba mostra a fórmula (escrita à mão, com uma versão "em palavras" embaixo; passar o mouse ou tocar numa letra mostra o que ela significa), a legenda explicando cada letra, o passo a passo com os números e a resposta final em uma frase. O menu "Carregar exemplo" traz os exercícios da aula.

O botão **? Fórmulas**, no canto da tela, abre uma janela com todas as fórmulas, a tabela de valores críticos e as regras principais.

## Regras usadas

- Grau de confiança: 90% → zα/2 = 1,645 | 95% → zα/2 = 1,96 | 99% → zα/2 = 2,575
- Aceita vírgula como separador decimal
- Tamanho da amostra sempre é arredondado para cima
- Intervalos mostram o valor exato (4 casas) e o arredondado (2 casas)

## Publicação

O site fica em https://guilhermeoliveira0.github.io/calculadora-estatistica/ e é publicado sozinho pelo workflow `.github/workflows/publicar-pages.yml` a cada push na branch `main`. Para publicar de novo sem mudar nada, use o botão "Run workflow" na aba Actions.

## Arquivos

- `index.html`: a calculadora
- `prototipo.html`: o protótipo visual feito antes da implementação
- `prototipo-formulas.html`: o protótipo dos 3 estilos de fórmula escrita à mão (o escolhido foi "folha branca")
