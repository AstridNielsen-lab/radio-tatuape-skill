# Radio Tatuapé FM - Skill Alexa

Skill oficial da Radio Tatuapé FM para Amazon Alexa.

## Informações da Rádio
- **Nome**: Radio Tatuapé FM
- **Stream URL**: http://82.145.41.50/stream.mp3?ipport=82.145.41.50_16784
- **Invocação**: "Alexa, abra radio tatuapé"

## Funcionalidades
- Reproduzir a programação ao vivo da rádio
- Pausar/retomar reprodução
- Informações sobre a rádio
- Comandos de ajuda

## Comandos de Voz
- "Alexa, abra Radio Tatuapé"
- "Alexa, peça para Radio Tatuapé tocar música"
- "Tocar" ou "Reproduzir"
- "Parar" ou "Pausar"
- "Informações sobre a rádio"
- "Ajuda"

## Próximos Passos para Deploy

### 1. Configurar ASK CLI com sua conta Amazon
```bash
ask configure
```

### 2. Fazer deploy da skill
```bash
ask deploy
```

### 3. Testar a skill
Após o deploy, você pode:
- Testar no simulador do Amazon Developer Console
- Testar em dispositivos Alexa vinculados à sua conta
- Usar o comando: `ask dialog --locale pt-BR`

## Estrutura do Projeto
```
├── skill.json              # Configuração da skill
├── ask-resources.json       # Configuração de recursos ASK
├── models/
│   └── pt-BR.json          # Modelo de interação em português
└── lambda/
    ├── index.js            # Código principal da skill
    ├── package.json        # Dependências Node.js
    └── node_modules/       # Módulos instalados
```

## Personalização
Para personalizar a skill, edite:
- `lambda/index.js` - Lógica da skill e respostas
- `models/pt-BR.json` - Comandos de voz e intenções
- `skill.json` - Metadados da skill

## Notas Importantes
- A skill está configurada para o mercado brasileiro (pt-BR)
- Utiliza a interface AudioPlayer para streaming de áudio
- O stream deve estar sempre disponível para funcionamento adequado
- Certifique-se de que o URL do stream seja acessível publicamente

## Suporte
Para dúvidas sobre desenvolvimento de skills Alexa:
- [Documentação oficial Alexa Skills Kit](https://developer.amazon.com/docs/ask-overviews/build-skills-with-the-alexa-skills-kit.html)
- [ASK CLI Documentation](https://developer.amazon.com/docs/smapi/ask-cli-intro.html)

