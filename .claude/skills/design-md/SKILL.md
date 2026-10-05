---
name: design-md
description: Bibliothèque de 74 fichiers DESIGN.md (systèmes de design extraits de sites réels — Stripe, Apple, Linear, Vercel, Notion, Spotify…) issue de VoltAgent/awesome-design-md. À utiliser quand l'utilisateur veut changer le style/le look de l'interface (index.html, admin.html), "faire ressembler" la station météo à un site connu, choisir une palette, une typographie ou des composants cohérents, ou créer un DESIGN.md pour le projet.
---

# DESIGN.md — systèmes de design prêts à l'emploi

Source : https://github.com/VoltAgent/awesome-design-md (licence MIT, voir `LICENSE`).

Chaque fichier de `designs/` est un DESIGN.md (format Google Stitch) : un front-matter YAML avec les tokens
(`colors`, `typography`, `spacing`, `radius`, composants…) suivi d'une analyse en prose des règles visuelles
(ambiance, hiérarchie, usages à faire / à éviter).

## Designs disponibles

airbnb, airtable, apple, binance, bmw-m, bmw, bugatti, cal, claude, clay, clickhouse, cohere, coinbase, composio, cursor, dell-1996, elevenlabs, expo, ferrari, figma, framer, hashicorp, hp, ibm, intercom, kraken, lamborghini, linear.app, lovable, mastercard, meta, minimax, mintlify, miro, mistral.ai, mongodb, nike, nintendo-2001, notion, nvidia, ollama, opencode.ai, pinterest, playstation, posthog, raycast, renault, replicate, resend, revolut, runwayml, sanity, sentry, shopify, slack, spacex, spotify, starbucks, stripe, supabase, superhuman, tesla, theverge, together.ai, uber, vercel, vodafone, voltagent, warp, webflow, wired, wise, x.ai, zapier

Fichier : `.claude/skills/design-md/designs/<nom>.md`

## Comment l'utiliser

1. **Choisir un design** : si l'utilisateur nomme une marque, ouvre le fichier correspondant. Sinon, propose 2–3
   options adaptées à une station météo (lisible, orientée données) — par ex. `linear.app`, `vercel`, `stripe`,
   `apple`, `posthog`, `clickhouse` — en résumant leur ambiance en une ligne d'après la `description` du front-matter.
2. **Lire le fichier en entier** avant d'écrire du code : les tokens seuls ne suffisent pas, la prose contient les règles
   (poids de police, espacements, quand utiliser la couleur primaire, mode sombre…).
3. **Appliquer** :
   - Traduire les tokens en variables CSS sur `:root` (`--color-primary`, `--font-display`, `--radius-md`…) et les
     utiliser partout plutôt que des valeurs en dur.
   - Les polices propriétaires (Söhne, SF Pro, Circular…) ne sont pas disponibles : utiliser la pile de repli indiquée
     ou l'équivalent Google Fonts le plus proche (Inter, Geist, Manrope…).
   - Respecter les règles de composants (boutons, cartes, inputs) et de hiérarchie décrites dans la prose.
4. **Optionnel** : copier le fichier choisi à la racine du projet sous `DESIGN.md` pour que les futures sessions
   gardent le même langage visuel.

Ces fichiers décrivent un style *inspiré* de ces marques : ne pas reproduire leurs logos, noms ou contenus.
