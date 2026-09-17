# Prompt final consolidado

Base: a versão com o tubo fino e a faixa de fio/miçangas a meio (melhor tubo
até à data). Conversa **nova** na ferramenta de imagem, imagem anexada, um
único prompt.

## Prompt

```
Edit only the two men's faces, the area between them, the large title, and two
of the captions at the bottom. Keep everything else exactly as it is — same
headdresses, same forest, same light, same tube with its beaded band, same
composition, same icons.

THE MAN ON THE LEFT
He is actively blowing through the tube. His lips are pressed firmly around the
near end of it, his cheeks slightly rounded with the effort of a short
controlled breath, his brow focused, and his eyes open and fixed on the other
man's nostril — attentive, precise, deliberate.

THE AIR BETWEEN THEM
Completely clear and empty, showing only the forest foliage and the warm golden
light behind them.

THE MAN ON THE RIGHT
The far end of the tube rests against his nostril instead of his mouth, angled
slightly upward, with a soft contact shadow where the wood meets his skin. His
mouth is closed and relaxed, his chin lowered slightly, his eyes closed, his
expression calm and inward — receiving, still.

THE TITLE
The title is a two-line block: the word RAPÉH on the first line, and the word
CEREMONY on the second line beneath it. Change ONLY the first line: remove its
final H so it reads RAPÉ, keeping the accented É. This is the removal of a
single letter, not a redrawing of the word — preserve the existing letterforms,
the speckled stone texture, the golden colour and the glow exactly as they are.
The second line, CEREMONY, must remain exactly as it is, unchanged and in place
beneath RAPÉ. Both lines stay on their current baselines, and the diamond
ornament and the line CONNECT CLEAR REALIGN below them stay exactly where they
are.

THE CAPTIONS
Under the second icon, the caption reads RAPÉH CEREMONY. Change it to RAPÉ
CEREMONY, on two lines — RAPÉ above, CEREMONY below.
Under the fourth icon, the caption reads SONGS. Change it to MEDICINE SONGS, on
two lines — MEDICINE above, SONGS below.
Both must keep exactly the same serif typeface, letter spacing, colour and size
as the other captions, centred under their icons in the same way. Leave the
icons and the two other captions untouched.

Photorealistic, warm golden backlight, shallow depth of field.
```

## Prompt curto — só repor CEREMONY

Se a base for a versão em que o título ficou reduzido a RAPÉ:

```
Add the word CEREMONY on its own line directly beneath the large title RAPÉ,
centred, in the same speckled stone texture, golden colour and glow as RAPÉ,
sized slightly smaller — the proportion of a title to its subtitle. Push the
diamond ornament and the line CONNECT CLEAR REALIGN down slightly to make room,
and restore the breathing space above the title. Change nothing else in the
image at all.
```

## Lições de redação acumuladas

1. **Escala ancorada na imagem**, nunca em centímetros ("no thicker than his
   own index finger", não "30 cm"). Os modelos não têm noção de escala absoluta.
2. **Descrever o estado desejado, nunca negar o indesejado.** "The air between
   them is clear and empty" funciona; "no smoke" reintroduz fumo.
3. **Quantificar termos de forma** ou omiti-los. `flare`, `funnel`, `cone`,
   `taper` sem qualificador de escala são amplificados — foi assim que a ronda 3
   produziu uma trombeta.
4. **Evitar vocabulário que ative filtros de conteúdo:** `blowpipe`/`blowgun`
   (arma), `seated inside the nostril` (penetração), `bone` (restos humanos).
   Alternativas: `slender ceremonial wooden tube`, `rests at the opening of the
   nostril`, `polished dark wood`.
5. **Uma edição de cada vez, conversa nova, a partir da melhor base guardada.**
   Reutilizar o fio faz o modelo reintroduzir defeitos das versões anteriores.
6. **Assimetria de postura resolve ambiguidade de papéis** melhor do que
   descrever objetos: olhos abertos e foco de um lado, olhos fechados e
   quietude do outro.
7. **Nomear tudo o que compõe um elemento antes de o alterar.** Dizer "o título
   diz RAPÉH" fez o modelo tratar o bloco inteiro como uma palavra e apagar a
   linha CEREMONY. Declarar "o título são duas linhas, X e Y; muda só X; Y fica
   intacta" evita-o.
8. **Terminar com `Nothing else in the image changes in any way.`** Sem essa
   linha, o modelo recompõe o espaçamento à volta do que editou.
