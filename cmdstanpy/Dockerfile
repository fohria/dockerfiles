FROM python:latest

RUN apt-get update && apt-get -y upgrade

# Switch to non-root user:
RUN useradd --create-home stan
WORKDIR /home/stan
USER stan

RUN pip install --upgrade cmdstanpy[all] arviz seaborn
ENV PATH="/home/stan/.local/bin:${PATH}"
RUN install_cmdstan
