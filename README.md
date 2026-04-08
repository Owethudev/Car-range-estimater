# Car Range Estimater

Simple full-stack prototype to estimate how far older cars can drive given a certain amount of fuel, using mocked South African petrol prices and a toggle between `inland` and `coastal` zones.

Structure
- backend: FastAPI app (port 8000)
- frontend: Vite + React app (port 5173)

Quick start

1) Backend

Install Python dependencies and run backend:

```bash
python3 -m venv .venv
source .venv/bin/activate
pip install -r backend/requirements.txt
uvicorn backend.main:app --reload --port 8000
```

2) Frontend

Install node deps and run dev server:

```bash
cd frontend
npm install
npm run dev
```

Open the frontend URL shown by Vite (usually http://localhost:5173). The frontend calls the backend at `http://localhost:8000`.

What to extend
- Replace mocked `prices` in `backend/main.py` with live SA petrol price API if available.
- Expand `backend/cars.json` with more models and images.
- Add authentication or local persistence for user-saved cars.
# Car range estimater
modern cars give drivers a range of how far the car can travel based on the amount of fuel they have but older cars do not have that luxury and I will create an app to assist
