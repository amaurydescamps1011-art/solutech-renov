# Guide — Reproduire les 2 emails dans systeme.io

> **Avant de commencer**
> Dans systeme.io → Emails → Campagnes → "Créer une campagne" → Ajouter un email → choisir **"Éditeur visuel"**
>
> **Couleurs de référence :**
> - Fond global : `#0b1009`
> - Fond carte : `#0f1a10`
> - Vert accent : `#6ab023`
> - Bleu accent : `#29a8c4`
> - Texte blanc : `#ffffff`
> - Texte gris clair : `#aaaaaa`
> - Texte gris foncé : `#666666`
> - Or (étoiles) : `#f7a600`
> - Fond footer : `#0a120b`

---

# EMAIL 1 — Diagnostic DPE
## "Votre diagnostic énergétique est lancé"

---

## PARAMÈTRES GÉNÉRAUX DE L'EMAIL

1. Ouvrir les **Paramètres de l'email** (icône engrenage ou panneau latéral)
2. **Couleur de fond** du body : `#0b1009`
3. **Largeur** : 600px
4. **Police** : Arial ou Helvetica

---

## BLOC 1 — HEADER (Logo + Badge + Titre)

**→ Ajouter un bloc "Section"**
- Fond de section : `#0f1a10`
- Padding : 36px haut / 40px côtés / 28px bas
- Bordure radius (si disponible) : 20px en haut

**→ Dans cette section, ajouter un bloc "Image"**
- URL image : `https://i.postimg.cc/j5CtNN5L/image-(62)-(1).png`
- Hauteur : 50px
- Alignement : centré
- Marge basse : 20px

**→ Ajouter un bloc "Texte"**
- Contenu : `🔍 DIAGNOSTIC EN COURS D'ANALYSE`
- Police : Arial, 11px, **gras**
- Couleur texte : `#29a8c4`
- Alignement : centré
- Ajouter une bordure (si disponible) : couleur `#29a8c4`, épaisseur 1px, radius 100px
- Fond du bloc : `#0d2530` *(approximation du bleu foncé transparent)*
- Padding : 7px haut/bas, 16px gauche/droite
- Marge basse : 24px

> 💡 **Astuce** : Si systeme.io ne permet pas de border sur un texte, mets le badge en **image PNG** créée sur Canva (fond #0d2530, texte bleu, bords arrondis).

**→ Ajouter un bloc "Texte"**
- Contenu :
  ```
  Votre diagnostic
  énergétique est lancé
  ```
- Police : Georgia ou serif, 34px, **très gras (900)**
- "énergétique" en couleur `#6ab023` + italique
- Alignement : centré
- Couleur principale : `#ffffff`
- Marge basse : 14px

**→ Ajouter un bloc "Texte"**
- Contenu : `Nos experts analysent votre profil pour vous fournir une estimation précise de votre classe DPE et les travaux prioritaires pour l'améliorer.`
- "estimation précise de votre classe DPE" en **gras blanc** `#ffffff`
- Reste du texte : `#aaaaaa`, 16px, léger
- Alignement : centré

---

## BLOC 2 — JAUGE DPE (A à G)

> ⚠️ Le builder systeme.io ne peut pas reproduire les barres CSS. **2 options :**

### Option A (recommandée) — Créer l'image sur Canva
1. Aller sur canva.com
2. Créer un rectangle 520×120px, fond `#0f1a10`
3. Ajouter 7 rectangles colorés côte à côte avec lettres :
   - **A** — `#00a651` — hauteur 42px
   - **B** — `#51b848` — hauteur 50px
   - **C** — `#b2d235` — hauteur 58px
   - **D** — `#ffcc00` — hauteur 66px
   - **E** — `#f7a600` — hauteur 74px
   - **F** — `#e8601c` — hauteur 82px
   - **G** — `#cc0000` — hauteur 90px
4. Chaque lettre en blanc gras au centre de sa barre
5. Exporter en PNG et uploader dans systeme.io

**→ Ajouter un bloc "Image"**
- Uploader l'image de la jauge
- Alignement : centré
- Marge basse : 12px

**→ Ajouter un bloc "Texte"**
- Contenu : `Nos experts déterminent votre classe actuelle et votre potentiel d'amélioration`
- Police : 12px, couleur `#666666`
- Alignement : centré

### Option B — Texte symbolique
**→ Ajouter un bloc "Texte"** centré :
```
🟩 A   🟩 B   🟨 C   🟨 D   🟧 E   🟥 F   🟥 G
```
- 13px, centré, `#ffffff`

---

## BLOC 3 — ENCADRÉ "Notre analyse pour vous"

**→ Ajouter un bloc "Section"**
- Fond : `#0d2530` *(bleu très foncé)*
- Bordure : 1px `#29a8c4`
- Radius : 14px
- Padding : 24px haut/bas, 28px côtés
- Marge basse : 28px

**→ Dans cette section, ajouter un bloc "Texte"**
- Ligne 1 : `NOTRE ANALYSE POUR VOUS`
  - 12px, **gras**, lettres espacées, couleur `#29a8c4`, majuscules
- Ligne 2 : `À partir de vos réponses, nos experts réalisent une analyse approfondie de votre performance énergétique — déperditions thermiques, travaux prioritaires, gains attendus et aides mobilisables pour chaque poste de rénovation.`
  - "analyse approfondie de votre performance énergétique" en **blanc gras**
  - Reste : `#aaaaaa`, 14px
  - Interligne : 1.7

---

## BLOC 4 — LES 3 ÉTAPES "La suite pour vous"

**→ Ajouter un bloc "Texte"**
- Contenu : `LA SUITE POUR VOUS`
- 12px, **gras**, `#666666`, majuscules, espacement lettres
- Marge basse : 16px

**→ Répéter 3 fois : Ajouter un bloc "Section"**
Fond : `#1a1f1a` | Bordure : 1px `#2a2a2a` | Radius : 12px | Padding : 16px | Marge basse : 10px

**Dans chaque section → bloc "Colonnes" (2 colonnes)**

**Étape 1 :**
- Colonne gauche (15%) : `🔍` — 22px, centré
- Colonne droite (85%) :
  - Ligne 1 : `Analyse de votre profil énergétique` — 14px, **blanc gras**
  - Ligne 2 : `Classe DPE estimée + travaux prioritaires identifiés` — 12px, `#666666`

**Étape 2 :**
- Colonne gauche : `📞`
- Colonne droite :
  - Ligne 1 : `Appel de votre conseiller dédié` — **blanc gras**
  - Ligne 2 : `Sous 24h — il vous présente votre plan de rénovation personnalisé` — `#666666`

**Étape 3 :**
- Colonne gauche : `💰`
- Colonne droite :
  - Ligne 1 : `Chiffrage des aides disponibles` — **blanc gras**
  - Ligne 2 : `MaPrimeRénov', CEE, PTZ et aides locales cumulées` — `#666666`

---

## BLOC 5 — STATISTIQUES (3 colonnes)

**→ Ajouter un bloc "Texte"**
- `CE QU'UN MEILLEUR DPE CHANGE POUR VOUS`
- 12px, **gras**, `#666666`, majuscules
- Marge basse : 16px

**→ Ajouter un bloc "Colonnes" (3 colonnes égales)**

Chaque colonne :
- Fond : `#1a1f1a` | Bordure : 1px `#2a2a2a` | Radius : 12px | Padding : 16px | Alignement : centré

**Colonne 1 :**
```
📉
-40%
Sur vos factures d'énergie
```
- Emoji : 22px
- `-40%` : 13px, **blanc gras**
- Sous-texte : 11px, `#666666`

**Colonne 2 :**
```
📈
+15%
Valeur de votre bien
```

**Colonne 3 :**
```
🌿
-3t CO₂
Par an en moyenne
```

---

## BLOC 6 — BOUTON CTA

**→ Ajouter un bloc "Bouton"**
- Texte : `📷 Voir nos réalisations`
- URL : `https://www.instagram.com/solutech_renovation/`
- Couleur fond bouton : `#6ab023`
- Couleur texte : `#ffffff`
- Taille police : 15px, **gras**
- Padding : 16px haut/bas, 36px côtés
- Radius : 12px
- Alignement : centré
- Marge haut/bas : 28px

---

## BLOC 7 — AVIS CLIENTS

**→ Ajouter un bloc "Texte"**
- `ILS ONT AMÉLIORÉ LEUR DPE AVEC NOUS`
- 12px, **gras**, `#666666`, majuscules
- Marge basse : 14px

**→ Répéter 2 fois : Ajouter un bloc "Section"**
Fond : `#1a1f1a` | Bordure : 1px `#2a2a2a` | Radius : 12px | Padding : 16px | Marge basse : 10px

**Dans chaque section → bloc "Colonnes" (2 colonnes)**

**Avis 1 :**
- Colonne gauche (12%) : Image ronde `https://i.postimg.cc/PNcXKnXb/hf-20260305-065738-93a1c7fe-19ef-44bc-b621-92bbefd440ae.png` — 36x36px, radius 50%
- Colonne droite (88%) :
  - Ligne 1 : `Philippe D. — Bordeaux` (13px, blanc gras) + `★★★★★` (11px, `#f7a600`)
  - Ligne 2 : `Maison de 1971, on était en F. Isolation + PAC, on paie presque plus de chauffage.` — 12px, `#aaaaaa`

**Avis 2 :**
- Colonne gauche : Image `https://i.postimg.cc/xqqjK12x/hf-20260305-070009-001a1cf1-3fe8-4a37-b404-75888f768731.png`
- Colonne droite :
  - `Sophie L. — Montpellier` + `★★★★★`
  - `Sceptique au départ mais le conseiller m'a tout expliqué sans pression. 11 000€ récupérés.`

---

## BLOC 8 — FOOTER

**→ Ajouter un bloc "Section"**
- Fond : `#0a120b`
- Padding : 24px haut/bas, 40px côtés
- Radius bas : 20px (si disponible)
- Bordure haut : 1px `#222222`

**→ Bloc "Image"**
- URL : `https://i.postimg.cc/j5CtNN5L/image-(62)-(1).png`
- Hauteur : 32px | Opacité : 70% (si disponible, sinon laisser normal)
- Centré | Marge basse : 12px

**→ Bloc "Texte"**
- `Solutech Renov — Expert en rénovation énergétique`
- Saut de ligne
- `Cet email vous a été envoyé suite à votre demande de diagnostic. Conformément au RGPD, vos données sont confidentielles et ne seront jamais partagées.`
- Police : 11px, `#444444`, centré, interligne 1.6

---
---

# EMAIL 2 — Estimation des Aides
## "Votre estimation est en cours"

---

## PARAMÈTRES GÉNÉRAUX

- Mêmes réglages que l'Email 1 (fond `#0b1009`, 600px)

---

## BLOC 1 — HEADER

**→ Section** fond `#0f1a10`, padding 36px/40px/28px, radius haut 20px

**→ Image** : Logo `https://i.postimg.cc/j5CtNN5L/image-(62)-(1).png` — 50px, centré, marge basse 20px

**→ Texte** (badge) :
- Contenu : `✓ DOSSIER BIEN REÇU`
- 11px, **gras**, couleur `#6ab023`, majuscules
- Fond badge : `#0d1f08` | Bordure : 1px `#6ab023` | Radius : 100px
- Padding : 7px/16px | Centré | Marge basse : 24px

> 💡 Même conseil : si la bordure sur texte n'est pas possible, créer un PNG Canva du badge.

**→ Texte** (titre) :
```
Votre estimation
est en cours
```
- Georgia, 34px, très gras, `#ffffff`, centré
- "en cours" en `#6ab023` italique
- Marge basse : 14px

**→ Texte** (sous-titre) :
- `Nos experts analysent votre dossier pour identifier toutes les aides auxquelles vous avez droit — MaPrimeRénov', CEE, PTZ et aides locales.`
- "toutes les aides auxquelles vous avez droit" en **blanc gras**
- Reste : `#aaaaaa`, 16px, centré

---

## BLOC 2 — ENCADRÉ "Ce que nos experts font pour vous"

**→ Section** fond `#0d1f08` | Bordure : 1px `#6ab023` | Radius : 14px | Padding : 24px/28px | Marge basse : 28px

**→ Texte** :
- Ligne 1 : `CE QUE NOS EXPERTS FONT POUR VOUS` — 12px, **gras**, `#6ab023`, majuscules
- Ligne 2 : `À partir de vos réponses, notre équipe réalise une analyse poussée et personnalisée de toutes les aides financières disponibles pour votre situation — barèmes 2026, plafonds de revenus, cumulabilité des dispositifs. Rien n'est laissé de côté.`
  - "analyse poussée et personnalisée" en **blanc gras**
  - Reste : `#aaaaaa`, 14px, interligne 1.7

---

## BLOC 3 — LES 3 ÉTAPES

**→ Texte** : `LA SUITE POUR VOUS` — 12px, **gras**, `#666666`, majuscules, marge basse 16px

**→ 3 sections répétées** (fond `#1a1f1a`, bordure `#2a2a2a`, radius 12px, padding 16px, marge basse 10px)

Chaque section avec **2 colonnes** :

**Étape 1 :**
- `📊` | `Analyse de votre dossier` (blanc gras) + `Nos experts calculent le montant exact de vos aides` (gris)

**Étape 2 :**
- `📞` | `Appel de votre conseiller dédié` (blanc gras) + `Sous 24h — il vous présente votre estimation personnalisée` (gris)

**Étape 3 :**
- `🚀` | `Lancement de votre projet` (blanc gras) + `Nous gérons tout le dossier de A à Z` (gris)

---

## BLOC 4 — GRILLE DES 4 AIDES (2×2)

**→ Texte** : `LES AIDES QUE NOUS ALLONS ANALYSER POUR VOUS` — 12px, **gras**, `#666666`, majuscules, marge basse 16px

**→ Ajouter un bloc "Colonnes" (2 colonnes)**
Chaque colonne : fond `#1a1f1a`, bordure `#2a2a2a`, radius 12px, padding 16px, centré

**Ligne 1 :**

| Colonne gauche | Colonne droite |
|---|---|
| 💚 | ⚡ |
| **MaPrimeRénov'** | **CEE** |
| Jusqu'à 90% des travaux | Certificats d'économie d'énergie |

**→ Spacer** : 10px de hauteur

**→ Ajouter un 2e bloc "Colonnes" (2 colonnes)**

**Ligne 2 :**

| Colonne gauche | Colonne droite |
|---|---|
| 🏦 | 📍 |
| **Éco-PTZ** | **Aides locales** |
| Prêt à taux zéro | Région, département, commune |

Pour chaque cellule :
- Emoji : 20px
- Nom de l'aide : 13px, **blanc gras**
- Description : 11px, `#666666`

---

## BLOC 5 — BOUTON CTA

**→ Bouton**
- Texte : `📷 Voir nos réalisations`
- URL : `https://www.instagram.com/solutech_renovation/`
- Fond : `#6ab023` | Texte : `#ffffff` | 15px **gras**
- Padding : 16px/36px | Radius : 12px | Centré
- Marge haut/bas : 28px

---

## BLOC 6 — AVIS CLIENTS

**→ Texte** : `ILS NOUS ONT FAIT CONFIANCE` — 12px, **gras**, `#666666`, majuscules, marge basse 14px

**→ Section** (fond `#1a1f1a`, bordure `#2a2a2a`, radius 12px, padding 16px, marge basse 10px)
**2 colonnes :**
- Image : `https://i.postimg.cc/fJtLhT22/hf-20260305-065726-545303d0-5d90-4797-813b-19721366b7bb.png` — 36px, ronde
- Texte : `Marie-Claire B. — Toulouse` + `★★★★★` (`#f7a600`)
  - `On a remplacé notre vieille chaudière fioul, 14 800€ d'aides. Je m'attendais pas à autant honnêtement.` — 12px, `#aaaaaa`

**→ Section** (même style, marge basse 10px)
**2 colonnes :**
- Image : `https://i.postimg.cc/PNcXKnXb/hf-20260305-065738-93a1c7fe-19ef-44bc-b621-92bbefd440ae.png` — 36px, ronde
- Texte : `Philippe D. — Bordeaux` + `★★★★★`
  - `Maison de 1971, on était en F. Isolation + PAC, on paie presque plus de chauffage.` — 12px, `#aaaaaa`

---

## BLOC 7 — FOOTER

**→ Section** fond `#0a120b`, padding 24px/40px, radius bas 20px, bordure haut `#222222`

**→ Image** : Logo `https://i.postimg.cc/j5CtNN5L/image-(62)-(1).png` — 32px, centré, marge basse 12px

**→ Texte** :
- `Solutech Renov — Expert en rénovation énergétique`
- `Cet email vous a été envoyé suite à votre demande d'estimation. Conformément au RGPD, vos données sont confidentielles et ne seront jamais partagées.`
- 11px, `#444444`, centré, interligne 1.6

---

# NOTES IMPORTANTES

## Limites du builder systeme.io à anticiper

| Élément HTML | Remplacement dans systeme.io |
|---|---|
| Jauge DPE (barres CSS) | Image PNG créée sur Canva |
| Badges avec bordure arrondie | Image PNG ou texte stylisé |
| Couleurs transparentes (rgba) | Utiliser les équivalents hex ci-dessous |
| Border-radius sur sections | Utiliser si disponible, sinon ignorer |

## Équivalents hex des couleurs rgba

| Code original | Équivalent hex opaque |
|---|---|
| rgba(255,255,255,.45) | `#aaaaaa` |
| rgba(255,255,255,.35) | `#888888` |
| rgba(255,255,255,.20) | `#444444` |
| rgba(106,176,35,.06) | `#0d1f08` |
| rgba(41,168,196,.06) | `#0d2530` |
| rgba(255,255,255,.04) | `#1a1f1a` |
| rgba(255,255,255,.07) | `#2a2a2a` |

## Outil recommandé pour les badges et la jauge
👉 **Canva.com** — gratuit, export PNG, fond transparent possible
