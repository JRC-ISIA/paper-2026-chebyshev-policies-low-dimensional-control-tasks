# Chebyshev Policies and the Mountain Car Problem: Reinforcement Learning for Low-Dimensional Control Tasks

![ICML 2026 Spotlight](https://img.shields.io/badge/ICML%202026-Spotlight-blue)

> **Disclaimer:** This repository reflects the exploratory and iterative nature of research code developed over two years alongside the scientific process. It is released in the exact form used to produce the published results, with reproducibility taking precedence over refactoring, optimization, or style consistency.

## Citation

If you use this code, please cite:

```bibtex
@inproceedings{HUSR26,
  title     = {Chebyshev Policies and the Mountain Car Problem: Reinforcement Learning for Low-Dimensional Control Tasks},
  author    = {Huber, Stefan and Unger, Hannes and Sch{\"a}fer, Georg and Rehrl, Jakob},
  booktitle = {Proceedings of the 43rd International Conference on Machine Learning (ICML 2026)},
  year      = {2026},
  address   = {Seoul, South Korea},
  note = {Spotlight Paper}
}
```

> Huber, S., Unger, H., Schäfer, G., and Rehrl, J. Chebyshev Policies and the Mountain Car Problem: Reinforcement Learning for Low-Dimensional Control Tasks. In Proceedings of the 43rd International Conference on Machine Learning (ICML 2026), Seoul, South Korea, 2026. Spotlight Paper.

## Structure

| Path | Contents |
|---|---|
| `notebooks 01–04` | Training and evaluation experiments discussed in the paper. 01 and 02: MountainCarContinuous-v0, 03: Pendulum-v1, 04: Quanser Aero 2 |
| `algorithms/` | Approximators, RL algorithms, wrappers |
| `utils/` | Experiment execution utilities |
| `rl-trained-agents/` | Mountain Car SOTA baseline agents pulled from rl-zoo |
| `rlzoo-pendulum-trained-agents/` | Pendulum SOTA baseline agents pulled from rl-zoo |

## Dependencies: Linked Repositories

This project requires two companion packages, installed via local editable install:

| Package | Repository | Description |
|---|---|---|
| `aero-envs` | [aero-envs](https://github.com/yourorg/aero-envs) | Custom Quanser Aero 2 Gymnasium environment |
| `polynomial-rl-agents` | [polynomial-rl-agents](https://github.com/JRC-ISIA/polynomial-sb3-rl-agents) | Polynomial policy Stable Baselines3 agents |

## Requirements

- Python 3.10
- Jupyter Notebook / JupyterLab
- See `requirements.txt` for full dependencies