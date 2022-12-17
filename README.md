# Blockchain Demo
A web-based demonstration of blockchain concepts.

[![Blockchain 101 - Demo](https://img.youtube.com/vi/_160oMzblY8/0.jpg)](https://www.youtube.com/watch?v=_160oMzblY8)

This is a very basic visual introduction to the concepts behind a blockchain. We introduce 
the idea of an immutable ledger using an interactive web demo that is available here:

http://andersbrownworth.com/blockchain/

## Setup
Get the code:

```
git clone https://github.com/anders94/blockchain-demo.git
```

Install dependencies:

```
cd blockchain-demo
npm install
```
Run the server:

```
npm start
```

OR

```
./bin/www
```
#For windows: if the above command didn't work, use this (make sure you have Node.js installed in your system):
```
node ./bin/www      
```

Point a web browser at the demo:

```
http://localhost:3000
```

## Setup using Docker

Get the code:

```
git clone https://github.com/anders94/blockchain-demo.git
```

Run the Docker setup:

```
cd blockchain-demo
docker-compose up -d
```

Point a web browser at the demo:

```
http://localhost:3000
```

## Optional Configuration
You can adjust the "number of zeros" required by the demo by editing the first two lines of
`public/javascripts/blockchain.js`.

Because there are 16 possible characters in a hex value, each time you increment the difficulty
by one you make the puzzle 16 times harder. In my testing, a difficulty of 6 requires a
maximumNonce well over 500,000,000.



