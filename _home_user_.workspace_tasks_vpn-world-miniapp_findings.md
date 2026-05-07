# VPN World - Research Findings

## Magnus UI Analysis (from screenshots)
- Dark theme: background ~#0f0f0f / #1a1a2e
- Accent colors: teal/green (#00d4aa, #0aff99)
- Cards with subtle borders, rounded corners
- Smooth gradients on headers
- Metric cards with percentage changes
- List items with icon + text layout

## Telegram Web App Requirements
- Must include `<script src="https://telegram.org/js/telegram-web-app.js"></script>`
- Use `window.Telegram.WebApp` for theme, haptics, etc.
- Bot must be created via @BotFather with /newbot
- Web App URL must be HTTPS
- Menu button configured via BotFather: /setmenubutton

## Country + VPN Data Structure
- Need ~195 countries
- Each country: name, code, flag emoji, continent
- VPN servers: hostname/IP, protocol (WireGuard/OpenVPN/IKEv2), port, region
