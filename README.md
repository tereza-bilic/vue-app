1. interpolation/one-way binding:
2. two-way binding
3. methods
4. computed properties
5. barem jedan scoped style
6. koristiti barem jedan lifecycle hook
7. routing (više stranica)
  - aplikacija mora biti bookmarkable, tako da rade linkovi (ne samo na root, već i moj-web.com/stranica1, moj-web.com/stranica2)
  - dinamičko usmjeravanje s 404 stranicom ("catch all")
8. (barem) dvije komponente
 - komponenta bez stanja, koristiti properties
 - komponenta sa stanjem
9. barem jedna komponenta mora emitirati barem jedan event
10. store (Pinia)
11. asinkroni dohvat podataka s backenda, možete:
- koristiti Firebase ili Back4App, Mocky, itd.
- vlastiti storage, ili
- možete mock napraviti, držati podatke u memoriji, ali mora biti asinkroni poziv/upis
ostvariti asinkrono (lazy, po potrebi) učitavanje nekog dijela aplikacije (stranice ili komponente)
