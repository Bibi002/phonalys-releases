# Phonalys

Logiciel pour les logopèdes : dossier patient, bilans, exercices et assistant de rédaction, **entièrement hébergés chez vous**.

- **Vos données restent au cabinet** : aucun compte en ligne, aucun envoi à l'éditeur, aucune télémétrie.
- **Sécurité** : coffre chiffré, connexion à deux facteurs (phrase de passe et biométrie), verrouillage automatique, journal d'audit.
- **IA locale uniquement** : l'assistant de rédaction utilise un modèle installé sur votre matériel (Ollama, LM Studio…). Les IA en ligne sont bloquées.
- **Windows, Linux, iPhone et Android** (ces deux derniers via le serveur du cabinet).

## Télécharger

👉 **[Dernière version](https://github.com/Bibi002/phonalys-releases/releases/latest)**

| Vous avez | Fichier |
|---|---|
| Windows | `Phonalys_<version>_x64-setup.exe` |
| Linux | `.deb`, `.rpm` ou `.AppImage` |
| Des téléphones ou tablettes à connecter | En plus, `phonalys-server-<version>-…` sur l'ordinateur du cabinet |

Avant d'installer, lisez le **[guide d'installation](INSTALLATION.md)** et vérifiez l'empreinte du fichier avec `SHA256SUMS.txt`.

> Les versions actuelles ne sont pas encore signées : Windows affiche un avertissement SmartScreen. N'installez que si l'empreinte correspond.

## Sécurité

Pour signaler une faille, voir [SECURITY.md](SECURITY.md).

## Licence

Logiciel **propriétaire**. Ce dépôt ne contient que les fichiers d'installation, pas le code source. Voir [LICENSE](LICENSE). © 2026 M. Baron.

Phonalys est un outil de gestion et d'aide à la rédaction : il ne pose aucun diagnostic et ne remplace pas le jugement du logopède.
