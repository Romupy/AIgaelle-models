# Modèles d'AIgaelle — RomutechAI

Ce dépôt contient les modèles que l'application **AIgaelle** (RomutechAI) télécharge toute seule.
Les fichiers se trouvent dans les **Releases**, une par version de modèle (par exemple `robin_model-1.0`).
La release `catalog` contient leur liste, signée par RomutechAI : AIgaelle refuse tout autre catalogue
et vérifie chaque fichier (SHA-256) avant de l'utiliser.

- **Modèles RomutechAI** (`robin_model`, `robin_model_small`, `robin_model_large`) : chiffrés (AES-256).
  Ils ne fonctionnent qu'avec une licence AIgaelle.
- **Modèles publics**, fournis tels quels avec l'accord de leur licence :

| Modèle | Auteur | Licence | Modification |
|---|---|---|---|
| Whisper large-v3-turbo | OpenAI (conversion MLX : mlx-community) | MIT ([texte](LICENSE-MIT-WHISPER.txt)) | aucune |
| Kokoro 82M, voix ff_siwis | hexgrad ; corpus SIWIS (University of Edinburgh) | Apache 2.0 ; voix CC BY 4.0 | aucune |
| Z-Image-Turbo | Z-Image Team (Tongyi-MAI, Alibaba) | Apache 2.0 | quantifié en 8 bits (mflux-community) |
| FastWan 2.1 T2V 1.3B | FastVideo Team (Hao AI Lab) ; Wan Team (Alibaba) | Apache 2.0 | compressé par RomutechAI (texte 4 bits, vidéo 8 bits) |

Les modèles RomutechAI sont issus de modèles sous licence Apache 2.0 et ajustés par RomutechAI
(entraînement LoRA léger). Texte de la licence Apache 2.0 : [LICENSE-APACHE-2.0.txt](LICENSE-APACHE-2.0.txt).

Contact : https://romutechai.fr
