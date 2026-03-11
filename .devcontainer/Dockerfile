FROM hegerdes/vscode-latex:latest

RUN sed -i 's/main/main contrib non-free non-free-firmware/g' /etc/apt/sources.list.d/debian.sources && \
    apt update -y && \
    apt install -y \
        ttf-mscorefonts-installer \
        texlive-lang-cyrillic \
        texlive-bibtex-extra \
        biber \
    apt clean && \
    rm -rf /var/lib/apt/lists/*