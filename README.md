# POLYMER--IBCCHANNEL-NODE


# POLYMER-IBC-NODE

<h1 align="center"> POLYMER | IBC CHANNEL TESNET </h1>

<div align="center"

![image](https://github.com/Volkan081/POLYMER-IBC-NODE/assets/95221293/dbcc795f-b44a-41b3-a3f4-2f04a1d4287e)



   
     
# [Website](https://www.polymerlabs.org/) | [Twitter](https://twitter.com/Polymer_Labs) | [Discord](https://discord.gg/hvMQp4qcM6) | [Github](https://github.com/polymerdevs) | [Docs](https://docs.polymerlabs.org/)

 </div>

#

### Sistem Gereksinimleri

| Bileşenler | Minimum Gereksinimler | 

Herhangi bir suncu olabilir node yanına kurulabilir


### Linkler

https://github.com/Volkan081

https://twitter.com/BerraVolkan





     
-Dosyaları indirip kitaplıkları kuruyoruz

```
sudo apt update -y && sudo apt upgrade -y sudo apt-get install git -y sudo apt-get install -y ca-certificates curl gnupg sudo mkdir -p /etc/apt/keyrings

```



-Dosya hazırlıklarına devam ediyoruz

```
sudo apt update -y && sudo apt upgrade -y sudo apt-get install -y nodejs

```




#nano dosyasının içine giriyoruz ve 08 nolu kodu giriyoruz 



```
sudo nano /etc/apt/sources.list.d/nodesource.list

```


Not:# işareti ile deb arasında boşluk olmalı

08 nolu kod

```
# deb [signed-by=/etc/apt/keyrings/nodesource.gpg] https://deb.nodesource.com/node_ jammy main  
```
polymer kurulum
```
git clone https://github.com/sarox0987/polymerlab-ibc-app-solidity.git cd polymerlab-ibc-app-solidity

```


just  ve forge kurulum

```
curl --proto '=https' --tlsv1.2 -sSf https://just.systems/install.sh | bash -s -- --to /usr/local/bin
curl -L https://foundry.paradigm.xyz | bash
source /root/.bashrc
foundryup
forge build

```

# CÜZDAN VE APİ KEY İŞLEMLERİ

Poylmer için bir testnet metamask account oluşturun.

metamask açın ve acoount sekmesini tıklayın

![image](https://github.com/Volkan081/POLYMER-IBC-NODE/assets/95221293/71245eba-7d8e-4de9-8a86-f0b1ab3d71b7)


add acaoount sekmesini tıklayın


![image](https://github.com/Volkan081/POLYMER-IBC-NODE/assets/95221293/a42f5196-7d96-468a-bc28-952108e82911)



daha sonra add new accaount sekmesini tıklayın

![image](https://github.com/Volkan081/POLYMER-IBC-NODE/assets/95221293/c60b015a-3137-4fde-ab2e-5b1abc9491ea)



hesap adı verin ve oluştura tıklayın


![image](https://github.com/Volkan081/POLYMER-IBC-NODE/assets/95221293/a05e5a04-132d-40d3-a327-f0c383a89387)


private key daha sonra lazım olucak oluşturuduğumuz yeni hesabın private key sağda üç noktaya tıklayın özel anahtar basılı tutun  ve kopyalayın ve bir boş bir yere kayıt edin

![image](https://github.com/Volkan081/POLYMER-IBC-NODE/assets/95221293/08afa327-7c81-45e4-8ad5-225a9de3c487)






Alchemy hesabı oluşturup apps kısmından ''create apps'' tıklayıp  Optimism Sepolia ve Base Sepolia App oluşturun



![image](https://github.com/Volkan081/POLYMER-IBC-NODE/assets/95221293/db678305-3f73-4390-9a79-702505a733e7)


optimisim faucet alın 

https://www.alchemy.com/faucets/optimism-sepolia


base faucet alın 

https://www.alchemy.com/faucets/base-sepolia

buradaki işlemlerimiz tamamlandı

nano dosyasını düzenleyelim PRİVATE KEY GİRMEYİ UNUTMAYIN 

```
nano .env

```




PRIVATE_KEY_1 = Metamask private keyi

OP_ALCHEMY_API_KEY = Optimism API Key'i (RPC değil)

BASE_ALCHEMY_API_KEY = Base apı Key'i (RPC değil)

Tırnakların içersine olacak, CTRL X Y enter ile kaydedip çıkıyoruz

Aşağıdaki gibi olmalı 


![image](https://github.com/Volkan081/POLYMER-IBC-NODE/assets/95221293/165ab414-7b6b-467b-996c-ef5030c47329)




# channel oluşturalım

```
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.1/install.sh | bash source ~/.bashrc nvm install 18 nvm use 18 npm install just install just do-it

```

Aşağadaki gibi çıktı almalısınız ve en sonunda 'done it' dediğinde ekran görüntünü #proof kanalına discordda atın ve devs rolünüzü alın 

![image](https://github.com/Volkan081/POLYMER-IBC-NODE/assets/95221293/d76b10c9-2bc2-44cc-9086-9ee374dbecdd)



Hata alındığında ise aşağıdaki kodları girin




```
npx hardhat clean
```


```

just do-it

```
