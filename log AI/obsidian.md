obsidian.md

Para usar o Obsidian em conjunto com um repositório Git, basta configurá-lo para editar e salvar seus arquivos de Markdown, enquanto o Git gerencia o versionamento. Aqui está um guia sobre como configurar o `.gitignore` e os fluxos necessários para evitar conflitos e garantir sincronização.

### Configurando o `.gitignore` para o Obsidian

O Obsidian gera alguns arquivos e pastas que você provavelmente não quer versionar, pois eles são específicos da configuração local do editor. No diretório do seu repositório Git, edite o `.gitignore` e adicione as seguintes regras:

```plaintext
# Ignora as configurações locais do Obsidian
.obsidian/      # Pasta de configurações do Obsidian (plug-ins, temas, etc.)

# Ignora os arquivos de cache e histórico de anotações
.obsidian/workspace # Estado do workspace do Obsidian (posição de janelas etc.)
.obsidian/cache     # Cache do Obsidian
```

Essas entradas garantem que apenas os arquivos de Markdown (e outros que você deseja versionar) sejam rastreados pelo Git, enquanto as configurações específicas do Obsidian, que podem diferir entre dispositivos, serão ignoradas.

### Fluxo de Trabalho para Usar Obsidian com Git

#### 1. Edição e Salvamento no Obsidian
   - Abra o Obsidian na pasta onde está o repositório Git. Essa pasta conterá seus arquivos Markdown que o Obsidian pode editar e salvar.
   - Edite, salve e organize seus arquivos livremente. O Obsidian salvará as mudanças automaticamente.

#### 2. Controle de Versionamento com Git

   Cada vez que você terminar um conjunto de edições no Obsidian, siga estes passos no Git para sincronizar com o repositório remoto e manter tudo versionado:

   ```bash
   # Verifique o estado para ver quais arquivos foram alterados
   git status

   # Adicione os arquivos alterados ao próximo commit
   git add .

   # Crie um commit com uma mensagem descritiva
   git commit -m "Atualizações nos textos Markdown"

   # Envie as alterações para o repositório remoto
   git push origin main
   ```

#### 3. Sincronizando em Outro Dispositivo

   Em outro dispositivo onde você também usa o Obsidian, certifique-se de **fazer um pull antes de editar** para evitar conflitos:

   ```bash
   git pull origin main
   ```

   Isso trará todas as mudanças mais recentes para o repositório local. Agora, você pode abrir o Obsidian e editar os arquivos normalmente.

#### 4. Resolução de Conflitos (Se Necessário)

   Caso edite os mesmos arquivos em dispositivos diferentes sem sincronizar, o Git pode sinalizar conflitos. Nesse caso:
   
   - Use `git status` para ver os arquivos em conflito.
   - Edite esses arquivos manualmente, removendo as marcações de conflito (`<<< HEAD`, `===`, `>>> branch`).
   - Após resolver os conflitos, use `git add` nos arquivos e finalize o processo com um `git commit` para salvar as resoluções.

### Resumo

Esse fluxo permite que você use o Obsidian para editar e organizar arquivos de Markdown e o Git para versionar e sincronizar entre dispositivos. Certifique-se apenas de fazer `pull` no início de cada sessão em um novo dispositivo e `push` após concluir as edições.