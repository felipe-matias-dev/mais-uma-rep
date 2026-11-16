# Mais Uma Rep

App de treino com progressão: cada treino, uma rep a mais. A barra no topo mostra quanto falta pra superar a última vez.

## Baixar no celular (Android)

**https://github.com/felipe-matias-dev/mais-uma-rep/releases/latest/download/MaisUmaRep.apk**

Abra esse link no celular, baixe e toque no arquivo pra instalar (o Android vai pedir pra permitir apps de fontes desconhecidas).

## Como funciona o projeto

- `www/` é o app (um `index.html` só, com as fontes em `www/fonts/`).
- `android/` é o projeto Android gerado pelo [Capacitor](https://capacitorjs.com), com ícone e tela de abertura do app.
- A cada push na `main`, o GitHub Actions (`.github/workflows/apk.yml`) compila o APK e publica em **Releases** como `MaisUmaRep.apk`.
- O APK é assinado com a chave em `keystore/`, sempre a mesma, então uma versão nova instala por cima da antiga sem apagar os treinos.

Pra mudar o app: edite `www/index.html`, faça commit na `main` e espere uns 5 minutos pelo APK novo.

Os treinos ficam salvos só no celular. Use **Ficha → Copiar backup** antes de trocar de aparelho.
