```markdown
# Identifying Components

Straight to the manufacturer's website can save you lots of time. Most components have a date code which used to be year and week (like 8634) but these days they can be cryptic batch codes. (In the old days, a TTL 74-series logic IC made in 1974, with a 74xx date code (Figure 2) could be a puzzler!)

If you have a few components of one type, look for a code that's the same on all of them — that will be the part number, the other codes will be date — or batch codes of no interest.

Values on passive components are either shown directly (like 47 pF) or as figures or resistor colour code in the form Digit1, Digit2, Multiplier (often having the number of zeros) on the components. So in this SMD, inductors is 3.3 µH (3300 µH, 3.3 is 33 mm (3300 µH). Capacitors may be marked in picofarads. A tantalum capacitor labelled 227 is 22 x 10^6 pF = 220 µF. Some have five rings of colour code, but the Internet is a great help in decoding these.

Most small SMD capacitors are not marked at all, so use your component test skills and equipment to verify them. And get a magnifying glass or a USB microscope (which is what used to take most of the photos for this article) — it makes it much easier to see the tiny writing on small components.

The internet has many resources to assist you — search for "IC Manufacturer's logos" or "SMD codes" if you need more information. And look up "EIA-96" to decode SMD resistors with what looks like a weird 2-number plus 1-letter code.

## Consider the Context

If you're stripping parts from old boards, or otherwise know where the components came from, that may give you a clue as to what the part is. A power supply is likely to have a switched-mode PWM IC, whereas an audio board is more likely to have op-amps.

## Don't Expect to Identify Everything!

I have a bag of transistors labelled 0V5F which have stubbornly refused to be identified. SMD components can be difficult or impossible to identify, as they often have shortened part numbers on them. Even with the considerable resources on the internet, they are not easy.

## Be Selective

I mentioned the boards I got as a kid, with bent-over component leads. I religiously unsoldered all of them. These days I won't touch such components unless they are really special; it's not worth the effort.

Electrolytic capacitors should always be tested, especially large power supply types, and look for domes on the tops — a dead giveaway that they have gone dry or leaky.

---

### Contributors

- Idea, text & illustrations: David Ashton
- Editor: Clemens Valens
- Layout: Giel Dols, Harman Heida

### Questions or Comments?

Do you have technical questions or comments about his article? Email the author at stn564@yahoo.com.au or contact Ektor at editor@elektor.com.

### RELATED PRODUCTS

- Andonstar AD407 HDMI Digital Microscope (SKU 19079) [www.elektor.com/19079](www.elektor.com/19079)
- Miniwatt DT71 Mini Digital Tweezers (SKU 19422) [www.elektor.com/19422](www.elektor.com/19422)
- OWON OW16B Digital Multimeter with Bluetooth (SKU 18780) [www.elektor.com/18780](www.elektor.com/18780)

### WEBLINKS

[1] Good datasheet site with lots of options: [www.alldatasheet.com/](www.alldatasheet.com/)

---

*lektron March & April 2022 39*
```