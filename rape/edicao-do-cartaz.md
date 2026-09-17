# Edição do cartaz — alterar só o que está errado

Original: `referencia/cartaz-original.png`

Objetivo: corrigir **duas** coisas. Tudo o resto — composição, enquadramento,
luz dourada, floresta, rostos, cocares, colares, tipografia e todo o texto —
fica **exatamente igual**.

---

## Edição 1 — substituir o tubo

**Máscara:** a região do tubo de bambu grosso, entre a boca do ancião da
esquerda e o rosto do ancião da direita, incluindo a mão que o segura.

**Instrução:**
> Replace the thick bamboo tube with a **thin ceremonial tepi blowpipe**: a
> slender straight tube roughly **30 cm long and no thicker than a finger**,
> made of narrow dark bamboo, with a carved tapered tip and **cotton thread and
> small beads wrapped around the middle**. Held **delicately between thumb and
> fingers, like a pen or a small flute** — not gripped in a closed fist.
> One end at the elder's lips, the **other end resting lightly against the
> right-hand elder's nostril**. Keep the same hand position and skin tones;
> adjust the fingers only as needed to hold a thin object.

**Nota de composição:** o tepi é bem mais curto que o tubo atual. Duas opções:
- **(a) Preferível** — aproximar ligeiramente as duas figuras, fechando o vão
  central, para que o tepi curto chegue de uma boca à outra narina.
- **(b) Alternativa sem mexer nas figuras** — manter o afastamento e aceitar um
  tepi no limite superior (~40 cm). Menos ideal, mas ainda correto.

---

## Edição 2 — remover o fumo

**Máscara:** toda a nuvem branca à volta do rosto do ancião da direita e a
saír-lhe do nariz e da boca.

**Instrução:**
> **Remove all smoke completely.** No plume, no white vapour, nothing leaving
> the nose or mouth. Fill the area with the **forest background and golden
> backlight** that belong behind it, matching the surrounding bokeh and haze.
> Optionally, a **barely visible wisp of fine light-brown powder** right at the
> nostril where the tube touches — a few grains, nothing more.

**Postura do recetor:** manter olhos fechados e expressão recolhida. Se a
edição o permitir, baixar ligeiramente o queixo (com o fumo, a cabeça está
atirada para trás como quem exala; sem fumo, a pose correta é mais contida).

---

## Negative prompt

```
smoke, smoke plume, white smoke, vapour, exhaling, cigarette, pipe, tobacco
smoke, thick bamboo trunk, blowgun, wide tube, long tube, closed fist grip,
fire, embers, ash
```

## Verificação final

- [ ] Tubo fino, calibre de um dedo ou menos
- [ ] Fio/miçangas enrolados a meio do tubo
- [ ] Ponta encostada à narina, não apontada ao ar
- [ ] Segurado entre os dedos, não com a mão fechada
- [ ] Zero fumo em qualquer ponto da imagem
- [ ] Texto e tipografia inalterados

## Nota sobre o título

`RAPÉH` é grafia inventada. Se fores refazer a tipografia, usar **RAPÉ** ou
**HAPÉ**. Se a edição for só às duas zonas acima, o texto fica como está.

---

# Ronda 2 — afinar a ponta do tepi

Estado após a ronda 1: `referencia/cartaz-v2.png`. Corpo do tubo correto
(fino, reto, fio e miçangas a meio) e fumo removido. Falta a extremidade.

## O que ainda está errado

1. **Sem bico esculpido.** Diâmetro uniforme até um corte reto — lê como lápis
   ou vareta. Um tepi afina nos últimos 2–3 cm num cone, muitas vezes com um
   ligeiro alargamento em funil na extremidade, tipicamente em osso polido ou
   madeira escura, com brilho e material distintos do corpo de bambu.
2. **Não entra na narina.** Está encostado à lateral do nariz. O bico assenta
   alguns milímetros **dentro** da abertura, com a narina comprimida à volta.
3. **Ângulo horizontal.** Deve subir em ângulo para dentro do nariz.
4. **Sem sombra de contacto.** Falta oclusão onde toca na pele — é o que faz o
   objeto parecer flutuar. Provavelmente o maior denunciador do render.

## Prompt (máscara: últimos 3–4 cm do tubo + narina)

> Refine the tip of the tepi blowpipe. The last 3 cm should be hand-carved and
> tapered: the bamboo narrows into a cone and ends in a slight funnel-shaped
> flare, made of polished bone or dark hardwood, visibly different in material
> and sheen from the bamboo shaft. The tip is seated a few millimetres inside
> the elder's nostril, angled slightly upward into the nose, not horizontal and
> not touching the side of the nose. The nostril is gently compressed and
> deformed around it. Add a soft contact shadow and ambient occlusion where the
> tip meets the skin. Photorealistic macro detail, matching the warm golden
> backlight.

**Negative:** `blunt cut end, uniform diameter tube, pencil tip, floating
object, no contact shadow, tip touching side of nose, horizontal alignment`

## Menores

- O pó está a sair acima e atrás do nariz; devia estar no ponto de contacto.
- O queixo continua atirado para trás (pose de exalação); recolhido é mais fiel.

## Terminologia

O instrumento desta cena é o **tepi**, não o kuripe. Não usar "kuripe" no
prompt — devolve a peça curva em V da auto-aplicação.

---

# Ronda 3 — REGRESSÃO, voltar à v2

Resultado: `referencia/cartaz-v3-regressao.png`. **Pior que a v2.** Não usar.

## O que correu mal

A expressão "funnel-shaped flare" no prompt da ronda 2 foi interpretada como
uma boca cónica: a ponta virou uma trombeta mais larga que um punho, tipo corno
cerimonial ou didgeridoo. Reintroduz o erro original de espessura e acrescenta
um defeito novo — tubo assimétrico, fino na boca e maciço no nariz. Apareceu
também uma segunda banda de miçangas junto ao bico.

Num tepi real o alargamento da extremidade é de **um a dois milímetros**,
quase impercetível. O calibre é fino e essencialmente uniforme de ponta a ponta.

## Correção: reaplicar sobre a v2, não sobre a v3

Máscara: últimos 3 cm do tubo + narina.

> Keep the blowpipe slim and uniform: the tube must stay the same thin diameter
> along its entire length, no wider than a finger from end to end. The final
> centimetre narrows very slightly into a smooth rounded nozzle of polished dark
> wood or bone, subtly different in sheen from the bamboo shaft. The change in
> width is only a millimetre or two and barely noticeable. The nozzle is seated
> a few millimetres inside the elder's nostril, angled slightly upward into the
> nose. The nostril is gently compressed around it. Soft contact shadow and
> ambient occlusion where it meets the skin. Photorealistic macro detail in warm
> golden backlight.

**Negative:** `flared end, funnel, cone, horn, trumpet bell, widening tube,
thick end, tapered wide mouth, didgeridoo, asymmetric tube, beaded collar at
the tip`

## Plano B

Se a ferramenta voltar a engrossar a ponta, remover do prompt toda a frase
sobre o bico e pedir **apenas** a sombra de contacto e o assentamento na
narina. A v2 sem bico esculpido, mas com contacto credível, é aceitável — e
preferível a arriscar nova regressão.

## Nota de redação de prompt

Evitar `flare`, `funnel`, `cone`, `bell`, `taper` sem qualificador de escala.
Estes modelos amplificam qualquer termo de forma. Quantificar sempre
("a millimetre or two", "barely noticeable") ou omitir.
