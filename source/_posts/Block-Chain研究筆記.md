---
title: Block-Chain 研究筆記
date: 2017-11-01 00:00:00
tags: 
- Block-Chain
- SITCON
categories: Block-Chain
thumbnail: https://i.imgur.com/69fpV24.jpg

---

# Blockchain ＆ 智能合約
>  for SITCON 2018
> [name=牟展祐] [Jun , 2018 11：30 PM] 
###### tags : `SITCON`

 # [議程 Github](https://github.com/William-Mou/Blockchain)
 # [詳細說明文件](https://drive.google.com/file/d/1Emrsj72jDzPzsskhkmPcqFgTRzPcRgCs/view?usp=sharing)
 
 ## 關於Talk內容：
 ---
 ## 一、從銀行、中心化到比特幣、去中心化
    * 簡短故事開頭，深入淺出比特幣 

> 區塊鏈（BlockChain）原本只是比特幣網路的一種記帳技術，近幾年來卻在金融、知識產權、數據交易、墊子證照、慈善機構、新能源等領域引起了廣泛的關注。其不外乎有兩大特色：
   * １.區塊鏈具有去中心化的特徵，不以參與交易任何一方為中心，這帶來了效率的提升與成本的降低，直接增加了企業的利潤。
   * ２.區塊鏈具有去信任的特徵，也就是假定交易中的任何一方都是不可信任的。透過記錄不可抵賴的交易的信息，來使交易各方遵守誠信。
> 區塊鏈（BlockChain）是透過「去中心化」和「去信任化」的方式來共同維護資料庫的技術，其將資料庫分別放在不同的節點裡保存，並互相監控數據，資料更動須其餘節點的共識同意。它讓交易過程中每個節點的每一筆交易，都能透明、安全地被紀錄下來。

>而各交易被廣播到全網後一段時間，會被收進一個區塊（Block），和全部的節點複製共享；隨著時間區塊一個一個生成形成一條鏈（Chain）。而所有節點都會擁有所有交易紀錄，共同驗證鏈上資料的正確性，故極難利用少數節點竄改歷史數據。
 ----
 
 ## 二、blockchain概論與架構講解
    python3介紹與代碼說明
    (不細談橢圓形加密與一些特殊算法)
    (視情況省略基礎內容)
 ### ==Github：https://github.com/William-Mou/Blockchain/blob/master/others_python/server.py

 #### Block chain with Python3：
 ![](https://i.imgur.com/DIj0zWE.png)
   
圖1.1藉由/mine挖礦：http://localhost:5000/mine
![](https://i.imgur.com/75Td4DC.png)

  
圖1.2 藉由/transactions/new新增交易：http://127.0.0.1:5000/transactions/new
![](https://i.imgur.com/lZ4dyKG.png)

圖1.3藉由/nodes/register新增交易：http://0.0.0.0:5000/nodes/register
![](https://i.imgur.com/XGNlCXA.png)

圖1.4 藉由/nodes/resolve新增交易：http://127.0.0.1:5000/nodes/resolve
![](https://i.imgur.com/1msmOlE.png)

 ----
 
 ## 三、從區塊鏈到以太坊
     從代幣到智能合約
 #### 啟動 以太坊console with Geth：
 ![](https://i.imgur.com/m6GwSIO.png)
 
 ----
 
 ## 四、架構一簡單以太坊智能合約
     solinium介紹與代碼說明
     (建立在blockchain的觀念上，介紹環境和應用為主)
 
2.1起初帳戶總覽
 ![](https://i.imgur.com/tcDCMoC.png)

2.2建設智能合約
 ![](https://i.imgur.com/J5UX6Cq.png)

2.3建設合約認證
 ![](https://i.imgur.com/qaCLHmD.png)

2.4合約寫入區塊鏈
 ![](https://i.imgur.com/gcPZtO8.png)

2.5 Add方法新增押金	
 ![](https://i.imgur.com/R1iJi4h.png)
 
2.6 合約驗證
 ![](https://i.imgur.com/GLgUjgM.png)

5.2.7 合約寫入區塊鏈
 ![](https://i.imgur.com/i512mNa.png)

2.8勞方使用Collect方法，拿到工資
 ![](https://i.imgur.com/pjSQ2iq.png)

2.9合約寫入區塊鏈
 ![](https://i.imgur.com/gcBRRDJ.png)

2.10勞方獲得工資（ACCOUNT3）
 ![](https://i.imgur.com/FI5do7x.png)


 ### ==solidity範例 Github：https://github.com/William-Mou/Blockchain/tree/master/Hello==
  #### Ethereum Remix 代碼運行截圖
 ![](https://i.imgur.com/yaRMI8D.png)
 ### ==[眾酬範例](https://github.com/William-Mou/Blockchain/blob/master/Hello/contracts/HelloWorld.sol)==
 ### ==[勞基法範例](https://github.com/William-Mou/Blockchain/blob/master/Hello/contracts/Transaction.1.sol)==
 
 ----
 
 ### ==架構智能合約於區塊鏈上 Github：https://github.com/William-Mou/Blockchain/tree/master/Mist==
 
 #### Mist錢包與合約實作
 ![](https://i.imgur.com/Ta10QgS.png)
 ![](https://i.imgur.com/J3VcZ0b.png)
 ### [Mist錢包架設](https://github.com/William-Mou/Blockchain/tree/master/Mist)

 > 之後陸續完成細部截圖說明與剪報...
 > 暫時先放結果0.0

 ## ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~    
    
 ## Some Webs
 ## 參考資源
 :smile:[57屆科展：使用區塊鏈開發可監督捐款之公開募捐平台](http://activity.ntsec.gov.tw/activity/race-1/57/pdf/052505.pdf)
 
 ### 乙太访運作與實作
[以太坊白皮书](https://github.com/ethereum/wiki/wiki/%5B%E4%B8%AD%E6%96%87%5D-%E4%BB%A5%E5%A4%AA%E5%9D%8A%E7%99%BD%E7%9A%AE%E4%B9%A6)
 :smile:[智能合約](https://blog.gasolin.idv.tw/2017/08/13/got-my-ens-domain/)
 [以太坊錢包Parity](https://medium.com/taipei-ethereum-meetup/%E5%9C%A8parity%E5%89%B5%E5%BB%BA%E4%BB%A5%E5%A4%AA%E5%9D%8A%E9%8C%A2%E5%8C%85-b2c2977378fc)
 [教練，我”只”想學Solidity](https://medium.com/taipei-ethereum-meetup/%E6%95%99%E7%B7%B4-%E6%88%91-%E5%8F%AA-%E6%83%B3%E5%AD%B8solidity-92b7ba8054f5)
 
 :smile:[收到我的ENS網域啦 gasolin.eth](https://blog.gasolin.idv.tw/2017/08/13/got-my-ens-domain/)
 :smile:[如何撰寫智能合約(Smart Contract)?(I)](https://blog.gasolin.idv.tw/2017/09/06/howto-write-a-smart-contract/)
 :smile:[如何撰寫智能合約(Smart Contract)?(II)建立加密代幣 ](https://blog.gasolin.idv.tw/2017/09/11/howto-write-a-simple-token/)
 :smile:[如何撰寫智能合約(Smart Contract)?(III)建立標準代幣 ](https://blog.gasolin.idv.tw/2017/09/16/howto-write-an-erc20-compatible-token/)
 [如何撰寫智能合約(Smart Contract)?(IV)加入單元測試](https://blog.gasolin.idv.tw/2018/01/02/howto-write-a-contract-test/)
 
 
 [区块链开发（一）搭建基于以太坊的私有链环境](http://blog.csdn.net/sportshark/article/details/51855007)
 [区块链开发（二）部署和运行第一个以太坊智能合约](http://blog.csdn.net/sportshark/article/details/52249607)
 [区块链开发（三）编写调试第一个以太坊智能合约](http://blog.csdn.net/fidelhl/article/details/52524434)
 [Solisity文檔](http://solidity.readthedocs.io/en/latest/)
 [Solidity中文語法表](http://www.tryblockchain.org/Solidity%E6%99%BA%E8%83%BD%E5%90%88%E7%BA%A6%E6%96%87%E4%BB%B6%E7%BB%93%E6%9E%84.html)
 [Solidity語法教學](http://blog.csdn.net/diandianxiyu_geek/article/details/77877841)
 
 [如何在私有区块链上编写、部署以及与以太坊进行交互的智能合约](http://blog.csdn.net/dev_csdn/article/details/78893014)
 
 
 [台北乙太坊社群專欄](https://medium.com/taipei-ethereum-meetup)
 [Solidity撰寫智能合約與注意事項(一)](https://medium.com/taipei-ethereum-meetup/solidity%E6%92%B0%E5%AF%AB%E6%99%BA%E8%83%BD%E5%90%88%E7%B4%84%E8%88%87%E6%B3%A8%E6%84%8F%E4%BA%8B%E9%A0%85-%E4%B8%80-6c9eacc00168)
 [Solidity撰寫智能合約與注意事項(二)](https://medium.com/taipei-ethereum-meetup/solidity%E6%92%B0%E5%AF%AB%E6%99%BA%E8%83%BD%E5%90%88%E7%B4%84%E8%88%87%E6%B3%A8%E6%84%8F%E4%BA%8B%E9%A0%85-%E4%BA%8C-dd915bdeafa0)
 [合約與以太接收](https://ethereum.stackexchange.com/questions/27052/how-to-create-a-smart-contract-to-send-an-eth-tx-on-time)
 
 
 ### Python語法
 :smile:[python2 廖雪峰教程](https://www.liaoxuefeng.com/wiki/001374738125095c955c1e6d8bb493182103fac9270762a000)
 :smile:[python3 廖雪峰教程](https://www.liaoxuefeng.com/wiki/0014316089557264a6b348958f449949df42a6d3a2e542c000)
 :smile:["@"裝飾器概念](https://foofish.net/python-decorator.html)
 :smile:[Python & Flask](http://blog.techbridge.cc/2017/06/03/python-web-flask101-tutorial-introduction-and-environment-setup/)
 
 ### 觀念建構
:smile:[區塊鏈技術概觀（一）：讓我們從歷史文本說起](https://finance.technews.tw/2017/08/01/block-chain-technology-overview/)
:smile:[區塊鏈技術概觀（二）：資料分割與密碼學](https://technews.tw/2017/08/09/blockchain-principle-part-two/)
:smile:[區塊鏈技術概觀（三）：多數決的運作結構](https://technews.tw/2017/08/16/blockchain-principle-part-three/)
[區塊鏈技術指南](https://yeasy.gitbooks.io/blockchain_guide/content/)


 ### python實作
 [用Python从零开始创建区块链](http://www.jianshu.com/p/cc6663cbbc41)
 [50 行 Python 代码构建一个区块链](http://blog.csdn.net/simple_the_best/article/details/75448617)

 ### 其他實作
 [瀏覽器挖礦分析](https://4hou.win/wordpress/?p=9162)
 [javascript](http://robertvmp.pixnet.net/blog/post/24544521-javascript---入門觀念基礎教學)
 [Socket](http://beej-zhtw.netdpi.net/02-what-is-socket/2-1-two-internet-sockets)
 :smile:[Flask](http://dormousehole.readthedocs.io/en/latest/quickstart.html)
 
## 一些個人想法
一日半夜所思：
中心思想：有鑒於「信任」成為了網路世界中的最後一道難題，區塊鏈這把鑰匙將成為下個10年的關鍵技術！而學習區塊鏈這多技術合成的概念，必能使個人與網路環境更趨於完善！

幾個方向：
1.交易公平去中心：採比特幣技術，可以達到交易不受到任何一方掌控，我認為這對於未來得金融支付系統可以產生重大動搖！
2.合約透明散中心：透過交易資料，使合約成為一種交易狀態，有望用於一但交易完成不可更改而大筆的交易，如土地、不動產交易，權力的轉移（著作權、親權等），以至於人口紀錄，戶籍遷移等等。
3.資訊永存分中心：若所有人民無法共同達到最高公民素養，那政府機制（中心機制）必仍然存在；如同若無法每個人都擁有相同電腦，那挖礦速度必存在差異。如此一來，縱使再怎麼強調烏托邦世界，一定程度的中心存在是不可避免的，那麼，能夠讓中心權利分治，變成為一關注重點。現今透過媒體等等來監督政府體制，但無法達到高效率同步，亦不能維持訊息完整度，經過一層轉手，資訊比有失真。故，透過區塊鏈不可更改，可快速傳播的特性，有望能夠達成全民監督政府資訊（透過軟件檢視政府是否串改資料），使過往諾言不可食言。

願景：
本科展願能對三方面做出淺分析與實作，又以2.3.為主要目標，希望能拋磚引玉，促進台灣區塊鏈新技術的發展。

  
## 代碼
```python=
import hashlib
import json
from textwrap import dedent
from time import time
from uuid import uuid4
from flask import Flask, jsonify, request
from urllib.parse import urlparse
import requests


class Blockchain(object):
    def __init__(self):
        self.chain = []
        self.current_transactions = []
        self.nodes = set()
        # Create the genesis block
        self.new_block(previous_hash=1, proof=100)
        
    def register_node(self, address):
        """
        Add a new node to the list of nodes
        :param address: <str> Address of node. Eg. 'http://192.168.0.5:5000'
        :return: None
        """

        parsed_url = urlparse(address)
        self.nodes.add(parsed_url.netloc)

    def new_block(self, proof, previous_hash=None):
        # Creates a new Block and adds it to the chain
        """
        生成新块
        :param proof: <int> The proof given by the Proof of Work algorithm
        :param previous_hash: (Optional) <str> Hash of previous Block
        :return: <dict> New Block
        """

        block = {
            'index': len(self.chain) + 1,
            'timestamp': time(),
            'transactions': self.current_transactions,
            'proof': proof,
            'previous_hash': previous_hash or self.hash(self.chain[-1]),
        }

        # Reset the current list of transactions
        self.current_transactions = []

        self.chain.append(block)
        return block
    
    def new_transaction(self, sender, recipient, amount):
        """
        生成新交易信息，信息将加入到下一个待挖的区块中
        :param sender: <str> Address of the Sender
        :param recipient: <str> Address of the Recipient
        :param amount: <int> Amount
        :return: <int> The index of the Block that will hold this transaction
        """

        self.current_transactions.append({
            'sender': sender,
            'recipient': recipient,
            'amount': amount,
        })

        return self.last_block['index'] + 1
    
    @staticmethod
    #從外部非實體化調用函數
    def hash(block):
        """
        生成块的 SHA-256 hash值
        :param block: <dict> Block
        :return: <str>
        """

        # We must make sure that the Dictionary is Ordered, or we'll have inconsistent hashes
        block_string = json.dumps(block, sort_keys=True).encode()
        return hashlib.sha256(block_string).hexdigest()

    @property
    #檢查參數後再傳入
    def last_block(self):
        return self.chain[-1]
    
    @staticmethod
    def valid_proof(last_proof, proof):
        """
        验证证明: 是否hash(last_proof, proof)以4个0开头?
        :param last_proof: <int> Previous Proof
        :param proof: <int> Current Proof
        :return: <bool> True if correct, False if not.
        """

        guess = f'{last_proof}{proof}'.encode()
        guess_hash = hashlib.sha256(guess).hexdigest()
        return guess_hash[:4] == "0000"
    
    def proof_of_work(self, last_proof):
        """
        简单的工作量证明:
         - 查找一个 p' 使得 hash(pp') 以4个0开头
         - p 是上一个块的证明,  p' 是当前的证明
        :param last_proof: <int>
        :return: <int>
        """
        proof = 0
        while self.valid_proof(last_proof, proof) is False:
            proof += 1

        return proof
    def valid_chain(self, chain):
        """
        Determine if a given blockchain is valid
        :param chain: <list> A blockchain
        :return: <bool> True if valid, False if not
        """

        last_block = chain[0]
        current_index = 1

        while current_index < len(chain):
            block = chain[current_index]
            print(f'{last_block}')
            print(f'{block}')
            print("\n-----------\n")
            # Check that the hash of the block is correct
            if block['previous_hash'] != self.hash(last_block):
                return False

            # Check that the Proof of Work is correct
            if not self.valid_proof(last_block['proof'], block['proof']):
                return False

            last_block = block
            current_index += 1

        return True

    def resolve_conflicts(self):
        """
        共识算法解决冲突
        使用网络中最长的链.
        :return: <bool> True 如果链被取代, 否则为False
        """

        neighbours = self.nodes
        new_chain = None

        # We're only looking for chains longer than ours
        max_length = len(self.chain)

        # Grab and verify the chains from all the nodes in our network
        for node in neighbours:
            response = requests.get(f'http://{node}/chain')

            if response.status_code == 200:
                length = response.json()['length']
                chain = response.json()['chain']

                # Check if the length is longer and the chain is valid
                if length > max_length and self.valid_chain(chain):
                    max_length = length
                    new_chain = chain

        # Replace our chain if we discovered a new, valid chain longer than ours
        if new_chain:
            self.chain = new_chain
            return True

        return False

# Instantiate our Node
app = Flask(__name__)

# Generate a globally unique address for this node
node_identifier = str(uuid4()).replace('-', '')

# Instantiate the Blockchain
blockchain = Blockchain()


@app.route('/mine', methods=['GET'])
def mine():
    # We run the proof of work algorithm to get the next proof...
    last_block = blockchain.last_block
    last_proof = last_block['proof']
    proof = blockchain.proof_of_work(last_proof)

    # 给工作量证明的节点提供奖励.
    # 发送者为 "0" 表明是新挖出的币
    blockchain.new_transaction(
        sender="0",
        recipient=node_identifier,
        amount=1,
    )

    # Forge the new Block by adding it to the chain
    block = blockchain.new_block(proof)

    response = {
        'message': "New Block Forged",
        'index': block['index'],
        'transactions': block['transactions'],
        'proof': block['proof'],
        'previous_hash': block['previous_hash'],
    }
    return jsonify(response), 200
  
@app.route('/transactions/new', methods=['POST'])
def new_transaction():
    values = request.get_json()

    # Check that the required fields are in the POST'ed data
    required = ['sender', 'recipient', 'amount']
    if not all(k in values for k in required):
        return 'Missing values', 400

    # Create a new Transaction
    index = blockchain.new_transaction(values['sender'], values['recipient'], values['amount'])

    response = {'message': f'Transaction will be added to Block {index}'}
    return jsonify(response), 201


@app.route('/chain', methods=['GET'])
def full_chain():
    response = {
        'chain': blockchain.chain,
        'length': len(blockchain.chain),
    }
    return jsonify(response), 200

@app.route('/nodes/register', methods=['POST'])
def register_nodes():
    values = request.get_json()
    print(values)
    nodes = values.get('nodes')
    if nodes is None:
        return "Error: Please supply a valid list of nodes", 400

    for node in nodes:
        blockchain.register_node(node)

    response = {
        'message': 'New nodes have been added',
        'total_nodes': list(blockchain.nodes),
    }
    return jsonify(response), 201


@app.route('/nodes/resolve', methods=['GET'])
def consensus():
    replaced = blockchain.resolve_conflicts()

    if replaced:
        response = {
            'message': 'Our chain was replaced',
            'new_chain': blockchain.chain
        }
    else:
        response = {
            'message': 'Our chain is authoritative',
            'chain': blockchain.chain
        }

    return jsonify(response), 200

if __name__ == '__main__':
    app.run(host='0.0.0.0', port=5000)

```