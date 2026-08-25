# tiravis-demo

Demo de prezentare pentru **Tiravis** (tiravis.ro), construit de RTR Tech Solutions.

Folderul conține doar build-ul static. Sursa stă în
`website/templates/magazin online/magazin-electrocasince`.

Nu are backend: plățile, curierul, facturarea și conturile sunt simulate.
Indexarea e blocată prin `robots.txt` și prin `noindex` pe fiecare pagină, ca
demo-ul să nu concureze site-ul real al clientului.

Regenerare:

```bash
PUBLIC_BASE=/tiravis-demo PUBLIC_DEMO=1 npm run build
node scripts/publica.mjs <folder> tiravis-demo
```
