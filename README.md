# Site do desenvolvedor — CesarSoftDevelopment

Site estático (HTML + CSS puros, sem dependências) que serve como página do desenvolvedor
dos apps Android da **CesarSoftDevelopment**, usado na Google Play Console e para hospedar
o arquivo `app-ads.txt` do Google AdMob.

## Arquivos

- `index.html` — landing page com os apps e o contato.
- `privacidade.html` — política de privacidade (modelo, revisar antes de usar).
- `style.css` — estilos (claro/escuro, responsivo).
- `app-ads.txt` — arquivo do AdMob (deve ficar na raiz do domínio).
- `assets/` — ícones dos apps. Coloque aqui um **PNG quadrado (recomendado 512×512)**
  para cada app, com os nomes: `world-flags.png`, `controdata.png`,
  `viva-sampa.png`, `pomo-time.png` e `http-codes-with-dogs.png`. Há um `icon-placeholder.svg`
  de exemplo que pode ser removido depois.

## Publicar no GitHub Pages

> **Importante:** para o `app-ads.txt` ficar na raiz do domínio
> (`https://cesarsoftdevelopment.github.io/app-ads.txt`), o repositório precisa se chamar
> **exatamente** `cesarsoftdevelopment.github.io`.

### 1. Criar o repositório no GitHub
Crie um repositório **público** com o nome exato:

```
cesarsoftdevelopment.github.io
```

(Não marque a opção de adicionar README, pois este projeto já tem um.)

### 2. Enviar os arquivos (o commit inicial já está feito neste projeto)

```bash
git remote add origin https://github.com/CesarSoftDevelopment/cesarsoftdevelopment.github.io.git
git branch -M main
git push -u origin main
```

### 3. Ativar o GitHub Pages
No repositório: **Settings → Pages → Build and deployment → Source: Deploy from a branch**,
selecione a branch `main` e a pasta `/ (root)`, e salve.

### 4. Verificar
Após alguns minutos, confira:

- Página: `https://cesarsoftdevelopment.github.io/`
- App-ads: `https://cesarsoftdevelopment.github.io/app-ads.txt`

Depois configure esse domínio como o **site do desenvolvedor** na Google Play Console e
aguarde o AdMob validar o `app-ads.txt` (pode levar algumas horas/dias).
