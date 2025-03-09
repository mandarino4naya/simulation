insert installation and config instructions here

For MacOS Silicon chip:

Anaconda use NOT recommended, use miniforge3 (install [here](https://github.com/conda-forge/miniforge))

1) Activate miniforge3 on your path:
`~/miniforge3/bin/conda init zsh`

2) Create your conda miniforge3 env:
`conda create -n droids python=3.12`

3) Activate env
`conda activate droids`

4) Check that your Python is arm64 (for libraries compatibility)
`lipo -archs $(which python3)`

If you don't have homebrew, install [here](https://brew.sh/)

5) Use homebrew to install cmake and gcc dependencies first:
`brew install cmake gcc `

Now, install a bunch of libraries you need:

`pip install mujoco`        phys simulation
`pip install -U jax`        CPU-only version of JAX
`pip install brax`          parallel phys simulation
`pip install mediapy`       visuals
`pip install wandb`         AI dev tool
`pip install playground`    robotics learning sim-to-real

Extra stuff you might need:
`pip install torch`
`pip install dm_control`

Useful conda commands for verifying your setup:

conda list           | to list your packages in env
conda env list       | to list your existing envs
conda deactivate     | to exit your curr env