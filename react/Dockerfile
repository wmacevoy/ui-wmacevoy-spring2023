# Build: docker build -t js .
# Run: docker run -v "$PWD:/app" -p 3000:3000 -t js

FROM node:14-alpine

RUN mkdir /app
WORKDIR /app
EXPOSE 3000


# RUN yarn install --production
CMD ["/bin/sh","-c","(test -f client/package.json || npx create-react-app client) && (cd client && yarn install --production && npm start)"]
