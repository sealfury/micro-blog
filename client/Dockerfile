FROM node:alpine

# overcome create-react-app bug w/r/t docker
ENV CI=true

WORKDIR /app
COPY package.json ./
RUN npm install
COPY ./ ./

CMD ["npm", "start"]