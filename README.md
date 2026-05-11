# Projeto CI/CD com GitHub Actions

Este projeto foi desenvolvido para a disciplina de Teste e Manutenção de Software com o objetivo de demonstrar os conceitos de Integração Contínua (CI) e Entrega Contínua (CD) utilizando GitHub Actions.

## Objetivo

Automatizar a execução de testes sempre que houver alterações no repositório, garantindo maior confiabilidade e qualidade no desenvolvimento do software.

## Tecnologias utilizadas

* Node.js
* Jest
* Git
* GitHub Actions

## Estrutura do projeto

```bash
.github/workflows/ci.yml
soma.js
soma.test.js
package.json
```

## Funcionamento do pipeline

O pipeline foi configurado utilizando GitHub Actions.

Sempre que um `push` é realizado na branch `main`, o GitHub executa automaticamente as seguintes etapas:

1. Baixar o código do repositório
2. Instalar o Node.js
3. Instalar as dependências do projeto
4. Executar os testes automatizados

## Arquivo de workflow

O arquivo responsável pela automação está localizado em:

```bash
.github/workflows/ci.yml
```

## Teste automatizado

O projeto possui um teste automatizado simples utilizando Jest para validar a função de soma.

### Função

```js
function soma(a, b) {
    return a + b;
}
```

### Teste

```js
test('soma 2 + 2', () => {
    expect(soma(2, 2)).toBe(4);
});
```

## Demonstração prática

Durante a apresentação, será demonstrado:

* Pipeline funcionando corretamente
* Falha proposital no código
* Detecção automática do erro
* Correção do problema
* Execução bem-sucedida após correção

## Integrantes

CAIO MOREIRA MARQUES
JOÃO PEDRO CARVALHO DE OLIVEIRA
DAVI TELLES RAVIER
ADENILSON RODRIGUES

## Disciplina

Teste e Manutenção de Software
PUC Minas Betim
