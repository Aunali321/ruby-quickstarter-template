FROM mcr.microsoft.com/vscode/devcontainers/base:jammy

# Install Ruby
RUN apt-get update && apt-get install -y ruby-full build-essential

# Switch to root to install gems globally
USER root

# Clean up
RUN apt-get autoremove -y && apt-get clean -y && rm -rf /var/lib/apt/lists/*