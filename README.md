<h2 align=center>Aligned zkQuiz NFT</h2>

![Img1](https://github.com/user-attachments/assets/4e323dd3-cdee-44be-b62c-f18253da6446)

- Download Rust
```bash
source <(wget -O - https://raw.githubusercontent.com/zunxbt/installation/main/rust.sh)
```
- Download Foundry
```bash
source <(wget -O - https://raw.githubusercontent.com/zunxbt/installation/main/foundry.sh)
```
- Install OpenSSL and pkg-config
```bash
sudo apt update && sudo apt install pkg-config libssl-dev
```
- Import a burner wallet that have Holesky ETH
```bash
[ -d ~/.aligned_keystore ] && rm -rf ~/.aligned_keystore && echo "Deleted existing directory ~/.aligned_keystore." ; mkdir -p ~/.aligned_keystore && cast wallet import ~/.aligned_keystore/keystore0 --interactive
```
- Clone Aligned Layer repo
```bash
[ -d aligned_layer ] && rm -rf aligned_layer && echo "Deleted existing aligned_layer directory." ; git clone https://github.com/yetanotherco/aligned_layer.git && cd aligned_layer/examples/zkquiz
```
- Run this final command
```bash
make answer_quiz KEYSTORE_PATH=~/.aligned_keystore/keystore0
```
- In the last stage it will ask some questions, here is the answers

`y` , `c` , `c` , `a` , `y`
