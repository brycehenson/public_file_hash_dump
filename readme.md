This git contains some hashes of files which I would like to prove I that I have eg proof of existence.

# objectives
- difficulty to fake
  - Far more difficult than I have resources.
  - Best practice.
- reliability
  - not dependent on a single company or service running
  - long term ~10 years
  - able to survive multiple waves of inovation
  - on the user side need to store the unmodified file for as long as proof (obv).
- security
  - dont want to reveal file so must be able to give service only hash
  - could get arrount this requirement by uploading encrypted document to the hash service and then keeping the key

# Hashing
- use the most crypto secure hash to make collision very hard
- use multiple algos
  - hashcheck and 7z makes it trivial produce multple hashes CRC-32,SHA-1,SHA-256,SHA-512
- curretly using hashcheck

# Crypto solutions
using some kind of blockchain approach to store the file hash.
- [origin stamp](https://originstamp.com/) 
  - seems like a pretty good solution.
  - not dependent on company existing if the raw Merkle Tree is downaloded and bitcoin ledger exists
- [Proof of Existence](https://proofofexistence.com/)
  - currently charges 0.25 mBTC (~4 AUD) for each sorage
- [privatestamp](https://github.com/mustafarefaey/PrivateStamp) 
  - if usage is low long term reliability is hard
- [doc2block](https://doc2block.com/) adds to etherium, what is cost ? Not sure if just hash can be given to prevent sending file.

# public publish solutions
publish the hash on a public form that would take substantial effort to modify.
- github, is the commit hash secure?
- twitter
- facebook with permisions set to public
- archive.com

# encrypt and dump the file
- might be easy with small files.
- problems with how tamper resistant the hosting is, left with the same problem...
- hard to store large files

# private send solitions
- email hash or enc file to trusted & untrusted parties
  - more important that they will hang on to it for long enough
