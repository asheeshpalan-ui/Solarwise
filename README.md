# Pixora Shield

Pixora Shield is a focused privacy MVP that uploads a video, detects faces, and
optionally detects license plates, then produces an MP4 with those regions
blurred.

By default, every detected face is blurred. Enable “Protect the main person”
in the frontend to keep the largest/tracked face visible and blur other faces.
Short detector misses are covered by frame-to-frame tracking. License plates are detected only by a
configured model: set `PLATE_MODEL_PATH` for local YOLO weights, or set
`ROBOFLOW_API_KEY`, `ROBOFLOW_MODEL_ID`, and optional `ROBOFLOW_VERSION` for a
hosted Roboflow model.

## Roboflow computer vision plugin

On the machine running Claude Code, add the official plugin once:

```powershell
claude plugin marketplace add roboflow/computer-vision-skills
claude plugin install roboflow
```

This plugin is for model selection, deployment, datasets, and inference
workflows. It does not make the uploaded video API detect plates by itself.

Processed videos are browser-ready MP4/H264. The backend uses bundled
`imageio-ffmpeg` to transcode OpenCV output when FFmpeg is not installed on the
system.

## Run locally

Backend:

```bash
python -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
python -m src.web.backend.run
```

Frontend:

```bash
cd src/web/frontend
npm install
npm run dev
```

Open `http://localhost:3000`. The API runs at `http://localhost:5000`.



