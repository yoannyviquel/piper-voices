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

## Pocket TTS (français)

| Fichier | Taille |
| --- | --- |
| `pocket-tts/fr/model.onnx.part00` à `part04` | 402 Mo en tout (morceaux de 95 Mo, GitHub refuse plus de 100 Mo par fichier) |
| `pocket-tts/fr/assets.json` | 0,9 Mo : tokeniseur, configuration, voix Estelle et Javert |
| `pocket-tts/fr/manifest.json`, `source.json` | provenance : dépôt, révision Hugging Face, sha256 du modèle entier, liste des morceaux |

- Copie sans modification de l'export ONNX [thewh1teagle/pocket-tts-onnx](https://huggingface.co/thewh1teagle/pocket-tts-onnx)
  (dossier `fr/`), faite par le workflow `.github/workflows/pocket-tts.yml`, qui fige la révision et
  vérifie l'empreinte. Les morceaux se recollent dans l'ordre (`cat model.onnx.part0* > model.onnx`).
- Modèle [Pocket TTS](https://github.com/kyutai-labs/pocket-tts) de Kyutai, sous licence
  [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/) ; export ONNX par thewh1teagle, CC BY 4.0.
