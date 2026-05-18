# TODO

## Setup
- [ ] Decide on Python / framework versions (PyTorch vs. JAX)
- [ ] Add `pyproject.toml` / `requirements.txt` and pin dependencies
- [ ] Set up repo layout (`src/`, `configs/`, `scripts/`, `tests/`)
- [ ] Add `.gitignore` and initialize git
- [ ] Configure formatter / linter (ruff, black) and pre-commit hooks

## Data
- [ ] Choose driving dataset(s) (nuScenes, Waymo Open, NAVSIM, etc.)
- [ ] Write data loaders and preprocessing
- [ ] Define action / observation / future-state representations
- [ ] Split train / val / test and document the split

## Model
- [ ] Survey existing world-model work (GAIA-1, DriveDreamer, Vista, GenAD, DriveLaW)
- [ ] Define model interface: `(obs_t, action_t) -> obs_{t+1}` (or latent variant)
- [ ] Implement baseline tokenizer / encoder for camera + state
- [ ] Implement action-conditioned dynamics module
- [ ] Implement decoder / rollout

## Training
- [ ] Define training loop and loss (reconstruction, prediction, auxiliary)
- [ ] Add logging (wandb / tensorboard) and checkpointing
- [ ] Run small-scale overfit sanity check
- [ ] Scale to full dataset; track GPU / throughput

## Evaluation
- [ ] Define metrics: prediction fidelity, action consistency, planning score
- [ ] Compare against DriveLaW and other baselines
- [ ] Qualitative rollouts and failure-mode analysis

## Planning / downstream
- [ ] Use world model for action selection (MPC / search / learned policy)
- [ ] Closed-loop evaluation in simulator (e.g., CARLA / nuPlan)

## Docs
- [ ] Expand README with install + quickstart once stable
- [ ] Add architecture diagram
- [ ] Document configs and reproduce-this-run instructions
