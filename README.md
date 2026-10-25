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

## Vérifier l'authenticité (facultatif, pour les informaticiens)

Chaque version est signée automatiquement avec [Sigstore](https://www.sigstore.dev) et porte une attestation de provenance GitHub. La signature prouve que les fichiers ont été publiés par ce dépôt et n'ont pas été modifiés.

Avec l'outil [GitHub CLI](https://cli.github.com) :

```sh
gh attestation verify Phonalys_<version>_x64-setup.exe -R Bibi002/phonalys-releases
```

Avec [cosign](https://docs.sigstore.dev/cosign/system_config/installation/) :

```sh
cosign verify-blob SHA256SUMS.txt --bundle SHA256SUMS.txt.sigstore.json \
  --certificate-oidc-issuer https://token.actions.githubusercontent.com \
  --certificate-identity-regexp '^https://github\.com/Bibi002/phonalys-releases/\.github/workflows/signer\.yml@'
sha256sum --check --ignore-missing SHA256SUMS.txt
```

## Sécurité

Pour signaler une faille, voir [SECURITY.md](SECURITY.md).

## Licence

Logiciel **propriétaire**. Ce dépôt ne contient que les fichiers d'installation, pas le code source. Voir [LICENSE](LICENSE). © 2026 M. Baron.

Phonalys est un outil de gestion et d'aide à la rédaction : il ne pose aucun diagnostic et ne remplace pas le jugement du logopède.
