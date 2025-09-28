# 📺 Guia de Hospedagem da Lista M3U

## 🚀 Passo 1 — Preparar a lista

1. Crie um arquivo chamado **`lista.m3u`**.
2. Cole dentro dele seus canais/links de streaming.

Exemplo básico:

```m3u
#EXTM3U
#EXTINF:-1 tvg-id="CanalExemplo" tvg-name="Canal Exemplo HD" group-title="Filmes",Canal Exemplo HD
https://meuserver.com/stream/canal1.m3u8
```

---

## 🚀 Passo 2 — Subir no GitHub

1. Entre no [GitHub](https://github.com).
2. Clique em **New Repository**.

   * Nome: `iptv-lista` (ou o que você quiser).
   * Deixe público.
3. Faça upload do arquivo `lista.m3u`.
4. Clique em **Commit changes**.

Link cru do GitHub:

```
https://raw.githubusercontent.com/SEU-USUARIO/iptv-lista/main/lista.m3u
```

---

## 🚀 Passo 3 — Hospedar no Netlify

1. Vá em [Netlify](https://app.netlify.com/).
2. Crie um site novo a partir do **GitHub repo**.
3. Escolha o repositório criado (`iptv-lista`).
4. Deploy 🎉

Link do Netlify:

```
https://SEUAPP.netlify.app/lista.m3u
```

---

## 🚀 Passo 4 — Usar o seu domínio

1. No Netlify: **Site settings → Domain management → Add custom domain**
2. Coloque seu domínio (`seudominio.com`).
3. No painel DNS do seu domínio, aponte:

   * **CNAME**: `www → SEUAPP.netlify.app`
   * (ou use ALIAS/ANAME se quiser raiz direto `seudominio.com`).
4. Aguarde a propagação do DNS.

Agora o link final será:

```
https://seudominio.com/lista.m3u
```

---

## 🎯 Resultado Final

* 📂 Arquivo no GitHub: `lista.m3u`
* 🔗 Link cru: `https://raw.githubusercontent.com/.../lista.m3u`
* 🌐 Netlify: `https://seudominio.com/lista.m3u`

Pronto! Sua lista está hospedada, acessível e com domínio próprio.
