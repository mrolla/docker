FROM debian:jessie
MAINTAINER Matteo Rolla

# Install base packages
RUN apt-get update && \
    DEBIAN_FRONTEND=noninteractive apt-get --no-install-recommends -yq install \
        make \
        git \
        python-pip \
        texlive \
        texlive-latex-recommended \
        texlive-latex-extra \
        texlive-fonts-recommended \
    && rm -rf /var/lib/apt/lists/*

# Install Sphinx
RUN pip install Sphinx sphinx_bootstrap_theme sphinxcontrib-httpdomain

WORKDIR /doc