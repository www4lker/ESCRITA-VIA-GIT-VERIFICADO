Para lançar um repositório Git local no GitHub e fazer seu primeiro commit, você pode seguir os passos abaixo. Vou assumir que você já tem um repositório no GitHub criado e que você deseja conectar seu repositório local a ele.

### Passos para fazer o primeiro commit e enviar para o GitHub

1. **Navegue até o diretório do seu projeto** (você já está nesse diretório):
   ```bash
   cd ~/Documentos/GitHub/TES-TIG
   ```

2. **Adicione todos os arquivos ao seu repositório local**:
   ```bash
   git add .
   ```

3. **Faça seu primeiro commit**:
   ```bash
   git commit -m "Meu primeiro commit"
   ```

4. **Adicione o repositório remoto** (substitua `URL_DO_REPOSITORIO` pela URL do seu repositório no GitHub):
   ```bash
   git remote add origin URL_DO_REPOSITORIO
   ```

5. **Envie seu commit para o GitHub**:
   ```bash
   git push -u origin master
   ```

### Observações

- Se você estiver usando uma branch diferente de `master` (como `main`), substitua `master` pelo nome da sua branch.
- Se você não tiver um repositório no GitHub ainda, crie um novo repositório no site do GitHub e copie a URL fornecida.
- Se você estiver usando autenticação de dois fatores no GitHub, pode ser necessário usar um token de acesso pessoal em vez da sua senha.

Após seguir esses passos, seu repositório local deve estar conectado ao GitHub e seu primeiro commit deve estar disponível no repositório remoto.