# Pacote de design · Ykedin Sushi (Nível 1, jornada única)

## 1. Premissa
Uma palavra: **momento**. O Ykedin não serve apenas sushi, cria momentos. O site inteiro ensina isso e termina num convite: "Viva esse momento!". Cada seção mostra um momento (a chegada à mesa, a história, o prato, a ocasião, a entrega) e afunila para UMA ação: **Fazer pedido** (https://pedido.anota.ai/loja/ykedin-cozinha-oriental). WhatsApp é a segunda via.

## 2. Paleta (tokens)
```css
:root{
  --canvas:#1b1312;       /* Preto Ykedin aprofundado para casar com o preto da fotografia */
  --panel:#261b1a;
  --accent:#BA4C4C;       /* Sakura: só no CTA, foco e 1 ou 2 ênfases */
  --accent-hover:#c85b5b;
  --accent-muted:#7a3131; /* a pétala escura da flor */
  --text-secondary:#b8aca2;
  --text-primary:#F5F1EA; /* Areia */
  --sand:#F5F1EA; --sand-2:#ECE5DA; --ink:#221616; --madeira:#B79578; --salvia:#899285;
}
```
Seções claras (Areia) alternam com escuras, seguindo a hierarquia do manual (claros + preto estruturam, Sakura assina).

## 3. Fontes
- Manrope 500/700/800: títulos em caixa-alta, texto, rótulos espaçados.
- Noto Serif itálico 400: palavras de destaque e o slogan.
- Desvio declarado: sem mono. O manual usa rótulos em Manrope caixa-alta espaçada, e a marca vence.

## 4. Mapa de faixas (pontos de partida, hero 460vh)
| Faixa | Intervalo | Momento da filmagem | Texto | Entrada |
|---|---|---|---|---|
| 1 | 0.00 a 0.30 | escuro, brilho quente lá embaixo | "Jacobina e Capim Grosso · desde 2016" / "NÃO SERVIMOS APENAS SUSHI." | deriva para baixo (a câmera desce) |
| 2 | 0.35 a 0.64 | a câmera desce, a luz acende na madeira | "Criamos *momentos.*" / "O primeiro encontro. O aniversário. A sexta que pede algo especial." | desfoque para nítido (a luz chegando) |
| 3 | 0.70 a 1.00 | pousa na foto real do combinado | "Viva esse momento!" / "Seu combinado favorito, do jeito que você gosta." / Fazer pedido · WhatsApp | subida palavra por palavra em etapas |

## 5. Hero estático (celular e movimento reduzido)
Foto real do hashi (retrato) ou do combinado (paisagem). "Viva esse momento!" / "Gastronomia japonesa em Jacobina e Capim Grosso, desde 2016." / Fazer pedido · WhatsApp.

## 6. Abaixo da dobra
1. **História (Areia):** "ANTES DE SER TENDÊNCIA, *já era* YKEDIN." 1º de abril de 2016, os primos Luiz e Pedro. Seis marcos do manual, com linhas que se desenham.
2. **Cardápio (escuro):** fotos reais, nomes curtos. CTA "Ver cardápio completo e pedir".
3. **Momento interativo (escuro, painel):** "Segure a flor." As cinco pétalas da flor original desabrocham uma a uma, cada uma revelando um momento (casais, família, amigos, delivery, sempre). Completo: "Viva esse momento!".
4. **Delivery (Areia):** "A EXPERIÊNCIA *chega inteira.*" Embalagem própria desde 2016, primeiro app próprio da região, cardápio online.
5. **Unidades (escuro):** Jacobina e Capim Grosso, horários, selo "aberto agora" calculado ao vivo.
6. **Perguntas:** como pedir, horários, fresco no delivery, quem não come cru, comemorações.
7. **CTA final + rodapé:** "Hoje tem Ykedin." Instagram @ykedinsushi.
Sem formulário: a ação liga direto ao pedido online existente.

## 7. Camada vetorial
Flor original grande a 5% de opacidade, fixa ao fundo, girando devagar (120s). Linhas de 1px que se desenham (grafismo 01 do manual). Grão sutil.

## 8. Engenharia
Blob com anel, interpolação por dt, seeks travados, DOM por delta, faixas com teste de flick, legibilidade em 4 camadas, 5 portões vivos, completo sem vídeo, movimento reduzido nas duas direções.

## 9. Gate de texto
Zero travessões, zero palavras de estoque, varredura de sinais de IA antes de mostrar.
