FROM python:latest

RUN apt-get update && apt-get -y upgrade

# Switch to non-root user:
RUN useradd --create-home stan
WORKDIR /home/stan
USER stan

RUN pip install --upgrade cmdstanpy[all] arviz seaborn
RUN install_cmdstan
