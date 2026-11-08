# LIBERO-Pro display media

Public demonstration videos and preview images for the [LIBERO-Pro2.0 website](https://racingemperor.github.io/LIBERO-Pro2.0/).

This repository hosts 331 NORA perturbation recordings and their 331 WebP posters. Paths use the website's public model, task and perturbation IDs. Base recordings have not been supplied for NORA. The website presents the recordings at 2× playback speed; files retain their original frame rate and duration.

NORA videos are 640×640 exports enlarged from 256×256 policy observations, with their orientation matched to the website. They are demonstrations, not a source of leaderboard scores. Internal evaluation records and logs are not distributed here.

Pi0.5 recordings are hosted at `assets/rollouts/models/pi0-5-native640-20261029/`: 331 native 640×640, 20 fps front-view videos and WebP posters, covering every applicable perturbation across the eight evaluation tasks. Both successful and unsuccessful episodes are retained. The separate recording camera preserves the policy's official observation preprocessing, action horizon and episode limits. The website retains its existing Base clips and plays these demonstrations at 2×; the files retain their original frame rate and duration.

WorldVLA recordings are hosted at `assets/rollouts/models/worldvla/`: 331 native 640×640, 20 fps front-view videos and their WebP posters. Both successful and unsuccessful episodes are retained. These single-episode demonstrations do not replace the separate repeated evaluations used for leaderboard scores.

The Home overview film is served at `assets/promo/libero-pro2.0-overview-20261022.mp4`, with its poster at `assets/promo/libero-pro2.0-overview-opening-20261022.webp`. The supplied complete 90-second, 1920×1080, 30 fps film is preserved byte for byte without re-encoding. Home waits for Play before playing it with native sound and fullscreen controls.

GitHub Pages serves the files from the root of the `main` branch. Keep `.nojekyll` in place. The website's public media index is maintained in [LIBERO-Pro2.0](https://github.com/racingemperor/LIBERO-Pro2.0).

Training-task BASE demonstrations are hosted at `assets/rollouts/training/base/`: 32 native 640×640 X-VLA recordings and WebP posters. Each recording reaches the task's success condition. A 20 Hz simulation is encoded at 80 fps for uniform 4× playback, matching the website's Evaluation-task examples. The browser plays these files at 1×. Original actions, simulator state, run metadata and success-verification records are not published.

Training-data previews are hosted at `assets/rollouts/training/perturbations/`: 846 selected successful replay videos and their WebP posters, across 22 static shifts and 20 dynamic interventions. These compact 256×256, 20 fps videos replay recorded actions from the [public training dataset](https://huggingface.co/datasets/zhouxueyang/LIBERO-Pro2.0-Train) at revision `67b414109131ce92c2c0fc7e0d8e1d79cdc553b2`, without running a policy. Transformed camera observations retain visual and sensor interventions. This display selection does not change the dataset or represent evaluation scores. The website's training-media index specifies which previews are displayed.
