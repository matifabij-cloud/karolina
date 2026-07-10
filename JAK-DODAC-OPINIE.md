# Jak dodać opinie na stronę (bez programisty)

Sekcja „Opinie" jest na razie **ukryta**, bo nie ma jeszcze prawdziwych opinii.
Gdy zbierzesz 2–3 opinie od klientek, dodasz je tak:

## Krok po kroku (na github.com)

1. Wejdź na swoje repozytorium **matifabij-cloud/karolina**.
2. U góry wybierz gałąź **`claude/modest-clarke-2ehqp9`** (tę samą, na której działa strona).
3. Kliknij plik **`index.html`**, a potem ikonę **ołówka** (Edit / „Edytuj").
4. Wciśnij **Ctrl+F** i wpisz: `id="opinie"` — przeskoczysz do sekcji opinii.
5. **Pokaż sekcję:** w linijce `<section id="opinie" ... hidden>` **usuń samo słowo** ` hidden`.
6. **Wstaw opinie:** znajdź fragmenty `[DO UZUPEŁNIENIA: prawdziwa opinia klientki – wklej tutaj]`
   i zamień je na prawdziwe opinie. Zamień też `[Imię]` na imię klientki.
7. Na dole strony kliknij zielony przycisk **`Commit changes`**.
8. Poczekaj 1–2 minuty i odśwież stronę (Ctrl+F5). Gotowe!

## Gotowy wzór JEDNEJ opinii (skopiuj, jeśli chcesz dodać więcej)

Wklej taki blok w środku `<div class="opinie__grid"> ... </div>`:

```html
<div class="opinie__card reveal">
  <div class="opinie__stars" aria-hidden="true">★★★★★</div>
  <p class="opinie__text">„Tutaj wpisz treść opinii klientki."</p>
  <p class="opinie__author">— Ania, Łódź</p>
</div>
```

- Chcesz mniej opinii? Usuń jeden taki blok.
- Chcesz więcej? Skopiuj blok i zmień treść.

## Podpowiedź
Jeśli utkniesz — możesz wkleić treść opinii do dowolnej rozmowy z Claude
i poprosić: „przygotuj mi gotowy blok HTML z tą opinią do wklejenia w sekcję opinie".
