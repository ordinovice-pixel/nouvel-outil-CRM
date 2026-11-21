## Ce que fait l'outil

```mermaid
flowchart LR
    OUTIL(["📱 <b>Outil OrdiNovice</b><br/>sur téléphone et sur PC"])

    OUTIL --- A["👤 <b>Fiche client</b><br/>Tout l'historique en un coup d'œil"]
    OUTIL --- B["⚡ <b>Saisie express</b><br/>« Je sors de chez un client » : 1 minute"]
    OUTIL --- C["📷 <b>Chèque en photo</b><br/>Lu par l'IA, paiement prérempli"]
    OUTIL --- D["⏱️ <b>Crédit temps et maintenances</b><br/>Minutes décomptées, appels planifiés"]
    OUTIL --- E["✉️ <b>Factures et e-mails</b><br/>Facture, merci et avis Google en un clic"]
    OUTIL --- F["🔔 <b>Rappels et récap du matin</b><br/>Plus d'oubli"]
    OUTIL --- G["📊 <b>Tableau de bord</b><br/>CA et plafond micro-entreprise"]
    OUTIL --- H["📣 <b>Communication et parrainage</b><br/>La bonne offre aux bons clients"]

    classDef hub fill:#1E5AA8,color:#fff,stroke:#1E5AA8
    classDef c1 fill:#E6EEF9,stroke:#1E5AA8,color:#1C2430
    classDef c2 fill:#E2F4F1,stroke:#17705F,color:#1C2430
    classDef c3 fill:#FDF1DC,stroke:#9A5B00,color:#1C2430
    classDef c4 fill:#EEE9FA,stroke:#5B3FB0,color:#1C2430
    classDef c5 fill:#FBE8EE,stroke:#A3264F,color:#1C2430
    classDef c6 fill:#FDEBDD,stroke:#A44A0B,color:#1C2430
    classDef c7 fill:#E7F4E4,stroke:#2F6B24,color:#1C2430
    classDef c8 fill:#E3F2FB,stroke:#11608F,color:#1C2430
    class OUTIL hub
    class A c1
    class B c2
    class C c3
    class D c4
    class E c5
    class F c6
    class G c7
    class H c8
```

> Fonctionne avec Google Agenda, Drive, Gmail, Contacts et Tâches · **Gratuit** (seule la lecture des chèques par l'IA coûte quelques centimes) · **Données privées** dans Google Drive, sauvegardées chaque semaine.

## Comment ça marche : une intervention, du début à la fin

```mermaid
flowchart LR
    subgraph MOI["🙋 Moi, sur mon téléphone"]
        direction LR
        M1["Je note le RDV<br/><i>Google Agenda</i>"] --> M2["Chez le client<br/>« Je sors de chez un client »"] --> M3["Photo du chèque"] --> M4["Je vérifie et je valide"]
    end
    subgraph AUTO["⚙️ L'outil, tout seul"]
        direction LR
        A1["8 h 00 : récap du jour"]
        A2["Pense-bête : chargeur, clés…"]
        A3["Lit le chèque, signale l'e-mail manquant"]
        A4["Met tout à jour : fiche, crédit temps,<br/>maintenance, Google Contacts"] --> A5["Dit merci + lien avis Google"]
    end
    subgraph SORT["✅ Ce qui en sort"]
        direction LR
        R1["Récap reçu dans Gmail"]
        R4["Facture PDF rangée dans Drive<br/>et envoyée par Gmail"]
        R5["Tableau de bord à jour"]
    end
    M1 --> A1 --> R1
    M2 --> A2
    M3 --> A3
    M4 --> A4 --> R4
    A5 --> R5

    classDef auto fill:#1E5AA8,color:#fff,stroke:#1E5AA8
    classDef res fill:#fff,stroke:#2F8F5B,stroke-width:2px,color:#1C2430
    class A1,A2,A3,A4,A5 auto
    class R1,R4,R5 res
```

> **Et le lendemain ?** Un RDV noté dans l'agenda mais rien de saisi dans l'outil : il me le rappelle.
