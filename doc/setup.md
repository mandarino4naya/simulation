insert installation and config instructions here

For MacOS Silicon chip (M1-M4):

Anaconda use not recommended, use Poetry or virtual-env from here https://virtualenv.pypa.io instead

1) Create your conda env(#TODO):
```
conda create --name droids python=3.9
```
2) Activate
```
conda activate droids
```
3) For JAX installation (#TODO):

Refer to: https://developer.apple.com/metal/jax/
and the thread here: https://stackoverflow.com/questions/70815864/how-to-install-trax-jax-jaxlib-on-m1-mac-on-macos-12

4) For absl:
```
pip install absl-py
```
5) For BRAX installation (#TODO):
```
conda install -c conda-forge brax
```
Useful conda commands for verifying your setup:

conda list           | to list your packages in env
conda deactivate     | to exit your curr env