# ↓ 現時点のデフォルトイメージ
FROM mcr.microsoft.com/devcontainers/ruby:3.2

RUN apt update && \
  apt-get install --no-install-recommends -y \
  build-essential \
  default-libmysqlclient-dev \
  mariadb-client \
  libvips \
  pkg-config \
  git

# RUN su vscode -c "gem install rails:7.0.4.3"
RUN su vscode -c "/usr/local/rvm/bin/rvm fix-permissions"

WORKDIR "/workspaces/rails_devcontainer"
# RUN bundle install