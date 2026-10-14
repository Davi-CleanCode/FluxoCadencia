# Fluxo de Cadência — página de vendas

Página estática responsiva em HTML/CSS/JavaScript, preparada para deploy.

## Configurado
- Link de checkout Kiwify: https://pay.kiwify.com.br/NFPSyZ6
- Meta Pixel ID: 4424416794447577
- Evento `PageView` no carregamento
- Evento `InitiateCheckout` ao clicar nos botões de checkout
- Não dispara `Purchase` nesta página: esse evento deve acontecer somente após a confirmação de pagamento, idealmente pela integração da Kiwify.

## Deploy rápido (Netlify)
1. Extraia o ZIP.
2. Acesse https://app.netlify.com/drop
3. Arraste a pasta `fluxo_cadencia_site` (ou o `index.html` dentro dela, conforme a interface permitir).
4. Aguarde a publicação e copie a URL pública.
5. Na Kiwify, substitua o endereço temporário no campo de página de vendas pela URL publicada.

## Antes de anunciar
- Confirme que os PDFs/playbooks e o vídeo estão realmente publicados na área de membros.
- Abra o site publicado em uma janela anônima e teste os botões.
- Use a extensão Meta Pixel Helper ou Eventos de Teste do Gerenciador de Eventos para confirmar `PageView` e `InitiateCheckout`.
- Configure/valide o evento `Purchase` na Kiwify após pagamento confirmado. Não marque o botão como compra.
- Confira políticas de privacidade e dados de contato/suporte adequados ao seu negócio.

## Personalização
Edite o `index.html`. O site não exige Node.js, build ou dependências.
