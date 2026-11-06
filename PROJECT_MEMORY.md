# Projektová paměť Bunny Studios

## Přehled ověřený 2026-11-06

- Repozitář: toxiclevan-del/bunny-studios, větev main. Výchozí commit: 026936a.
- Statický web bez balíčkovacího systému a backendu. HTML, assets/site.css,
  assets/site.js; dokumentace doporučuje GitHub Pages z main a kořene.
- index.html je anglický úvod, cs/index.html český; nomad/ je produktová stránka.
- Produkt NOMAD Shop Core 0.2.0-rc.4 je modulární RPG obchod pro Unity:
  katalog, Shop Editor, 3D náhled, lokalizace a adaptéry herních systémů.
- docs/ obsahuje EN/CZ návody: QuickStart, UserManual, ShopEditor, Integration,
  VisualGuide, Dependencies, Troubleshooting a Architecture, včetně screenshotů.
- Herní ukládání, produkční inventář a síťovou autoritu řeší hostitelská hra.
- Veřejný kontakt je zatím placeholder; veřejné stažení ani schválení Asset Store
  nejsou doložené. Zachovat tuto přesnost.

## 2026-11-06 — počítadlo a paměť

Zadání: přidat počítadlo úplně dolů na hlavní stránku, poznat obsah repozitáře
a uchovávat výsledky, ověření, schválení a chyby pro další úkoly.
Uživatelka schválila zahájení po shrnutí zadání. Následně 2026-11-06
potvrdila přítomnost počítadla na webu a výslovně povolila zapsat dobrý výsledek.

Změny:
- index.html a cs/index.html: společný Hits.sh SVG čítač v patičce pod odkazy,
  překlady popisků, začátek měření od listopadu 2026, odkaz na statistiky.
- assets/site.css: responzivní řádek počítadla v barvách webu.
- AGENTS.md: čtení paměti před úkolem a aktualizace po úkolu a feedbacku.
- PROJECT_MEMORY.md: tento přehled a historie.

Počítadlo:
- Klíč: toxiclevan-del.github.io/bunny-studios, společný pro oba jazyky.
- Externí služba: https://hits.sh/ ; dokumentace: https://github.com/silentsoft/hits
- Zobrazení obrázku čítače, nikoli audit unikátních lidí. Historická návštěvnost
  není známa a nedoplňuje se. Cache, blokátory a dostupnost služby ovlivní měření.
- Žádné API klíče ani vlastní backend. Prohlížeč kontaktuje Hits.sh;
  referrerpolicy=no-referrer omezuje předávání odkazující stránky.
- Na úvodních stránkách byl nahrazen původní slib „bez analytiky a sledování“.
- Kontrola endpointu vrátila HTTP 200 a image/svg+xml, cache-control no-store.
  Technická kontrola může přidat zkušební zobrazení.

Stav: implementováno. Prošly kontroly obou patiček, společného klíče,
alt textů, no-referrer, lokálních odkazů úvodních stránek a git diff --check.
Nasazení hlavní změny ověřeno na veřejné české stránce v prohlížeči;\nčítač zobrazil hodnotu. Stará cache CSS při první kontrole nezobrazila nové\nrozložení; doplněna verze URL stylesheetu na obou úvodech pro obnovu cache.\nMobilní zobrazení nebylo vizuálně ověřeno.
Potvrzení výsledku uživatelkou: POTVRZENO 2026-11-06 — dobrý výsledek.
Zpětná vazba: „je to tam“ a „mužeš si zapsat dobrý výsledek“.
Pokyn pro tento navazující úkol: zapsat pouze potvrzení do paměti, nic jiného nedělat.

## Feedback a neúspěšné postupy

- Zatím žádný negativní feedback uživatelky k implementaci.
- Nezaměňovat souhlas s plánem za potvrzení funkčního výsledku.
- GitHub konektor odmítl čtení /pages jako nepodporovaný endpoint; z tohoto
  odmítnutí nevyvozovat, že Pages nejsou aktivní.
- Automatické zachování kontextu napříč všemi chaty nelze zaručit; pravidla
  v repozitáři a paměť fungují při jejich načtení agentem.
