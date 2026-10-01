# piper-voices

Voix [Piper](https://github.com/rhasspy/piper) servies telles quelles par `raw.githubusercontent.com`,
pour l'app [Learning](https://github.com/yoannyviquel/learning) : sa dictée télécharge la voix au
premier lancement et la garde dans le navigateur. GitHub répond avec `access-control-allow-origin: *`,
là où Hugging Face peut être bloqué.

## Voix

| Fichier | Taille |
| --- | --- |
| `fr/fr_FR/siwis/medium/fr_FR-siwis-medium.onnx` | 69,8 Mo |
| `fr/fr_FR/siwis/medium/fr_FR-siwis-medium.onnx.json` | 5,8 Ko |

## Provenance et licence

- Copie sans modification de `voice-fr-siwis-medium.tar.gz`, release
  [`v0.0.2` de rhasspy/piper](https://github.com/rhasspy/piper/releases/tag/v0.0.2) (seuls les noms de
  fichiers suivent ceux de [rhasspy/piper-voices](https://huggingface.co/rhasspy/piper-voices)).
- Voix entraînée sur la [SIWIS French Speech Synthesis Database](https://datashare.is.ed.ac.uk/handle/10283/2353)
  (Honnet, Lazaridis, Garner, Yamagishi, 2017), sous licence
  [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/) : cf. `MODEL_CARD`.
