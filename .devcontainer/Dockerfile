FROM mcr.microsoft.com/devcontainers/base:ubuntu

# 必要なパッケージのインストール
RUN apt-get update && export DEBIAN_FRONTEND=noninteractive \
    && apt-get -y install --no-install-recommends \
    graphviz \
    default-jdk \
    nodejs \
    npm \
    texlive-latex-extra \
    texlive-fonts-extra \
    texlive-lang-japanese \
    pandoc \
    && apt-get clean \
    && rm -rf /var/lib/apt/lists/*

# Node.jsのバージョン管理ツールのインストール
RUN npm install -g n \
    && n stable

# npmのグローバルインストール先をユーザーディレクトリに変更
ENV NPM_CONFIG_PREFIX=/home/vscode/.npm-global
ENV PATH=/home/vscode/.npm-global/bin:$PATH

# PlantUMLのインストール
RUN mkdir -p /opt/plantuml \
    && curl -L https://sourceforge.net/projects/plantuml/files/latest/download -o /opt/plantuml/plantuml.jar

# 環境変数の設定
ENV PLANTUML_JAR=/opt/plantuml/plantuml.jar

# ユーザー設定
USER vscode
WORKDIR /workspace

# npmのグローバルディレクトリを作成
RUN mkdir -p /home/vscode/.npm-global 