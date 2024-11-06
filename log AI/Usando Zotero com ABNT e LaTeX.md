## Usando Zotero com ABNT e LaTeX

### Configuração ABNT

1. **Instalando o Estilo ABNT**
- Acesse as Preferências do Zotero
- Vá para a aba "Cite"
- Clique em "Get additional styles"
- Procure e instale "Associação Brasileira de Normas Técnicas - ABNT"

### Integração com LaTeX

**Configuração Inicial**
- Instale o Better BibTeX para Zotero
- Configure a exportação automática da biblioteca
- Use chaves de citação consistentes

### Workflow LaTeX-Zotero

1. **Exportação da Bibliografia**
```latex
\bibliography{nome-do-arquivo.bib}
\bibliographystyle{abnt}
```

2. **Citações no LaTeX**
- Use `\cite{chave-do-item}` para citações simples
- Use `\citeyear{chave-do-item}` para citar apenas o ano
- Use `\citeauthor{chave-do-item}` para citar apenas o autor

### Dicas Práticas

**Exportação Automática**
- Configure o Better BibTeX para exportar automaticamente
- Mantenha o arquivo .bib na mesma pasta do seu projeto LaTeX
- Use "Keep updated" para sincronização automática

**Organização**
- Crie uma coleção específica para cada projeto
- Use tags para identificar referências importantes
- Mantenha os PDFs anexados às referências

### Compilação

1. Sequência de compilação recomendada:
```bash
pdflatex arquivo
bibtex arquivo
pdflatex arquivo
pdflatex arquivo
```

Esta configuração permite manter suas referências organizadas no Zotero enquanto produz documentos formatados corretamente na ABNT usando LaTeX.

Citations:
[1] https://ppl-ai-file-upload.s3.amazonaws.com/web/direct-files/31920892/9185fddd-2c51-4846-b1c6-35f7347b0e4b/paste.txt