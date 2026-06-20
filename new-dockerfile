FROM registry.access.redhat.com/ubi8/nodejs-18
WORKDIR /opt/app-root/src
COPY --chown=1001:0 package*.json ./
RUN npm install
COPY --chown=1001:0 . .
EXPOSE 3000
CMD ["node", "app.js"]
