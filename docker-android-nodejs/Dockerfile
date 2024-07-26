FROM slarrieu/docker-android:12.1

# Set the environment variables to avoid interaction during installation
ENV DEBIAN_FRONTEND=noninteractive

# Install dependencies
RUN apt-get update && apt-get install -y \
    curl \
    gnupg \
    ca-certificates \
    && rm -rf /var/lib/apt/lists/*

# Add NodeSource signing key and NodeSource repository for Node.js 20.x
RUN curl -fsSL https://deb.nodesource.com/setup_20.x | bash -

# Install Node.js and npm
RUN apt-get install -y nodejs

# Verify installation
RUN node -v && npm -v &&  npm install -g yarn && yarn -v

