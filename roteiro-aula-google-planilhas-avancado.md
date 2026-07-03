# Roteiro de Aula — Google Planilhas Avançado

> **Projeto Extensionista Integrado — UFES**
> Aula prática de uso avançado do Google Planilhas: Google Forms, páginas, fórmulas e gráficos.

---

## 1. Informações gerais

| Item | Descrição |
|------|-----------|
| **Tema** | Uso avançado do Google Planilhas |
| **Público** | Pessoas que já sabem o básico de Google Planilhas (criar planilha, preencher células, formatar) |
| **Duração** | 2h |
| **Formato** | Presencial em laboratório OU online com compartilhamento de tela |
| **Pré-requisito mínimo** | Ter uma conta Google/Gmail e conhecimento básico de planilhas (equivalente ao roteiro introdutório) |

### Objetivos de aprendizagem
Ao final da aula, você será capaz de:
1. Criar um Google Forms e vinculá-lo a uma planilha de respostas.
2. Organizar as respostas recebidas em múltiplas páginas (abas) dentro de uma mesma planilha.
3. Usar fórmulas mais avançadas sobre os dados coletados: SE, SOMASE/SOMASES, CONT.SE/CONT.SES, PROCV e referências absolutas.
4. Criar e personalizar gráficos a partir dos dados de respostas.

---

## 2. Avisos iniciais para a turma

1. **A aula é focada na prática.**
2. **Sinta-se à vontade para explorar.**
3. **Não tenha medo de errar — planilhas têm Ctrl+Z.**
4. **Pergunte a qualquer momento.**

---

## 3. O que você vai precisar

- Computador/notebook com internet.
- Conta Google/Gmail (institucional, quando disponível).
- Nada mais! Google Planilhas e Google Forms funcionam pelo navegador, sem instalação.

---

## 4. Passo a passo

### Bloco 0 — Revisão rápida (5 min)

0. Entrar na conta institucional.
1. Relembrar rapidamente: célula, linha, coluna, página/aba, formatação básica.

---

### Bloco 1 — Google Forms

0. Enviar a planilha da aula introdutória para a conta institucional.
1. Abrir a planilha da aula introdutória
   - 1.1 Relembrar do que se trata a planilha
   - 1.2 Criar página/aba
   - 1.3 Deletar página/aba
2. Abrir o Google Drive em uma nova aba
   - 2.1 Desafio: criar formulário
3. Respostas > Link para as Planilhas
   - 3.1 Selecionar planilha da aula
   - 3.2 Observação importante: será criada sempre uma nova página
4. No formulário adicionar campos relacionados com a planilha da aula introdutória
   - 4.1 Desafio: como adiciona nova pergunta?
   - 4.2 Desafio: sexo é qual tipo de resposta?
   - 4.3 Desafio: conferir a planilha sendo alterada
   - 4.4 Desafio: pergunta obrigatória?
   - 4.5 Desafio: Idade texto livre ou multipla escolha?
5. Visualizar planilha (ver andamento)
   - 5.1 Não é possível enviar a resposta de fato
6. Publicar o formulário
   - 6.1 Desafio: url curto
7. Formatar página de respostas na planilha
   - 7.1 Desafio: congelar colunas
   - 7.2 Desafio: excluir excesso de linhas e colunas

---

### Bloco 2 — Fórmulas

1. Clonar planilha do professor "Aula - Planilha avançada"
   - 1.1 Há vários itens já cadastrados
2. Criar uma página nova
   - 2.1 Desafio: renomear a nova página para "Fórmulas"
3. Se não tiver preenchido, preencher:
   - 3.1 De A1 até A6 escrever 12, 14, 16, 19, 22
   - 3.2 De B1 até B6 escrever 18, 10, 17, 15, 19
4. Na célula A7 escrever: =1+2
5. Na célula A7 mudar para =MAIOR(A1:A5; 1)
   - 5.1 Nomes das funções em inglês?
      - 5.1.1 Opcional: Arquivo > Configurações > Sempre usar os nomes de funções em inglês
   - 5.2 Desafio: o que o 1 no final faz?
   - 5.3 Desafio: trocar MAIOR para MENOR
   - 5.4 Desafio: e se fosse A1:A3?
   - 5.5 Desafio: e se fosse A1:B5?
   - 5.6 Perceber a seleção que mostra quando o cursor está no intervalo da fórmula
6. Intervalos
   - 6.1 Deixar A7 =MENOR(A1:A5; 1), copiar a célula com a fórmula, colar na B7
   - 6.2 Desafio: por que o intervalo mudou?
   - 6.3 Desafio: intervalo relativo A1:A5 vs absoluto $A$1:$A$5
   - 6.4 Desafio: e se recortar em vez de copiar?
   - 6.5 Desafio: intervalo sem fim? =SOMA(A1:A)
   - 6.6 Desafio: dependência circular, =SOMA(A1:A) => #REF!
7. Fórmula entre páginas
   - 7.1 Apague completamente a página de Fórmulas
   - 7.2 Renomeie a página para Estatísticas
   - 7.3 A1 "Maior idade", B1 =MÁXIMO(Educandos!D:D)
   - 7.4 Desafio: Menor idade
   - 7.5 A3 "Quantidade Meninos", B3 =CONT.SE(Educandos!C:C; "M")
   - 7.6 Desafio: Quantidade Meninas
   - 7.7 A5 "Média moradores por domicílio", B5 =MED(Educandos!G:G)
   - 7.8 Desafio: "Quantidade Turno M" e "Quantidade Turno V"

---

### Bloco 3 — Gráficos

1. Na página Educandos, selecione toda planilha, Inserir > Gráfico
   - 1.1 Ignorando o que o gráfico faz por enquanto
   - 1.2 Perceba que o gráfico está tapando os dados
   - 1.3 No "Editor de gráficos", perceba "Intervalo de Dados"
2. Crie uma nova página, renomeie para Gráficos
3. Inserir > Gráficos
   - 3.1 Intervalo de dados: "Educandos!A:G"
   - 3.2 Perceba que mudou para um intervalo definido
   - 3.3 Eixo X: idade, Marcar "Agregar"
   - 3.4 Usar linha 1 como cabeçalho (não é um dado)
   - 3.5 Gráficos sugeridos
4. Abrir edição de gráfico: dois cliques no gráfico
