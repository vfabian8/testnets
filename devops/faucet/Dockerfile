# The only officially supported distribution channel of the faucet binary is @cosmwasm/faucet on npmjs.com

# Choose from https://hub.docker.com/_/node/
FROM node:12.14.1-alpine

RUN yarn global add @cosmjs/faucet@0.24.0-alpha.9

# Check it exists
RUN /usr/local/bin/cosmos-faucet version

EXPOSE 8000
CMD ["/usr/local/bin/cosmos-faucet", "start", "http://localhost:1317"]
