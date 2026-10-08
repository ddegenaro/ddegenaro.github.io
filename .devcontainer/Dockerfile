FROM mcr.microsoft.com/devcontainers/jekyll

# The base image's Yarn apt repo has a missing/expired signing key, which
# breaks `apt-get update` for anything that runs after. Drop the repo.
# (This doesn't uninstall yarn itself if the image already includes it.)
RUN rm -f /etc/apt/sources.list.d/yarn.list