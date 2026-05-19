# Gibberlink Glossary

## Lexique canonique du Gibberlink

**Version :** 0.1 - Base terminologique  
**Auteur :** Xavier Fleriag / Twins Productions  
**Statut :** Glossaire de consolidation  
**Perimetre :** Gibberlink uniquement

---

## 1. Objet du glossaire

Ce glossaire fixe les termes essentiels du Gibberlink afin d'eviter les confusions entre symbole, etat, flux, priorite et interpretation.

Regle generale :

```text
Gibberlink = langage symbolique compact d'etats
```

Il sert a lire les documents et exemples lies aux fichiers `.glg`.

---

## 2. Termes fondamentaux

### Gibberlink

Langage symbolique compact destine a representer des etats, des vecteurs, des glyphes, des flux et des priorites sous une forme courte et routable.

Formule canonique :

```text
Gibberlink = etat + symboles + flux + priorite
```

---

### .glg

Extension de fichier associee aux contenus Gibberlink.

Un fichier `.glg` peut contenir un etat, un protocole, une signature symbolique ou une representation compacte d'execution.

---

### STATE

Bloc representant un etat courant, un etat de sortie ou une signature compacte d'execution.

Exemple :

```text
STATE {
  vectors: <A|B|C>
  energy_flux: PHI(1->2) = +DELTA
  priority: MEDIUM
}
```

---

### Vectors

Sequence compacte de symboles, marqueurs ou identifiants.

Role : porter une signature symbolique courte.

Exemple :

```text
vectors: <KA|SIGMA|PI|LAMBDA>
```

---

### Glyphe

Marqueur symbolique pouvant porter un sens compact.

Un glyphe ne doit pas etre traite comme une preuve. Il represente un signal, une route, une signature ou une intention symbolique.

---

### Glyph marker

Marqueur de glyphe utilise dans un vecteur ou un etat.

Exemple :

```text
KA
SIGMA
PI
LAMBDA
```

---

### Flux

Mouvement, transition ou passage d'un etat vers un autre.

Forme simple :

```text
source -> target
```

---

### Energy flux

Representation d'une variation ou transition symbolique.

Exemple :

```text
energy_flux: PHI(5->9) = +DELTA
```

Role : indiquer une transformation, une intensification ou un mouvement.

---

### PHI

Marqueur utilise pour exprimer un flux ou une fonction de transition.

Dans ce glossaire, PHI est traite comme un symbole de flux, pas comme une preuve scientifique.

---

### DELTA

Marqueur de variation.

Exemples :

```text
+DELTA = augmentation ou transition positive
-DELTA = reduction ou transition negative
```

---

### Priority

Niveau d'importance ou d'attention associe a un etat.

Exemples :

```text
LOW
MEDIUM
MEDIUM_PLUS
HIGH
CRITICAL
```

Role : orienter le niveau de traitement.

---

### EXEC_STATE

Etat d'execution emis par un protocole ou un processus Gibberlink.

Il peut contenir :

```text
vectors
energy_flux
priority
```

---

### Signal

Information compacte transmise par un symbole, un vecteur, un flux ou une priorite.

Le signal doit rester lisible dans son contexte.

---

### Signature symbolique

Combinaison courte de marqueurs permettant de reconnaitre un etat ou une orientation.

Exemple :

```text
<INTENT|GLYPH|ROUTE|OUTPUT>
```

---

### Route

Direction de traitement ou orientation d'un flux.

Une route peut etre explicite :

```text
A -> B
```

Ou implicite dans un vecteur ou un etat.

---

## 3. Distinctions importantes

### Gibberlink vs langage naturel

```text
Langage naturel = explication
Gibberlink = condensation symbolique
```

Le langage naturel explique. Gibberlink encode un etat.

---

### Gibberlink vs JSON

```text
JSON = structure explicite
Gibberlink = etat symbolique compact
```

JSON organise. Gibberlink condense.

---

### Symbole vs preuve

Un symbole represente un etat, une route, une priorite ou une signature.

Il ne constitue pas une preuve factuelle par lui-meme.

Regle canonique :

```text
Un symbole signale. Il ne prouve pas.
```

---

### Compression vs opacite

Gibberlink cherche la compacite, mais ne doit pas devenir illisible ou arbitraire.

Regle canonique :

```text
Compacter assez pour router. Ne pas compacter au point d'obscurcir.
```

---

## 4. Formules canoniques

```text
Gibberlink = etat symbolique compact
```

```text
Gibberlink = vectors + energy_flux + priority
```

```text
STATE = bloc d'etat
```

```text
vectors = signature symbolique
```

```text
energy_flux = transition ou variation
```

```text
priority = niveau d'attention ou de traitement
```

```text
symbole = signal, pas preuve
```

---

## 5. Regles d'ecriture recommandees

### Regle 1 - Utiliser des blocs courts

Un bloc Gibberlink doit rester compact.

### Regle 2 - Nommer l'etat

Utiliser `STATE` lorsqu'un etat doit etre represente.

### Regle 3 - Garder les vecteurs lisibles

Les vecteurs doivent etre courts et separables.

### Regle 4 - Expliciter la priorite

Si la priorite influence le traitement, elle doit etre presente.

### Regle 5 - Ne pas utiliser les symboles comme preuves

Un symbole indique un signal. Il ne remplace pas une source ou une verification.

### Regle 6 - Eviter la prose longue

Gibberlink n'est pas fait pour devenir un paragraphe naturel.

---

## 6. Exemple minimal

```text
STATE {
  vectors: <A|B|C>
  energy_flux: PHI(1->2) = +DELTA
  priority: MEDIUM
}
```

Lecture :

```text
Etat compact avec trois marqueurs, transition positive et priorite moyenne.
```

---

## 7. Exemple de signature

```text
STATE {
  vectors: <INTENT|GLYPH|ROUTE|OUTPUT>
  energy_flux: PHI(source->target) = +DELTA
  priority: HIGH
}
```

Lecture :

```text
Etat oriente execution avec priorite haute.
```

---

## 8. Conclusion

Le Gibberlink est une langue de signal compact.

Il ne cherche pas a tout expliquer. Il cherche a transporter vite un etat symbolique.

Formule finale :

```text
Gibberlink condense.
Gibberlink signale.
Gibberlink route.
```
