# 📱 Diário Saúde — Instalação no Android

## Como instalar no Android (sem Play Store)

### Opção 1 — Chrome (recomendada)
1. Abra o arquivo `index.html` em um servidor local ou hospede no GitHub Pages / Netlify
2. Acesse pelo Chrome no celular
3. Toque nos **3 pontinhos** no canto superior direito
4. Selecione **"Adicionar à tela inicial"**
5. O app será instalado como PWA (Progressive Web App) nativa

### Opção 2 — Hospedagem rápida (GitHub Pages)
1. Crie um repositório no GitHub
2. Faça upload dos 3 arquivos: `index.html`, `manifest.json`, `sw.js`
3. Ative GitHub Pages em Settings > Pages
4. Acesse a URL gerada no celular e instale

### Opção 3 — Servidor local (Wi-Fi)
```bash
# No computador com Python:
cd pasta-do-app
python -m http.server 8080

# No celular (mesma rede Wi-Fi):
# Acesse: http://IP-DO-COMPUTADOR:8080
```

---

## Configuração inicial

1. Abra o app e toque em **"⚡ IA: —"** no topo ou vá em **Config**
2. Selecione a IA preferida:
   - **Claude** → API Key em console.anthropic.com
   - **GPT-4o** → API Key em platform.openai.com
   - **Gemini** → API Key em aistudio.google.com
3. Cole a API Key e salve

---

## Funcionalidades

| Aba | Função |
|-----|--------|
| 🗓 Hoje | Registrar pressão, sintomas, refeições |
| 📈 Gráficos | Visualizar tendências (diário/semanal/mensal) |
| 📋 Histórico | Consultar registros anteriores |
| 📊 Relatório | Gerar análise mensal com IA |
| ⚙️ Config | Configurar IA, API Key, meta calórica |

---

## Dados e privacidade
- Todos os dados ficam **salvos localmente** no navegador (localStorage)
- As chamadas de IA são diretas para as APIs (sem servidor intermediário)
- Use "Exportar dados" em Config para fazer backup em JSON
