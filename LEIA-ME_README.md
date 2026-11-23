# Central PS: link próprio, ícone no celular e sem o aviso do Google

**English version below.**

## Português

Esta pasta é uma página pequena que abre a Central PS em tela cheia. Com ela:
- o aviso cinza "Este app foi criado por um usuário do Google Apps Script" não aparece;
- o iPhone e o Android usam o ícone do PF na tela de início, sem o app Atalhos;
- não tem a formatação estranha do Google Sites;
- existem dois links: um em português e um em inglês (`/en/`).

Planilhas, e-mails e recados do Urgente continuam iguais nas duas versões. Só a interface muda de idioma.

### 1. Conferir o link do app (1 minuto)
Abra `index.html` e `en/index.html` num editor de texto. Na linha `var APP_URL = '...'`, confira se o link é o mesmo que aparece em Apps Script → Implantar → Gerenciar implantações (termina em `/exec`). Se for diferente, troque nos dois arquivos.

### 2. Publicar no GitHub Pages (grátis, 5 minutos)
1. Entre em github.com (crie uma conta com o e-mail do PF, se não tiver).
2. Clique em **+ → New repository**. Nome: `central-ps`. Marque **Public** e clique em **Create repository**.
3. Clique em **uploading an existing file** e arraste **todo o conteúdo desta pasta**, incluindo a pasta `en`. Clique em **Commit changes**.
4. Vá em **Settings → Pages**. Em **Branch**, escolha `main` e `/ (root)` e clique em **Save**.
5. Depois de 1 a 2 minutos, o link aparece no topo da página: `https://SEU-USUARIO.github.io/central-ps/`.
   - Português: `https://SEU-USUARIO.github.io/central-ps/`
   - Inglês: `https://SEU-USUARIO.github.io/central-ps/en/`

### 3. Colocar na tela de início
- **iPhone (Safari):** abra o link → botão **Compartilhar** (quadrado com seta) → **Adicionar à Tela de Início** → **Adicionar**. O ícone do PF aparece sozinho.
- **Android (Chrome):** abra o link → **⋮** → **Adicionar à tela inicial** (ou **Instalar app**).
- **Quem já tinha atalho antigo** (Atalhos ou Google Sites): apague o atalho antigo e crie de novo com o link novo.

### 4. Problemas comuns
| O que aparece | O que fazer |
|---|---|
| Tela preta parada | Confira o `APP_URL` (passo 1) e se a implantação está como "Qualquer pessoa". |
| "404" no GitHub | Espere 2 minutos depois do passo 4 e confira se `index.html` está na raiz do repositório, não dentro de outra pasta. |
| Ícone genérico no iPhone | Use o Safari (não o Chrome) para "Adicionar à Tela de Início" e confira se `icon-180.png` foi enviado. |
| Pede o código toda vez no iPhone | O Safari limita o armazenamento de páginas incorporadas. Entre uma vez pelo ícone da tela de início, que ele passa a lembrar. |
| O aviso do Google ainda aparece | Você abriu o link `/exec` direto. Use sempre o link do GitHub. |

### 5. Google Sites
Pode apagar o site criado antes (sites.google.com → ⋮ → Mover para a lixeira). Ele não é mais necessário.

---

## English

This folder is a small page that opens Central PS full screen. It:
- removes the grey "This application was created by a Google Apps Script user" banner;
- gives iPhone and Android the PF icon on the home screen, without the Shortcuts app;
- avoids the odd Google Sites layout;
- offers two links: Portuguese and English (`/en/`).

Spreadsheets, emails and Urgente messages stay the same in both versions. Only the interface language changes.

### 1. Check the app link (1 minute)
Open `index.html` and `en/index.html` in a text editor. On the line `var APP_URL = '...'`, make sure the link matches Apps Script → Deploy → Manage deployments (it ends in `/exec`). If it doesn't, replace it in both files.

### 2. Publish on GitHub Pages (free, 5 minutes)
1. Go to github.com (create an account with the PF email if needed).
2. Click **+ → New repository**. Name: `central-ps`. Select **Public** and click **Create repository**.
3. Click **uploading an existing file** and drag **everything in this folder**, including the `en` folder. Click **Commit changes**.
4. Go to **Settings → Pages**. Under **Branch**, choose `main` and `/ (root)` and click **Save**.
5. After 1 to 2 minutes the link shows at the top: `https://YOUR-USER.github.io/central-ps/`.
   - Portuguese: `https://YOUR-USER.github.io/central-ps/`
   - English: `https://YOUR-USER.github.io/central-ps/en/`

### 3. Add to the home screen
- **iPhone (Safari):** open the link → **Share** (square with arrow) → **Add to Home Screen** → **Add**. The PF icon is used automatically.
- **Android (Chrome):** open the link → **⋮** → **Add to Home screen** (or **Install app**).
- **If you had an old shortcut** (Shortcuts app or Google Sites): delete it and add the new link.

### 4. Common problems
| What you see | What to do |
|---|---|
| Black screen that never loads | Check `APP_URL` (step 1) and that the deployment is set to "Anyone". |
| "404" on GitHub | Wait 2 minutes after step 4 and make sure `index.html` is at the repository root, not inside another folder. |
| Generic icon on iPhone | Use Safari (not Chrome) for "Add to Home Screen" and make sure `icon-180.png` was uploaded. |
| Asks for the code every time on iPhone | Safari limits storage for embedded pages. Sign in once from the home-screen icon and it will remember you. |
| The Google banner still shows | You opened the `/exec` link directly. Always use the GitHub link. |

### 5. Google Sites
You can delete the site created earlier (sites.google.com → ⋮ → Move to trash). It is no longer needed.
