# Generador de fitxes de vistes

**Web:** https://antiahtml.github.io/vistes/

Web per crear peces 3D (cubs + talls inclinats) i generar fitxes i exàmens de vistes
(alçat, planta i perfil esquerre, sistema europeu) en català, castellà i gallec.

La web és `index.html` més la carpeta `logos`. No cal instal·lar res.

## Publicar-la a GitHub Pages

1. Crea un repositori nou a GitHub (per exemple `vistes`), públic.
2. Puja-hi el fitxer `index.html` i la carpeta `logos` (botó **Add file → Upload files**).
3. Ves a **Settings → Pages**. A *Branch* tria `main` i la carpeta `/ (root)` i desa.
4. Al cap d'un minut la web estarà a `https://EL-TEU-USUARI.github.io/vistes/`.

Per actualitzar-la, torna a pujar els fitxers que hagin canviat i substitueix els anteriors.

## On es guarden les dades

- Cada persona que obre la web té les seves dades (centres, logos, peces i documents)
  **només al seu navegador**. No s'envia res a cap servidor.
- A la pestanya **Dades** es poden exportar a un fitxer `.json` (còpia de seguretat,
  canvi d'ordinador o compartir peces amb un company) i tornar-les a importar.
- Si s'esborren les dades de navegació del lloc, es perd el que no s'hagi exportat.

## Requisits

Cal connexió a internet: el motor 3D (Three.js i Manifold) es carrega des de jsDelivr.

## Provar-la a l'ordinador

Obrir `index.html` amb doble clic pot no funcionar per les restriccions del navegador
amb els mòduls. Millor amb un servidor local:

```bash
python3 -m http.server 8765
```

i obrir `http://localhost:8765`.
