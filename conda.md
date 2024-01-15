# conda

## new environment

### yaml file

The environment name is chosen by the first line of the yaml file.(which is ```name: ENV_NAME```)

```bash
conda env create -f environment.yml
```

### empty environment

```bash
conda create --name ENV_NAME python
```

## check for all installed environments

```bash
conda env list
```

## look for a package

```bash
conda search PACKAGE_NAME
```

## check package version in a environment

```bash
conda list
```

## delete environment

```bash
conda remove --name ENV_NAME --all
```

## pip

install a specific version from github repo

```bash
pip install git+https://github.com/username/repo.git@1.2.3
```

## export environment to yaml

WARNING: the resulting yaml file contains a line metioning "prefix: ...\.conda\envs\ENV_NAME", showing your machine name and unique path to conda installation. Remember to remove it while publishing the yaml file.

```bash
conda env export > environment.yml
```

## remove unused packages

```bash
conda clean --all
```
