# POWERUP

POWERUP is a platform for generating predictive models from large reference datasets and applying them to new user samples. It produces probabilistic predictions that capture uncertainty and, when experimental observations are available, integrates these with model-derived priors to compute updated posterior estimates. The system supports job-based execution, preprocessing, sharded model training, aggregate result generation, and optional observation-based follow-up analyses.

## What POWERUP does

At a high level, POWERUP:

1. accepts a user matrix as input,
2. preprocesses the matrix against a reference dataset,
3. trains, scores, and applies many per-perturbation models,
4. generates aggregate outputs such as predictions and feature contributions,
5. optionally integrates experimental data to produce posterior probabilities.


## Main components

The POWERUP collection includes:

- a core R package for training and applying models
- a set of helper functions to assist with data preprocessing, batch execution, and plotting
- a backend API for job creation, monitoring, and parallel execution
- a web-based frontend for launching analyses and exploring results.


## Documentation map

- [Getting Started](getting-started.md)
- [Architecture](architecture.md)
- [Inputs and Outputs](inputs-and-outputs.md)
- [API](api.md)
- [Observations](observations.md)
- [Reproducibility](reproducibility.md)