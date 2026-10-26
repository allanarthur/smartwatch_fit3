# Fit3 Link para iPhone 15 — comece aqui

App nativo (Swift/SwiftUI) para usar a Samsung Galaxy Fit3 (SM-R390) no iPhone 15.
Baseado no projeto Fit3 Link (Vinizera-ai/samsung-app-for-ios), que por sua vez usa o protocolo
decifrado pelo yuriyurin/Fit3-App. Licença GPL-3.0 (veja LICENSE). Não é afiliado à Samsung.

Ajustes desta versão: alvo mínimo iOS 17 (iPhone 15). Código revisado: a única conexão com a
internet é a previsão do tempo (Open-Meteo); dados de saúde não saem do iPhone.

## Passo a passo (sem Mac)

1. Crie uma conta no GitHub (se não tiver) e um repositório **público** chamado `fit3link`.
2. Envie todo o conteúdo desta pasta para a branch `main` (pelo site: "Add file > Upload files"
   funciona, mas **inclua a pasta oculta `.github`**; pelo GitHub Desktop é mais fácil).
3. Aba **Actions**: o build roda sozinho (~10 min). Se pedir, clique em "Enable workflows".
4. Aba **Releases > latest**: baixe `Fit3Link-Saude.ipa` (ou `Fit3Link.ipa` se o outro falhar).
5. Instale com o **Sideloadly** no Windows/Mac (ou SideStore) — detalhes em `docs/INSTALACAO.md`.
6. No iPhone: Ajustes > Privacidade e Segurança > **Modo de Desenvolvedor** (ativar) e
   Ajustes > Geral > **VPN e Gerenciamento de Dispositivos** > confiar no seu Apple ID.
7. Abra o app > **Procurar minha Galaxy Fit3**. Se a pulseira estava num Android, redefina-a antes.

Com Apple ID gratuito o app precisa ser renovado a cada 7 dias (o Sideloadly faz isso pelo Wi-Fi).

## O que funciona / o que não dá

Funciona: notificações via Atalhos (SMS, iMessage, e-mail), toque de chamada e chamada perdida,
hora/idioma, bateria, música (Apple Music), passos, batimentos, oxigênio, estresse, sono, clima,
envio ao Apple Saúde (se a assinatura gratuita liberar o HealthKit).

Impossível no iOS: notificações do WhatsApp e outros apps, nome de quem liga, instalar mostradores
ou firmware.

## Primeiro teste

Este código ainda não tinha sido testado numa pulseira real. Se algo falhar, abra
Diagnóstico > **Log do protocolo** > compartilhar, e me mande o log para corrigirmos.
