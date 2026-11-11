# Design de teste — formulário "Adicionar carteira de motorista"

Projeto da Sprint 2 do curso de QA Engineer da TripleTen: análise de requisitos e design de testes para o formulário "Adicionar carteira de motorista" de um serviço de compartilhamento de carros, usando classes de equivalência e análise de valores limite.

## Objetivo

Criar a documentação de teste para os campos do formulário a partir dos requisitos, cobrindo valores válidos, inválidos e os limites de cada campo.

## O que foi feito

- **Classes de equivalência** para três campos:
  - **Nome** e **Sobrenome**: comprimento de 2 a 14 caracteres, campo vazio, letras latinas, espaço, hífen, outro idioma, números, alfanumérico e caracteres especiais.
  - **Data de nascimento**: dia, mês e ano (de 1880 a 2006), incluindo anos bissextos, meses de 30 e 31 dias e formatos inválidos.
- **Valores limite** para cada intervalo (por exemplo: 1, 2 e 3 caracteres; 13, 14 e 15 caracteres; dia 00, 01 e 32; mês 00 e 13).
- **20 casos de teste** para o campo "Nome", com pré-condição, etapas e resultado esperado (mensagem de erro "Inserir o nome correto" ou ausência de erro).

## Arquivos

- [`classes-de-equivalencia-e-casos-de-teste.xlsx`](classes-de-equivalencia-e-casos-de-teste.xlsx): planilha com duas abas:
  - **Classes de equivalência**: grupo de verificações, nome da classe, limites, dados de teste dentro da classe e nos limites, e classificação (intervalo ou conjunto).
  - **Casos de teste**: ID, nome do caso, pré-condição, etapas e resultado esperado.

## O que aprendi

Neste projeto aprendi a transformar requisitos em testes bem planejados:

- **Análise de requisitos:** entender o que cada campo deve aceitar ou recusar.
- **Design de teste:** usar classes de equivalência e valores limite para cobrir o máximo de situações com o mínimo de testes.
- **Casos de teste:** escrever casos claros, com pré-condição, etapas e resultado esperado.
