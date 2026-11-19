# Defenda a Vila

Jogo vertical para live, inspirado em ninjas, com eventos do TikTok recebidos por WebSocket.

## Publicar no GitHub Pages

1. Em **Settings > Pages**, selecione a fonte **GitHub Actions** ou **Deploy from a branch**.
2. Se usar branch, selecione `main` e a pasta `/ (root)`.
3. Aguarde o Pages gerar o endereço do site.

## Conectar ao TikFinity

1. Abra o TikFinity e confirme que o WebSocket está ativo na porta `21213`.
2. Abra o jogo no mesmo computador pelo endereço local do servidor Pages ou diretamente pela pasta.
3. Clique em **Conectar**, mantenha `ws://localhost:21213/` e teste os eventos.

Também é possível abrir pela URL:

```text
https://SEU-USUARIO.github.io/tik-tok/?ws=ws://localhost:21213/
```

**Importante:** páginas HTTPS não permitem uma conexão `ws://` comum por bloqueio de conteúdo misto na maioria dos navegadores. Para esse servidor local, a opção mais confiável é hospedar o jogo em HTTP local ou configurar um WebSocket seguro (`wss://`) no TikFinity/proxy.

## Eventos

- Like: dispara shuriken
- Chat/comentário: cria um clone
- Follow: ativa barreira de chakra
- Share: recupera vida
- Gift: ativa poderes conforme o valor em diamantes

Use as teclas `L`, `C`, `F`, `H` e `1` a `5` para testar sem o TikFinity.
