SDR-GS anonymous project website

PREVIEW
Open a terminal in this folder and run:
  python3 -m http.server 8080 --bind 127.0.0.1
Then open http://127.0.0.1:8080
Use HTTP rather than double-clicking index.html so the supplement index loads.

GITHUB PAGES
This package has not been published and no domain has been registered.
To obtain a root URL ending in github.io:
1. Create an anonymous GitHub account with a neutral username of your choice.
2. Create a public repository named exactly <username>.github.io.
3. Upload the CONTENTS of this folder to the repository root using Git.
4. In Settings > Pages, select Deploy from a branch, main, / (root).
5. The published address will be https://<username>.github.io/.
A suggested name is sdr-gs-anonymous, subject to availability; it is not reserved.
A project repository instead uses https://<username>.github.io/<repository>/.
Relative URLs in this package support either layout.

From this folder, after creating your repository:
  git init
  git add .
  git commit -m "Add anonymous SDR-GS project page"
  git branch -M main
  git remote add origin https://github.com/<username>/<username>.github.io.git
  git push -u origin main
Replace both <username> values. Authentication is handled by your own Git client.
No account, token, or remote is configured in this package.

LARGE FILES
Use Git rather than the browser file uploader: some assets exceed 25 MB.
Every individual file is below GitHub's 100 MiB Git object limit.
The top Video button opens https://www.youtube.com/watch?v=rcPl8J7DGG8.
Scene comparison clips and hero clips are web delivery encodes of actual renders.

ANONYMITY
Visible authorship is "Anonymous authors". No institution, personal profile,
email, analytics, or remote font requests are included.
There is no embedded presentation section.
PDF metadata is set to anonymous. Literature citations in the manuscript remain.
The page includes no fake DOI, arXiv identifier, code URL, or live deployment URL.
robots noindex is enabled for the review version; remove after de-anonymization.
A github.io hostname depends on the account name you select, so use a neutral
account rather than a personal account for anonymous review.

CONTENT
Paper, two-stage pipeline, 13-scene benchmark, component ablations, seven matched-view three-method image comparisons, and six videos spanning four dataset groups.
The page's benchmark table comes from the supplied paper. Video overlays retain
native per-frame measurements; those are not identical aggregation protocols.
The 7.3x matched-quality claim is not a ratio of the table's FPS entries.
No 3D model viewer is claimed; the scene explorer plays real rendered comparisons.
Code and models are not linked because no anonymous public repository was supplied.

DESIGN REFERENCES
Background, centered academic header and alternating section layout:
https://sketchvideo.github.io/
Scene navigation, interactive comparisons and methodological organization:
https://derthomy.github.io/SteadySplats/
The implementation is independently written; no reference-site media is copied.

THREE-METHOD COMPARISONS
The hero and image explorer use two draggable dividers, ordered left-to-right:
StochasticSplats, SteadySplats, Ours. Ours denotes the full method including WOIT.
Seven still-image scenes: Garden, Bonsai, Counter, Stump, Playroom, Room, Dr. Johnson.
SteadySplats uses the foreground-only lambda=1 representation (fg_raw), not the
warmed K4N4 output. All three methods use one fresh SPP with no temporal history.
The new hero StochasticSplats video is rendered from vanilla 3DGS with exactly
the same camera poses as the existing SteadySplats hero (240 matched camera frames; the atlas normalizes all sources to 30 fps).

Unused local presentation and supplement downloads are not included in this
upload package because the presentation is linked on YouTube and the supplementary
material section was removed. The standalone source files remain in the workspace.

The hero uses one synchronized video atlas, not three independent players.
All sources are aligned by frame number and encoded at 30 fps (240 frames).
A single native video decoder supplies all three comparison regions, ensuring
both smooth playback and exact temporal alignment. No per-frame seeking is used.
The Pipeline section immediately follows Abstract.
