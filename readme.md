This git contains some hashes of files which I would like to prove I that I have.

# objectives
- difficulty to fake
  - Far more difficult than I have resources.
  - Best practice.
- reliability
  - not dependent on a single company or service running
  - long term ~10 years
  - able to survive multiple waves of inovation
- security
  - dont want to reveal file so must be able to give service only hash
  - could get arrount this requirement by uploading encrypted document to the hash service and then keeping the key

# Hashing
- use the most crypto secure hash to make collision very hard
- use multiple algos
  - hashcheck makes it trivial to get CRC-32,SHA-1,SHA-256,SHA-512
- curretly using hashcheck

# Crypto solutions
using some kind of blockchain approach to store the file hash.
- [privatestamp](https://github.com/mustafarefaey/PrivateStamp) if usage is low long term reliability is hard
- [origin stamp](https://originstamp.com/) seems like a pretty good solution but if the company goes under so does the proof. Maybe the hash directory can be downloaded.
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
