# LIBERO-Pro display media

Public demonstration videos and preview images for the [LIBERO-Pro2.0 website](https://racingemperor.github.io/LIBERO-Pro2.0/).

This repository hosts 331 NORA perturbation recordings and their 331 WebP posters. Paths use the website's public model, task and perturbation IDs. Base recordings have not been supplied for NORA. The website presents the recordings at 2× playback speed; files retain their original frame rate and duration.

Videos are 640×640 exports enlarged from 256×256 policy observations, with their orientation matched to the website. They are demonstrations, not a source of leaderboard scores. Internal evaluation records and logs are not distributed here.

The Home overview film is served at `assets/promo/libero-pro2.0-overview-20261022.mp4`. Its 1920×1080 poster, `assets/promo/libero-pro2.0-overview-opening-20261022.webp`, comes from 2.8 seconds, showing the full opening title after the initial blank frame. This October 22 replacement is the supplied complete 90-second, 1920×1080, 30 fps film, preserved byte for byte without re-encoding: H.264 High video, stereo AAC audio and a front-loaded MP4 index. The previous 1080p and 1440p files and the earlier poster remain at their existing paths. Home buffers the current film as the visitor approaches the player, then waits for Play before showing motion or playing audio, with native sound and fullscreen controls. Production audits and internal episode records are excluded.

GitHub Pages serves the files from the root of the `main` branch. Keep `.nojekyll` in place. The website's public media index is maintained in [LIBERO-Pro2.0](https://github.com/racingemperor/LIBERO-Pro2.0).

Training-task BASE demonstrations are hosted at `assets/rollouts/training/base/`: 32 native 640×640 X-VLA recordings and WebP posters. Each recording reaches the task's success condition. A 20 Hz simulation is encoded at 80 fps for uniform 4× playback, matching the website's Evaluation-task examples. The browser plays these files at 1×. Original actions, simulator state, run metadata and success-verification records are not published.

Training-data previews are hosted at `assets/rollouts/training/perturbations/`: one recording per released task–perturbation pair, across 22 static shifts and 20 dynamic interventions. These compact 256×256, 20 fps videos replay recorded actions from the [public training dataset](https://huggingface.co/datasets/zhouxueyang/LIBERO-Pro2.0-Train) at revision `67b414109131ce92c2c0fc7e0d8e1d79cdc553b2`, without running a policy. Transformed camera observations retain visual and sensor interventions. Successful and unsuccessful replays are both retained; previews illustrate training coverage and are not evaluation results. Each distinct task is assigned to one of five rows with alternating right/left/right/left/right motion. Visual copies make the rows loop without counting as additional demonstrations. Home uses its existing media.
