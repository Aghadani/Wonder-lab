# Wonder Lab Gravity Playground

A polished, browser based one-minute science experiment. Move a planet with your mouse, touch, or webcam hand tracking and watch its gravity bend the paths of passing probes. Adjust planet mass and probe speed, launch new probes, and explore.

## Publish with GitHub Pages

1. Create a **public** repository on [GitHub](https://github.com/new), for example `wonder-lab`.
2. Choose **Add file → Upload files** and upload the contents of this folder (`index.html`, `app.js`, `style.css`, `.nojekyll`, and `README.md`) to the repository root.
3. Commit the files.
4. Open **Settings → Pages**. Choose **Deploy from a branch**, select branch `main` and folder `/(root)`, then click **Save**.
5. Wait for the deployment. GitHub displays the published URL on the Pages settings screen. Open it over HTTPS.
6. Drag in the space scene to move the planet. Choose **Enable hand tracking** to steer it with your index fingertip. Allow camera access when prompted.

## Local preview

Camera access requires a secure context such as HTTPS or localhost. Run this in the project folder:

```bash
python -m http.server 8000
```

Then visit http://localhost:8000.

## Privacy and science notes

- Camera video is processed locally in the browser; the app does not upload it.
- On first use, the app downloads MediaPipe and its hand landmark model from jsDelivr and Google Cloud Storage. Fonts load from Google Fonts.
- The simulation is an interactive illustration for learning, not a scale-accurate orbital mechanics model.
