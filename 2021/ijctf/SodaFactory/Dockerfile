FROM node:19.0.0
WORKDIR /app
COPY ["package.json", "package-lock.json*", "./"]
RUN npm install
ENV FLAG SOLVE_MY_CHALL
ENV PORT 3000
COPY . .
CMD ["npm", "start"]
