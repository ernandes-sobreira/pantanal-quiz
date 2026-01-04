# Pantanal Quiz – Android (offline)

Um app Android simples (Kotlin + WebView) que roda um quiz leve e colorido sobre o Pantanal e **serviços ecossistêmicos**.
Ele funciona **offline** (as perguntas ficam em um arquivo `.js`) e é fácil de você adicionar mais depois.

## Como abrir e gerar o APK/AAB (Android Studio)
1. Instale o **Android Studio**.
2. Abra o projeto: **File > Open** e selecione a pasta `PantanalQuiz/`.
3. Espere o Gradle sincronizar.
4. Rode no celular (USB debug) ou emulador: **Run > Run 'app'**.
5. Para publicar na Play Store, gere **AAB**: **Build > Generate Signed Bundle / APK** > **Android App Bundle (AAB)**.

## Onde adicionar perguntas
As perguntas ficam em:
`app/src/main/assets/www/questions.js`

Cada pergunta tem:
- `q`: enunciado
- `options`: alternativas
- `answer`: índice da alternativa correta (0..3)
- `explain`: explicação curta (ciência + humor leve)

## Ajustar cores/visual
- CSS: `app/src/main/assets/www/styles.css`
- Ícones: `app/src/main/res/mipmap-*`

## Observações
- O app é “casca Android” + quiz em HTML/JS (muito leve).
- Não precisa de internet.
