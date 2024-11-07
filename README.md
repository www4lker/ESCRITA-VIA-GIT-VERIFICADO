> **Observção**: repositório apenas para fim de análise e comparação. O repositorio original da pesquisa em andamento está privado - e deverá ser disponibilizado tão logo a defesa ocorra.

# Impacto das Ferramentas de IA na Criatividade: Uma Análise em Humanidades

## Descrição do Projeto

Este projeto de dissertação de mestrado investiga o impacto das ferramentas alavancadas por Inteligência Artificial (IA) na criatividade dentro do campo das humanidades. Focalizando na interseção entre Geografia, Filosofia e Cultura, a pesquisa visa compreender como a IA influencia processos criativos e a produção de conhecimento nessas áreas.

## Objetivos

1. **Analisar o impacto das ferramentas de IA na criatividade acadêmica**: Examinar como ferramentas como ChatGPT e similares afetam a geração de ideias, escrita e desenvolvimento de conceitos em humanidades.
2. **Garantir a integridade e autoria do trabalho**: Implementar um sistema de documentação e verificação utilizando Git para comprovar a autoria original e minimizar o uso excessivo de ferramentas de IA.
3. **Desenvolver um fluxo de trabalho eficiente**: Criar um ambiente de trabalho que permita a utilização de múltiplos dispositivos (computador, laptop, tablet e celular) para escrita e versionamento via Git.

## Estrutura do Projeto

```plaintext
projeto-tese/
│
├── 01-markdown/                 # Arquivos em Markdown
│   ├── 00-front-matter/         # Elementos pré-textuais
│   │   ├── capa.md
│   │   ├── folha-rosto.md
│   │   ├── ficha-catalografica.md
│   │   ├── dedicatoria.md
│   │   ├── agradecimentos.md
│   │   ├── epigrafe.md
│   │   ├── resumo.md
│   │   ├── abstract.md
│   │   └── sumario.md
│   │
│   ├── 01-capitulos/            # Capítulos do conteúdo principal
│   │   ├── introducao.md
│   │   ├── revisao_literatura.md
│   │   ├── metodologia.md
│   │   ├── resultados.md
│   │   ├── conclusao.md
│   │   └── ...
│   │
│   └── anexos/                  # Anexos e apêndices
│       ├── apendice_a.md
│       └── apendice_b.md
│
├── 02-referencias/              # Referências bibliográficas
│   ├── bibliografia.bib
│   └── referencias.md
│
├── 03-assets/                   # Recursos (imagens, tabelas, gráficos)
│   ├── figuras/
│   │   ├── figura1.png          
│   │   └── figura2.png
│   ├── tabelas/
│   │   └── tabela1.md
│   └── graficos/
│       └── grafico1.md
│
├── 04-latex/                    # Arquivos LaTeX para conversão
│   ├── abnt-templates/
│   │   ├── abnt.cls
│   │   └── abnt.sty
│   └── main.tex
│
├── 05-registros-ia/             # Registros de uso de IA
│   ├── usos-ia.md
│   ├── conversas/
│   │   ├── conversa1.md
│   │   └── conversa2.md
│   └── referencias-ia.md
│
├── diario_pesquisa.md           # Registro das atividades de pesquisa
└── README.md                    # Documentação do projeto
```

## Decisões Tomadas

### **Uso do Git e GitHub**

- **Controle de Versão**: Implementação do Git para rastrear todas as alterações no documento, garantindo um histórico detalhado do desenvolvimento da dissertação.
- **Repositório Privado**: Inicialmente, o repositório será privado no GitHub para proteger o conteúdo durante o desenvolvimento, tornando-o público apenas após a defesa conforme as diretrizes institucionais.
- **Branches e Commits**: Utilização de branches para experimentações e commits frequentes com mensagens descritivas para facilitar a rastreabilidade e a reversão de mudanças, se necessário.

### **Ferramentas de Escrita**

- **Visual Studio Code (VSCode)**: IDE principal no computador para edição e gerenciamento do Git.
- **Obsidian**: Aplicativo escolhido para dispositivos móveis (tablet e celular) para edições leves e criação de conteúdo quando em movimento.
- **Pandoc**: Ferramenta utilizada para converter arquivos Markdown em formatos acadêmicos como PDF e DOCX.
- **Markdown**: Linguagem de marcação adotada pela sua simplicidade e compatibilidade com múltiplos dispositivos e ferramentas.

### **Estrutura de Diretórios**

- **01-markdown/**: Contém todos os arquivos em Markdown organizados por capítulos e seções, facilitando a gestão e revisão.
- **02-referencias/**: Gerenciamento das referências bibliográficas usando BibTeX para integração futura com LaTeX.
- **03-assets/**: Armazenamento de recursos visuais como figuras, tabelas e gráficos.
- **04-latex/**: Preparação para conversão final do trabalho utilizando templates ABNT personalizados.
- **05-registros-ia/**: Documentação detalhada das interações com ferramentas de IA, garantindo transparência no uso dessas tecnologias.
- **diario_pesquisa.md**: Registro contínuo das atividades de pesquisa, ideias e decisões tomadas durante o desenvolvimento da dissertação.

## Plano de Trabalho

### **1. Configuração Inicial**

- **Configuração do Repositório Git**: Inicializar o repositório localmente e conectá-lo ao GitHub.
- **Estruturação dos Diretórios**: Organizar os diretórios conforme o esquema decidido.
- **Configuração das Ferramentas**: Instalar e configurar VSCode, iA Writer e Pandoc.

### **2. Desenvolvimento da Dissertação**

- **Escrita e Edição**: Utilizar VSCode e Obsidian no computador para a maior parte da escrita e gerenciar versões. Usar Obsidian em dispositivos móveis para edições rápidas e adições de conteúdo em movimento.
- **Documentação do Uso de IA**: Registrar todas as interações relevantes com ferramentas de IA no diretório `05-registros-ia/`, detalhando datas, contextos e integrações na dissertação.
- **Gestão de Referências**: Manter referências organizadas no arquivo BibTeX para facilitar citações e formatação.

### **3. Versionamento e Backup**

- **Commits Frequentes**: Realizar commits diários com mensagens claras e descritivas.
- **Uso de Tags**: Uso de tags para marcar momentos imporantes do processo de escrita.
- **Uso de Branches**: Criar branches para explorar diferentes abordagens ou estruturar capítulos específicos.
- **Sincronização com GitHub**: Fazer push regularmente para garantir backups e permitir acesso seguro a partir de múltiplos dispositivos.

### **4. Revisões e Feedback**

- **Colaboração com Orientador**: Compartilhar o repositório com o orientador para revisões via GitHub, utilizando issues para feedback e acompanhamento de tarefas.
- **Resolução de Conflitos**: Aprender e aplicar técnicas de merge para resolver possíveis conflitos de versões.

### **5. Preparação Final**

- **Conversão de Formatos**: Utilizar Pandoc para converter o trabalho final de Markdown para PDF ou DOCX conforme necessário.
- **Revisão e Polimento**: Realizar uma revisão abrangente de todo o documento, assegurando a integridade narrativa e a conformidade com as normas acadêmicas.
- **Tagging de Versões**: Marcar versões finais dos capítulos e do documento completo para referência.

### **6. Defesa e Publicação**

- **Defesa da Dissertação**: Preparar a apresentação e defender a dissertação com base no trabalho desenvolvido.
- **Publicação no GitHub**: Tornar o repositório público ou exportar o conteúdo conforme as diretrizes institucionais após a defesa.

## Considerações Finais

Este projeto visa não apenas explorar o impacto das ferramentas de IA na criatividade acadêmica, mas também estabelecer um fluxo de trabalho transparente e verificável que assegure a autoria e a integridade do trabalho. A utilização de Git e GitHub, combinada com ferramentas de escrita flexíveis, proporciona uma abordagem moderna e eficiente para a gestão de dissertações em humanidades.

---

**Contato**

- **Autor**: WALKER DE B DANTAS PANIAGUA
- **Email**: niilist@gmail.com
