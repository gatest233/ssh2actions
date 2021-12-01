# SSH to GitHub Actions

This GitHub Action offers you connect to GitHub Actions VM via SSH for interactive debugging

## Features

- Support Ubuntu and macOS
- Provides two optional SSH connection methods, tmate and ngrok
- Proceed to the next step to stay connected
- Send SSH connection info to Telegram

## Usage

### SSH to Github Actions

```yaml
- name: Start SSH
  uses: gatest233/ssh2actions@main
  with:
    mode: ssh
  env:
    # This password you will use when authorizing via SSH
    SSH_PASSWORD: ${{ secrets.SSH_PASSWORD }}

    # Send connection info to Telegram (optional)
    # You can find related documents here: https://core.telegram.org/bots
    TELEGRAM_BOT_TOKEN: ${{ secrets.TELEGRAM_BOT_TOKEN }}
    TELEGRAM_CHAT_ID: ${{ secrets.TELEGRAM_CHAT_ID }}
```

## Lisence

[MIT](https://github.com/P3TERX/ssh2actions/blob/main/LICENSE) © P3TERX
