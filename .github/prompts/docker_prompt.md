create a docker file required to run tictactoe.ipynb notebook using template below:

	- use the official Microsoft python base image from mcr.microsoft.com/devcontainers/python:3.12
	- Install uv in a container by copying from ghcr.io/astral-sh/uv:latest to /uv /uvx /bin/
	- Run uv lock to generate the uv.lock file
	- ADD the .python-version, pyproject.toml and uvlock to container ./
	- sets the working directory /HVEAGENT2
	- Install packages from pyproject.toml via uv by using uv sync --frozen in container 
	- Run apt-get update
	- exposes port
	- start the uv run "--with juypter" and run jupyter notebook server

