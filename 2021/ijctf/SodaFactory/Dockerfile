FROM node:19.0-buster-slim
WORKDIR /app
COPY ["package.json", "package-lock.json*", "./"]
RUN npm install
ENV FLAG SOLVE_MY_CHALL
ENV PORT 3000
COPY . .
CMD ["npm", "start"]
