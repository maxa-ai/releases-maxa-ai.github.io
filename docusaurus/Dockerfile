FROM node:current-alpine AS builder

# Copy everything
WORKDIR /app
COPY . .

# Install and build
RUN yarn
RUN yarn build --out-dir releases-maxa-ai-static

# using nginx as web server
FROM nginx:stable-alpine-slim AS runner

# Copy nginx configuration for our needs
COPY nginx.conf /etc/nginx/conf.d/default.conf

# Move to workdir
WORKDIR /nginx
COPY --from=builder /app/releases-maxa-ai-static /nginx
