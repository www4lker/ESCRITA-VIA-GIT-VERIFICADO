# Quero uma estrutura de pastas para escrever minha tese salvando no git e usando markdown em um...
Exported on 04/11/2024 at 12:01:46 [from Perplexity.ai](https://www.perplexity.ai/search/quero-uma-estrutura-de-pastas-bKIFDZc1T3.aoGX4q8718A) - with [SaveMyChatbot](https://save.hugocollin.com)


## User
quero uma estrutura de pastas para escrever minha tese salvando no git e usando markdown em um primeiro momento. Em revisões tardias, converter em latex dentro do formato ABNT.

## AI answer
Para organizar a estrutura de pastas para sua tese, garantindo que o processo de escrita inicial em **Markdown** seja eficiente e que a conversão para **LaTeX** no formato ABNT seja facilitada posteriormente, sugiro a seguinte estrutura. Ela é otimizada para uso com Git, permitindo versionamento, além de manter a organização necessária para uma transição suave entre os formatos.

Estrutura de Pastas
-------------------

```text
tese/
│
├── 01-markdown/                 # Diretório principal para arquivos em Markdown
│   ├── 00-front-matter/         # Elementos pré-textuais (capa, resumo, etc.)
│   │   ├── capa.md              # Capa
│   │   ├── folha-rosto.md       # Folha de rosto
│   │   ├── ficha-catalografica.md # Ficha catalográfica
│   │   ├── dedicatoria.md       # Dedicatória (opcional)
│   │   ├── agradecimentos.md    # Agradecimentos (opcional)
│   │   ├── epigrafe.md          # Epígrafe (opcional)
│   │   ├── resumo.md            # Resumo em português
│   │   ├── abstract.md          # Resumo em inglês
│   │   └── sumario.md           # Sumário
│   │
│   ├── 01-introducao.md         # Capítulo de introdução
│   ├── 02-desenvolvimento/      # Diretório para capítulos do desenvolvimento
│   │   ├── capitulo1.md         # Primeiro capítulo do desenvolvimento
│   │   ├── capitulo2.md         # Segundo capítulo do desenvolvimento
│   │   └── ...                  # Outros capítulos
│   │
│   └── 03-conclusao.md          # Capítulo de conclusão
│
├── 02-referencias/              # Diretório para referências bibliográficas e citações
│   ├── referencias.bib          # Arquivo BibTeX para referências (para uso futuro no LaTeX)
│   └── referencias.md           # Referências em Markdown durante a fase inicial
│
├── 03-assets/                   # Diretório para recursos (imagens, tabelas, gráficos)
│   ├── imagens/                 # Imagens usadas no texto
│   │   └── ...                  
│   ├── tabelas/                 # Tabelas usadas no texto
│   │   └── ...
│   └── graficos/                # Gráficos usados no texto
│       └── ...
│   
├── 04-latex/                    # Diretório para arquivos LaTeX (para conversão posterior)
│   ├── abnt-templates/          # Modelos ABNT LaTeX (template .cls e .sty)
│   │    └── abnt.cls            # Classe LaTeX ABNT personalizada 
│   │    └── abnt.sty            # Estilo ABNT personalizado 
│   │    
│   ├── main.tex                 # Arquivo principal LaTeX que compilará a tese completa 
│   
└── README.md                    # Instruções e documentação do projeto
```

**Explicação da Estrutura**
---------------------------

*   **01-markdown/**: Esse diretório contém todo o conteúdo da tese escrito em Markdown. Ele está dividido em subpastas conforme os elementos pré-textuais, textuais e pós-textuais exigidos pela ABNT. Cada capítulo ou seção é armazenado em um arquivo separado.
*   **02-referencias/**: Durante a fase inicial de escrita, as referências podem ser gerenciadas diretamente em um arquivo `referencias.md`. No entanto, quando você migrar para LaTeX, será útil ter um arquivo `.bib` já preparado com suas referências.
*   **03-assets/**: Este diretório armazena todos os recursos visuais que você usará na tese, como imagens, tabelas e gráficos.
*   **04-latex/**: Quando chegar o momento de converter seu trabalho para LaTeX e formatá-lo conforme as normas da ABNT, este diretório conterá os arquivos necessários. O arquivo principal `main.tex` será o ponto de entrada para compilar toda a tese. A pasta `abnt-templates` inclui os arquivos `.cls` e `.sty` que definem o estilo ABNT.

**Fluxo de Trabalho**
---------------------

1.  **Escrita Inicial em Markdown**:
    
    *   Você começará escrevendo diretamente no diretório `01-markdown/`, usando arquivos `.md` separados para cada seção ou capítulo.
    *   Utilize o Git para versionamento contínuo do seu progresso.
    
2.  **Referências**:
    
    *   Durante a escrita em Markdown, você pode adicionar suas referências diretamente no arquivo `referencias.md`. Se já estiver utilizando um gerenciador de referências como o Zotero ou Mendeley, exporte as referências no formato BibTeX (`referencias.bib`) para facilitar a transição futura para LaTeX.
    
3.  **Conversão para LaTeX**:
    
    *   Quando estiver pronto para migrar seu trabalho para LaTeX, você poderá usar ferramentas como `pandoc` para converter seus arquivos `.md` diretamente em `.tex`.
    *   O diretório `04-latex/` conterá os templates ABNT necessários e o arquivo principal `main.tex`, que compilará todos os capítulos e seções convertidos.
    
4.  **Compilação Final**:
    
    *   Após ajustar os detalhes finais no LaTeX (como formatação ABNT), compile sua tese usando o comando `pdflatex main.tex`.
    

**Ferramentas Úteis**
---------------------

*   **Pandoc**: Para converter seus arquivos Markdown em LaTeX.
*   **Git**: Para controle de versão do projeto.
*   **BibTeX**: Para gerenciamento das referências bibliográficas.

Essa estrutura permitirá uma transição suave entre Markdown e LaTeX enquanto mantém seu trabalho organizado e preparado tanto para revisões quanto para formatação final conforme as normas da ABNT.

---
**Sources:**
- (1) Fundamentos de Metodologia Científica
- (2) Artigo sobre Gráficos e Visualização de Dados
- (3) Obrigatoriedade dos Elementos Pré-textuais em Trabalhos Acadêmicos


