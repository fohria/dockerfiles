FROM python:latest

RUN apt-get update && apt-get -y upgrade

RUN pip install --upgrade cmdstanpy[all] arviz seaborn jupyter

ENV PATH="~/.local/bin:${PATH}"

RUN install_cmdstan
