# Diagnóstica em Foco

Painel interativo da **Avaliação Diagnóstica de Entrada do 2º semestre de 2026**, cruzada com a **Prova Paulista**, o **Mapa de Habilidades SARESP 3EM** e o **Plano de Ensino Semestral**.

Ensino Fundamental — Anos Finais. 373 estudantes avaliados, 13 turmas, 96 itens, 45 habilidades e 32 Aprendizagens Essenciais.

## Como abrir

Baixe o repositório e abra `index.html` no navegador — é um arquivo único, sem dependências de build. As fontes vêm do Google Fonts; sem internet, a página cai para a pilha de fontes do sistema e continua legível.

Não publique via GitHub Pages — veja a seção de privacidade abaixo.

## As três camadas

O painel é organizado pela hierarquia real de decisão da escola. Os filtros do topo — segmento, componente e turma — valem para todas as camadas ao mesmo tempo.

**Camada 1 · Estratégica — direção e gestão**
Proporção de estudantes em Adequado ou Avançado, distribuição pelos quatro níveis nas duas medidas do semestre, matriz de transição entre níveis, posição de cada turma na Prova Paulista e na Diagnóstica, e as turmas que exigem intervenção.

**Camada 2 · Tática — coordenação pedagógica**
Ranking das habilidades SARESP da mais frágil à mais consolidada, a tabela Plano de Ensino × Diagnóstica com a situação e o encaminhamento de cada Aprendizagem Essencial, e a variação por componente entre as duas medidas.

**Camada 3 · Operacional — professor e sala de aula**
Mapa de calor questão a questão por turma, os itens abaixo de 40% de acerto detalhados, os grupos de recuperação e a tabela completa de estudantes com busca, filtro por nível e ordenação.

## Leitura dos dados

O corte de leitura dos itens e habilidades é **60% de acerto**; abaixo de 40% o item entra como crítico. Os níveis seguem as faixas da rede: Abaixo do Básico 0–25%, Básico 26–50%, Adequado 51–75%, Avançado 76–100%.

As duas medidas do semestre **não são equivalentes**. A Prova Paulista foi aplicada antes e cobre todos os componentes curriculares — a medida comparável aqui é o recorte de Língua Portuguesa e Matemática. No 6º e no 7º ano o Livro 1 da Diagnóstica é mais acessível que a Prova Paulista, então parte do avanço nesse segmento é efeito do instrumento, não apenas de aprendizagem. No 8º e no 9º ano as duas provas têm dificuldade semelhante, e ali o movimento pode ser lido como avanço ou recuo real.

Dois achados que o cruzamento torna explícitos:

- **79,9%** dos estudantes de 6º e 7º ano estão em Adequado ou Avançado, contra **49,5%** no 8º e 9º ano.
- **As sete turmas de 8º e 9º ano recuam em Língua Portuguesa**, e cinco delas avançam em Matemática no mesmo período — justamente no segmento onde a comparação entre as duas provas é confiável.

## Privacidade — este repositório deve permanecer privado

O painel identifica os estudantes **pelo nome completo**, ao lado de notas individuais, nível de proficiência e habilidades a recuperar. São dados pessoais de menores de idade.

- O repositório precisa estar com visibilidade **Private** no GitHub. Confira antes de cada `push`.
- **Não ative o GitHub Pages.** Publicar as páginas tornaria o painel acessível por URL mesmo com o repositório privado.
- O acesso deve ficar restrito à equipe gestora e pedagógica da escola, pela aba Settings → Collaborators.
- A planilha de origem também contém dados pessoais e não é versionada aqui.

Se em algum momento o painel precisar ser compartilhado fora desse círculo, gere antes uma edição anonimizada, substituindo o nome por um código sequencial de turma.

## Origem

Gerado a partir de `Relatorio_Diagnostica_EF_SARESP.xlsx` (28 abas), mantido fora deste repositório. Para atualizar o painel, regenere o JSON embutido em `index.html` a partir de uma nova versão da planilha.
