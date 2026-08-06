# MindMaps English — Página de Vendas

Site estático de página única (`index.html`), sem build e sem dependências — todas as imagens já estão embutidas no próprio arquivo em base64.

## Deploy no Vercel via GitHub

1. Crie um repositório novo em https://github.com/new (pode ser privado).
2. Suba este projeto pra ele:
   ```
   git remote add origin https://github.com/SEU-USUARIO/NOME-DO-REPO.git
   git branch -M main
   git push -u origin main
   ```
3. Em https://vercel.com, clique em **Add New → Project**, selecione esse repositório no GitHub e importe.
4. Não precisa configurar nada: Vercel detecta automaticamente que é um site estático (sem framework, sem build command) e publica o `index.html` na raiz.
5. Depois do primeiro deploy, você pode ligar seu domínio próprio em **Project → Settings → Domains**.

## Pendências antes de divulgar o link de verdade

- **Pixel do Meta**: o código já está no `index.html` (ID `1516929236420773`), mas ele só passa a funcionar depois que o site sai do preview e vai para um domínio real — o que vai acontecer com esse deploy no Vercel.
- **Kiwify**: cadastre esse mesmo Pixel ID dentro do painel da Kiwify (Marketing/Integrações) para capturar o evento de compra, que acontece na página de checkout deles, fora deste site.
- **Rodapé**: os links de Termos de Uso, Política de Privacidade e Contato ainda apontam para `#` — atualize com páginas reais antes de rodar tráfego pago.
