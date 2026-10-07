# Prêt à émettre 2027 — Diagnostic de préparation e-invoicing

Mini-business de **diagnostic de préparation à la facturation électronique** (obligation d'émission au 1er septembre 2027), pour TPE, PME, indépendants B2B, comptables et cabinets.

**URL live** : https://dembis91-940.github.io/einvoicing-2027/

## Positionnement

La réforme impose l'émission de factures électroniques au format structuré (Factur-X / UBL / CII) via une Plateforme Agréée (PDP) au 01/09/2027. Le marché des **outils** est saturé (Pennylane, Tiime, Freebe, Axonaut…) : on ne vend **pas un 22e logiciel**, on vend le **diagnostic de préparation** — l'accompagnement « je choisis quoi avant 2027 ? » que personne ne vend.

## Offres

- **Lead magnet gratuit** (capture email + téléchargement direct) : `pdf/checklist-preparation-2027.pdf` (12 points) + `pdf/comparatif-pdp-2027.pdf` (comparatif PDP par métier).
- **Diagnostic Essentiel — 290 €** : audit des flux, rapport de conformité, reco PDP courte.
- **Diagnostic Complet — 390 €** (le plus choisi) : + comparatif détaillé, plan de bascule daté, 30 min de restitution.
- **Accompagnement Bascule — 490 €** : + test Factur-X/UBL/CII sur factures réelles, suivi jusqu'à conformité.

## Structure

```
einvoicing-2027/
├── index.html            Landing (compte à rebours réel vers 01/09/2027, 3 offres, 2 formulaires EmailJS)
├── legale.html           Mentions légales & CGV
├── chatbot-config.js     14 FAQ spécifiques (prix, échéance, formats, sanctions), accent #1E6B4E
├── chatbot.js            Widget (version corrigée : texte lisible sur accent clair)
├── pdf/                  Lead magnets générés (checklist + comparatif PDP)
├── pdf-src/              Sources Markdown des PDF
└── README.md
```

## Flux de vente (réel, sans simulateur)

1. Le visiteur fait le point (compte à rebours, sanctions chiffrées, pièges).
2. Il télécharge le lead magnet (PDF réels) ou le reçoit par email (EmailJS → Gmail).
3. Il commande une prestation via le formulaire (EmailJS, payload = récapitulatif complet offre + prix).
4. L'éditeur recontacte sous 24 h ouvrées avec devis + lien de paiement (virement / DM).

## Identité visuelle (unique)

« Échéancier fiscal 2027 » : papier crème `#F6F1E6`, encre vert sapin `#0E2A20`, accent vert `#1E6B4E`, ambre échéance `#C8772B`, rouge sanction `#B3402A`. Typo Spectral + Inter + IBM Plex Mono. Motif signature : frise échéancier + compte à rebours réel.

## EmailJS

service `service_cy1ytdb` · template `template_xpo58cv` · clé publique `8Pui4ZEqxW2jRVF7h` · payload `{site, name, email, question}`.

## Sources

economie.gouv.fr · service-public.gouv.fr · impots.gouv.fr · formalites.lesechos.fr. Sanctions loi de finances 2026 : 50 €/facture non conforme (plafond 15 000 €/an), 500 €/e-reporting, 500 € puis 1 000 €/trimestre sans PDP après mise en demeure.

*Ce site est une aide à la préparation, pas un conseil juridique, fiscal ou comptable.*
