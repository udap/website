# Universal Decentralized Asset Protocol(UDAP)

A White Paper

Version 0.6

**UDAP Foundation， 1/13/2007**

## 1.  background

In the beginning, there was Bitcoin.  

Although touted by its inventor as "digital cash", Bitcoin has been pushed to play pivotal roles beyond crypto-currency.  Many projects have created protocols on top of Bitcoin to facilitate the exchange of general assets. [Mastercoin][Counterparty][Prism]

But because Bitcoin has been first and foremost designed to work as a fungible currency, using it beyond as such has proved to be clunky and limited.

Ethereum (the E, for short reference) has emerged from the crowed to carry its inventor’s destiny as a general and abstract protocol of general blockchain based world computer. A general-purposed smart contract architecture lends its well to building a variety of on-chain applications to fulfill blockchain’s promise of being the backbone of the "Internet of Values".

But the most challenging thing posed to E is how to represent the "values". For the moment, like almost all the other open ledger platforms, E  is exclusively handling digital currency transfers, as Buterin put in one of his podcasting in early 2018:

"The very first vision was basically a general purpose platform for financial contracts. If X happens then send $5 to account Y, if Z happens send $5 to account B. That was basically what I thought Ethereum would be for" [http://unchainedpodcast.co/vitalik-buterin-creator-of-ethereum-on-the-big-guy-vs-the-little-guy]

E’s model of "value" is primitive. In the basic model, for any kind of value/asset the only attribute associated with this asset is the balance of it, a number. This simplified model probably will fit financial transactions well, but it's very lacking dealing with variety of asset types in the operation of the world economy.

The three-year-old smart contract implementation in Ethereum, although has attracted thousands of development teams to deploy applications, mostly in Solidity, on the platform, is far from being mature and productive towards becoming the world computer:
- Limited in features and functions. For instances:
    - Limited parameter types.
    - Lack advanced language features that JavaScript, Python, Java can offer.
    - Primitive collection processing and manipulations.
- Slow performance. The EVM is not really a modern virtual machine like JVM or V8 JavaScript engine. It’s an interpreter that parse the smart contract opcode and run the underlying supporting libraries.  The EVM is at least an order slower than regular system programming languages. The total throughput of the blockchain is directly impacted by the slow performance of the virtual machine. There are many reasons that faster and mature virtual machines cannot be used in the current version of Ethereum.  And there are quite a few efforts in development to enhance the performance of the virtual machine.
- The general purpose computing power in the  current version of EVM, on the other hand, has rendered itself vulnerable to many security breaches, as documented by [Making Smart Contract Smarter, https://www.comp.nus.edu.sg/~loiluu/papers/oyente.pdf, Loi Luu, et. al., 2016]. It's very hard for relatively inexperienced programmers to get the Smart contract right. Considering many of the smart contract are handling many millions of dollars of assets, customers take a huge risk in moving forward with a smart contract strategy.

If we can draw some analogies between web application development and blockchain application development, smart contract is to blockchain development what CGI is to web app development. It’s rather young.

The limitations of the current mainstream Smart contract platforms have become a serious impediment to peoples ever-growing interest in tokenization of everything.
Tokenization has become the symbol of The new economy, short named as token economy. In this new economy enabled by block team technologies, every bit of value is represented by a crypto-graphical token. With the security feature enabled by blockchain technologies, tokens have basically transformed the asset we deal with every day into capital, characterized by its high liquidity. Tokens make the people who own assets to realize the economic returns that those assets are capable of, in the meantime, tokens will make those people who are in need of capital to get the capital in a most feasible way. Tokens are basically the gasoline of the new economy. If there is one thing that will happen in the next few year for the Internet industry, this "one thing" is to "tokenize everything".


- Crypto tokens represent (or be pegged to) shares of right, access to services, voting power, real world financial assets, etc.  
- Tokens serve as accounting units in bookkeeping and payments.
- Tokens eliminate the requirement of intermediaries in many trading scenarios thus simplify and expedite the trading process at very low cost. Fungible tokens are very easy to trade en mass, while none-fungible tokens can help to track the asset flow in an economy thus to help people understand the dynamics of the economy.  
- In short, crypto-tokens are the private money for applications.

Tokens have been used in crowdfunding a new wave of innovative applications based on blockchain and related technologies. This has disrupted the startup model based on VC funding.  On one side startups can receive funding much earlier in their product development. On the other side, everyone can invest in projects they believe in and gain the potential for investment return which used to the privilege of so called "accredited investors".

Tokens are the tickets to the next Internet banquet.

UDAP has been designed to support tokenizing everything movement natively, in the low-level storage model and communications. We are shifting away from the lump sum description of values into individually identifying each every and every items in the physical world in virtual world alike. On top of the identifications, we are going to beauty brand-new user experience to deal with their personal properties intuitively, to sell them, to trade them, to pledge them for capital, to lead them to friends, or to give them away. In the back, UDAP is any neighborly protocol for any third parties to port their existing applications easily and quickly to open ledger technologies and a decentralized storage Technologies. Therefore from the back end to the user experience end, UDAP is created to become the native enabling technology to fulfill the promise of the Internet of values.

Blockchain technology is nicknamed the Internet of the moment
However, when we look closely at the carrier of value transfer currently carried by the blockchain, 99% of the applications are actually limited to the best liquidity and the most easily solved type of asset, which is cryptocurrency.
So the current blockchain is more accurately "The Internet of Money" \ [* The Internet of
Money *, A.M. Antonopoulos \].
But our neighborhood faces massive, palpable and non-palpable assets. Are these good blockchain, or related decentralized, bookkeeping techniques, good value, discovery, value recognition, and value transfer? There is no doubt that the answer is yes. There have been quite a few blockchain-based technologies that are attempting to address real-world non-monetary assets and how to decentralize their networks in recognition of the exchange of recognition. However, we find these protocol offerings and platforms based on the existing blockchain, the second-level structure based on currency transfers. Around 2014, when Bitcoin technology was recognized by the majority, many projects proposed the notion of a colored currency, one that is grafted onto the currency of permutable value - Unique identification technology that allows us to use currency symbols to represent real-life accessible and non-accessible assets.

早期的"颜色货币"靠在比特币网络传输的协议中增加交易的顺序来进行特殊含义的赋予。这种方法，当然是对比特币协议的特殊扩展应用。当然因为比特币独特的简化协议，使得任何第三方的应用想对自己的资产进行数字化和加密，货币化都需要比较大的工作和一定的技术门槛。以太坊作为另外一个主流的加密货币，一开始的初衷，就是希望能够把区块链的网络变成一个高度可编程的，可应用于对现实世界的价值节点进行确认，传输转移和交换的平台，它的目的是建立一个通用的，去中心化的计算平台，逐渐的，他也加入了更多去中心化的存储功能在内，虽然这两种功能尚未在成熟的版本中发布。

The early "color money" was given special meaning by increasing the order of transactions in the protocol transmitted by the Bitcoin network. This approach, of course, is a special extension of the Bitcoin protocol. Of course, because Bitcoin's unique simplified protocol makes any third-party application want to digitize and encrypt its own assets, monetization requires relatively large work and certain technical thresholds. Ethereum, as another mainstream cryptocurrency, initially aimed to turn the blockchain network into a highly programmable platform that can be used to identify, transfer, and exchange value for the real world , Whose purpose is to create a common, decentralized computing platform that, gradually, he has also added more decentralized storage capabilities, though both features have not yet been released in the mature release.

以太坊所体现的我们称之为颜色货币的概念，是通过智能合同来进行的，在常见的智能合同的应用场景中，外部世界的资产被智能合同中的电子对类型的数据库来进行存储，通过用户自定义的一些基本逻辑和安全机制来管理这些资产的登记，发售和流转。

Ethereum reflects what we call the concept of color money through smart contracts. In common applications of smart contracts, the assets in the outside world are stored electronically in a type of database by an intelligent contract, The registration, offering and circulation of these assets are governed by some basic logic and security mechanisms that are user-defined.

智能合同编写远非易事。我们看到，以太坊这两年在逐渐成熟的过程中，已经有自身非常大的性能问题和安全隐私问题，其主要的工作方向并不在于提供一套便捷的可供任何现实世界应用、利用的资产管理和应用平台，而是把注意力集中在更底层的性能吞吐量和安全隐私等更为基础的环节，当然这是非常好的，因为如果没有这些最基础的应用指标，那么在之上建筑的任何具有真正意义上的杀手级的应用，都会导致整个系统的性能迟缓和用户体验的急剧下降。最近在一台仿世界的加密小毛，一款简单的资产应用，就导致了一段时间内以太坊网络中25\~30%的流量都是被这一款应用所占据，以至于以太资产的转移和确认时间急剧增长。

Smart contract preparation is far from easy. We see that Ethereum has gradually had its own great performance problems and security privacy problems during its gradual maturity in the past two years. The main goal of Ethereum is not to provide a convenient and practical application for any real-world application Asset management and application platform, but instead focuses on the more basic aspects of bottom-level performance throughput and security privacy, which of course is very good because without these most basic application metrics, Any real killer application on the building can result in slow performance and dramatic user experience degradation across the entire system. Recently, in an imitation of the world's small encrypted hair, a simple asset application, resulting in a period of time Ethereum network 25 ~ ~ 30% of the traffic is occupied by this one application, so that the transfer of Ethernet assets And confirm the rapid growth of time.

智能合同的编程语言的成熟性远不如传统应用使用的编程语言的功能强大，
同时在健壮性方面还处于童年时期。 对大多数没有经验的程序员而言，
编写智能合同是一个"nightmare"。

The maturity of the programming language of smart contracts is far less powerful than the programming languages used by traditional applications,
At the same time in terms of robustness is still in childhood. For most inexperienced programmers,
Writing a smart contract is a "nightmare."

## 2.  目标

goal

我们的终极目标是建设一个"资产互联网"（The Internet of Asset）。
其价值定位有一个明确且清楚的边界，我们有三个目标：

Our ultimate goal is to build The Internet of Asset.
Its value proposition has a clear and clear boundary, and we have three goals:
1.  制定一个从区块链的角度理解和认识我们世界中的"资产"的概念，
    并且抽象出通常对于资产的各种处置行为， 并为之制定一个协议，
    为传统的各垂直行业的软件开发商提供一个便捷的API。这样的API不要求用户对区块链技术和去中心化的技术有较为深刻的认识和较为熟练的编程经验。

     Develop a concept of understanding and understanding "assets" in our world from a blockchain perspective,And abstraction of the various assets for the disposal of the general behavior and to develop an agreement,A convenient API for traditional vertical developers. Such an API does not require users to have a deeper understanding of blockchain technology and decentralized technology and a more experienced programming experience.

2.  提供一个资产互联网协议的参考实现，
    让他们能够在不改变现有应用架构的情况下，搭上去中心化的计算和去中心化存储的快车。
    我们把去中心化的计算，去中心化的存储技术和去中心化的信息机制中最核心的部分，抽象成简洁有效的API供他们使用，这样可以大大弥补目前你快练技术和去中心化的一整套技术对第三方垂直应用开发者的巨大的技术障碍和挑战。并且，考虑到去中心化的计算和存储技术目前还处于不成熟的阶段，还处于快速发展的时期，我们认为这样的技术平台会给第三方应用开发者带来巨大的价值。

    Provide a reference implementation of asset internet protocol,So that they can catch the decentralized computing and decentralized storage of express trains without changing the existing application architecture.We abstract the most central part of decentralized computing, decentralized storage technology and decentralized information mechanism into a concise and effective API for their use, which can greatly make up for your current skills and decentralization A set of technologies for third-party vertical application developers huge technical obstacles and challenges. And considering that the decentralized computing and storage technologies are still in an immature phase and are in a period of rapid growth, we believe such technology platforms will bring tremendous value to third-party application developers.

3.  我们平台将提供一个面向终端用户的通用资产钱包的实现，在这个通用资产钱包中，我们把一般性资产管理所面临的主要的问题都做出足够理性的抽象，并且把各种对资产的处置方式和手段都集中在那，对个人用户而言，操作简明易懂。这个通用资产钱包对个人用户提供了极大的便利来管理自己在使用各种应用中所积累的有形和无形资产。这样的设计对第三方应用开发平台而言，其实是一个非常有利的消息，原因是第三方平台可以专注于目前核心的用户体验，而无需考虑如何让自己的资产以区块链的方式和用户交互。

    Our platform will provide an implementation of a general-purpose wallet for end-users in which we capitalize on the rationale for the major issues that general asset management faces and rationalize various asset disposal Ways and means are focused on that, for individual users, the operation is easy to understand. This universal asset wallet offers great convenience to individual users to manage the tangible and intangible assets that they have accumulated in the use of various applications. Such a design for third-party application development platform, in fact, is a very favorable news, because the third-party platform can focus on the current core user experience, without having to consider how to make their own assets blockchain and user Interaction.

![](media/image1.png)




## 3.  设计理念

design concept

资产互联网协议的基本理念是建设一个"厚协议层"，支撑"薄应用层" （Thick Protocol + Thin Application）。

The basic idea of an asset internet protocol is to build a "thick protocol layer," supporting "Thick Protocol + Thin Application."

应用层主要关心的问题是和自己所在的特殊人群的交互行为，而这种行为的有些通用的资产处置部分，实际上也是可以由通用资产钱包来帮助解决的，所以，我们给第三方应用开发者提供的一个愿景就是，第三方应用开发者只需要对自己所垂直的行业有足够的知识和认识，那么基于我们的厚协议层就可以迅速开发出自己客户所需要的功能，并且以最短的时间投入市场，产生自己想追求的商业效益。

The main concern at the application level is the interaction with the particular population in which they are located, and some of the common asset disposal aspects of such behavior can in fact be helped by the universal wallet, so we give third-party application development One of the visionaries is that third-party application developers need only have enough knowledge and understanding of their vertical industry, then based on our thick protocol layer can quickly develop the features required by their customers, and the shortest Time into the market, have their own want to pursue business benefits.

用Ethereum区块链来作为参照的设计是我们的起点。 我们的设计思维和Ethereum 最大的差别是关于"Feature"。 Vitalik Buterin 认为Ethereum 的设计思想之一是Ethereum 是一个 "Feature-less" 的计算平台。

Designing as a reference using the Ethereum blockchain is our starting point. The biggest difference between our design thinking and Ethereum is about "Feature." Vitalik Buterin believes that one of Ethereum's design ideas is that Ethereum is a "Feature-less" computing platform.

**We Have No Features**: as a corollary to generalization, we often
refuse to build in even very common high-level use cases as intrinsic
parts of the protocol, with the understanding that if people really want
to do it they can always create a sub-protocol (e.g., ether-backed
subcurrency, bitcoin/litecoin/dogecoin sidechain, etc) inside of a
contract.  \[ <https://github.com/ethereum/wiki/wiki/Design-Rationale>\]


Ethereum 显然主要目标是建设成一个通用的区块链平台。 任何有针对性的高层次的功能性抽象都被推给了用户自定义的智能合约中。这种理性的有节制的目标是令人赞同的， 但是却不是我们构思的"Asset Internet"协议以及参考实现追求的方向。 智能合同因为其"Turning Complete" 的计算能力为DAPP开发者提供了相对而言的极大的灵活性, 但是也表现出明显的技术障碍和现实风险。智能合同虽然"Turning Complete"，但是提供的编程能力还是有很大的局限性，对于普通应用开发者而言有很多"坑"需要绕过。 同时因为一切代码被暴露的原因，用户自定义的智能合约暴露了很大的受攻击表面， 就像Ethereum 近两年所发生的几起造成严重的经济损失的事故所展现的一样。比特币网络拥有非常有限的智能合同能力。但是说到底，这并不是比特网络的一个明显的局限性，实际上很多比特币网络的忠实粉丝认为这种有限的设计是一种非常好的措施来防止比特币网络受到各种各样的攻击。比特币网络引以为傲的一个非常重要的指标就是，一段时间来比特币网络经受了无数的冲击，但是，比特币网络从本质上来说，还没有出现一次真正的巨大的漏洞。

Ethereum clearly has the main goal of building a common blockchain platform. Any targeted high-level functional abstraction is pushed to user-defined smart contracts. This rational and restrained goal is agreeable, but it is not the "Asset Internet" protocol we conceived and the direction we sought to pursue. Smart contracts offer DAPP developers relatively great flexibility because of their "Turning Complete" computing power, but also show obvious technical obstacles and real risks. Although Smart Contract "Turning Complete", but provide programming ability is still very limited, for ordinary application developers have a lot of "pit" need to bypass. At the same time, because of all the code being exposed, user-defined smart contracts have exposed a large attack surface, as evidenced by several incidents that have caused serious economic losses in the past two years in Ethereum. Bitcoin networks have very limited smart contract capabilities. Ultimately, however, this is not a clear limitation of a bit-based network. In fact, many loyal fans of bitcoin networks see this limited design as a very good way to prevent bitcoin networks from being subjected to a variety of attacks . A very important indicator of the bitcoin network's pride is that bitcoin networks have endured countless shocks for some time, but essentially no major loophole has emerged in the bitcoin network.

"Asset Internet" 从目标而言不是一个通用计算平台，而是一个专门处置财务角度和更一般的角度处理现实资产和加密资产的平台，是一个"Featured Chain". 从protocol 的角度评价是一个更thick 和更专门化的协议，这个协议natively 支持资产的代币化和通用的资产行为，例如存储，转移， 交易， 销售等等，面向的是一般软件开发者。并且我们希望在这个垂直领域中，我们能为我们第三方的客户提供一个健壮的，高性能的，持续有效，并且不会出错的一个资产管理和交易平台。为了达到这个目的，更为了从安全和性能的角度实现这个目的，我们甚至考虑不支持智能合约（或者至少不把智能合约的能力暴露给终用户）。也就是说我们不惜牺牲掉通用智能合约或者通用计算能力，直接把资产管理的能力的安全性和性能作为平台最主要的发展方向。这个实现级别的考虑也许会在项目进展中仔细推敲。

"Asset Internet" is not a universal computing platform from the goal, but a platform that handles financial assets and encrypted assets from a financial perspective and a more general perspective. It is a "Featured Chain." From a protocol perspective, it is a more thick and more specialized protocol that natively supports the tokenization of assets and common asset behavior such as storage, transfer, trading, sales, etc., for the average software developer. And we hope that in this vertical field we can provide our third-party clients with a robust, high-performing, asset management and trading platform that is both effective and error-free. To do this, we even consider not supporting smart contracts (or at least not exposing the capabilities of smart contracts to end users), even more for safety and performance reasons. In other words, we at the expense of general-purpose smart contracts or general-purpose computing power, the ability to directly asset management capabilities and performance as the most important platform for the development. This level of realization may be carefully considered in the progress of the project.

我们认为这种"Thick Protocol + Thin Application"的模式将是区块链应用的核心架构模式，它将极大地为互联网的新型应用带来极大的繁荣。这种模式从技术说有革新性的意义， 从价值上分析，会让互联网的价值从应用层下沉到协议层，让协议层变成一个跨应用的大数据沉积层。客观的结果是协议层变得更有战略价值和投资价值。

We think this "Thick Protocol + Thin Application" model will be the core architecture model for blockchain applications and will greatly boost the new applications of the Internet. This model is technically innovative and value-conscious, allowing the value of the Internet to sink from the application layer to the protocol layer, turning the protocol layer into a cross-application big data deposition layer. The objective result is that the protocol layer becomes more strategic and investment value.

![](media/image2.png)

## 4. 对应用开发者的价值陈述

App developer value statement

<!-- -->

1.  块链带来的坚不可摧的数据库能力。这种数据库能力，是过去传统的数据库体系里面梦寐以求的，并且可能是需要非常昂贵的设置和管理才能带来的效益。因为这其中牵涉了很复杂的数据库同步、备份、灾难恢复等等关键性的技术。这些能力在过去都是需要高级的数据库管理人员专注才能够得到较为妥善解决的技术能力，维护成本极为高昂。如果考虑到区块链本身能够提供一个全球性的覆盖的话，那么相对于传统的数据库技术，这种优势就更为明显。

    Unbreakable database capabilities brought by blockchain. This kind of database capability is what the traditional database system was dreaming of in the past and could be the result of the need for very expensive setup and management. Because it involves a very complex database synchronization, backup, disaster recovery, and other key technologies. In the past, these abilities required the attention of senior DBAs to get a better technical solution and the maintenance cost was extremely high. This is especially true when compared to traditional database technologies, given that the blockchain itself provides a global reach.

2.  第二类的价值发生在，当区块链的应用不仅仅局限于自己所在的用户范围内的时候。因为区块链技术提供的是一个有保障的，公开的记账体系，天然的适用于一个企业在自己所属的产业链中的上下游的整合。产业链中上下游数据的整合是过去传统应用中持续会面临的技术挑战。在上下游整合的过程中，由于缺乏互相之间的信任，如果没有一个较为复杂的商业协定，或者双方都可信任的第三者商业体（有时候是政府机构）来推动的话，这种整合的周期往往遥遥无期，并且整合中的责任和成本都很高昂，而区块链技术提供了这种不信任的商业环境中无需第三方信任实体的存在，又能提供数据价值整合的能力。

    The second type of value occurs when the application of the blockchain is not limited to the users within its own domain. Because blockchain technology provides a secure, open accounting system that naturally applies to the upstream and downstream integration of an enterprise in the industry chain to which it belongs. The integration of upstream and downstream data in the industry chain is a continuing technical challenge in the traditional applications. Integration in the upstream and downstream process, due to the lack of trust between each other, without a more complex commercial agreement, or both trusted third party business (sometimes government agencies) to promote this integration Are often outdated and have a high burden of integration and cost, and blockchain technology offers the ability to trust data in this distrusted business environment without the existence of third-party trust entities.

3.  为第三方应用提供立即的实现应用内经济代币化的手段。第三方应用可以把应用类的经济流动时所需要的手段使用加密货币的代币模型进行重新规划。应用内的市场营销手段，激励手段，用户付费的新模式，甚至包括利益分配的新模式。用以太坊的标准的手段来建立自己的经济货币的时候，需要较为熟练的智能合同的编程能力或者是雇佣具有这种编程能力的咨询团队来建立自己的应用内加密货币的智能合同提供的能力，我们的协议能够使用户只需要配置一些标准化的参数，就可以发行能够在自己的经济体系中使用的加密数字货币。这样的加密货币将立刻能够在我们提供的通用数字资产钱包中得以展现。不仅如此，通用资产协议本身还提供资产的分布是交易(Decentralized Exchange)的能力，这种能力能够把用户发行的自定义加密数字化资产和目前加密数字资产行业主流的加密货币建立交易对，能够让App内数字资产立刻产生流通性和流动性，极大地激活在应用内的经济体中较为复杂和多变的灵活的金融手段。这种应用内的代币满足ERC20协议，所以也能在绝大多数的兼容ERC20的钱包中存储。

    For third-party applications to provide immediate means of realization of economic tokens within the application. Third-party applications can reprogram the tokens used in cryptocurrencies for the means needed by the economy of the application class. In-app marketing, Incentives, new models for users to pay, and even new modes of distribution of benefits. Using Ethereum's standard means of setting up your own economic currency requires the ability to program smarter, smarter contracts or hire an in-house consulting team with this ability to set up their own in-app smarter contracts for cryptocurrencies , Our agreement enables users to distribute encrypted digital currencies that can be used in their economy simply by configuring a few standardized parameters. This cryptocurrency will immediately show up in the universal digital asset wallet we offer. Not only that, the GVAs themselves provide the ability to distribute assets as a Decentralized Exchange that enables the trading of custom-issued digitized assets issued by users with the cryptocurrencies in the mainstream of the current cryptographic digital asset industry The immediate emergence of liquidity and liquidity in digital assets within App greatly stimulates the more sophisticated and volatile financial instruments in an in-app economy. The token in this application fulfills the ERC20 protocol and can therefore also be stored in the vast majority of ERC20-compatible wallets.

4.  提供交易的缓冲和性能的提升。第三方应用利用区块链使的性能和吞吐量的支撑在现在能够支持智能合同的最常见的平台，也就是以太坊。Ethereum网络现在每天处理能力达到百万级，但是这个能力相对传统集中式的大型应用还是有极大的差距。 性能问题在未来2到3年里面，才有可能逐步地得到解决。[https://blog.ethereum.org/2018/01/02/ethereum-scalability-research-development-subsidy-programs] 对于立刻需要这种高吞吐能力的区块链技术的第三方应用来说，我们的通用的资产互联网将提供这种能力。这是如果用户绕开我们的资产互联网直接使用底层的已开放的智能合同的技术所不能达到的。

    Provide transaction buffering and performance improvements. Third-party applications leverage blockchain performance and throughput support in the most common platform now able to support smart contracts, which is Ethereum. The Ethereum network is now capable of handling millions of applications a day, but this ability is still far behind that of traditional centralized applications. Performance problems in the next two to three years, it is possible to gradually be resolved. [https://blog.ethereum.org/2018/01/02/ethereum-scalability-research-development-subsidy-programs] For third-party applications that immediately require this high-throughput blockchain technology, we The universal asset internet will provide this ability. This can not be achieved if the user bypasses our asset internet and uses the underlying open smart contract directly.

5.  用户的身份管理。区块链技术是基于最主流的密码学技术，在很大程度上，为第三方的应用提供新的安全的标准。它要求所有用户的行为都是安全的，经过认证的，每一个用户都通过自己的密钥为自己的行为进行签字，承担相应的责任。但是管理自己的数字身份本身是一个相对较为复杂的过程和计划，需要缜密管理的一套编程的方法学。我们资产管理协议，能够把较为复杂的，在区块链上的身份管理的工作，提供一个简化的包装。第三方的应用程序使用这样在保证安全性的基础之上的第三方应用，能够充分享受到区块链加密技术提供的方便。身份管理，第三方应用内用户的身份，在过去的世界中往往都是只在自己的应用内的上下文中有意义。进入区块链事件以后，所有用户的资产行为必须和区块链中的一个或者多个账号产生绑定关系。

    User's identity management. Blockchain technology is based on the most popular cryptography and, to a large extent, provides new security standards for third-party applications. It requires that all users behave in a secure manner. Each user, after their authentication, signs their own behavior with their own keys and assumes the corresponding responsibilities. But managing your own digital identity is itself a relatively complex process and plan that requires a well-managed set of programming methodologies. Our asset management agreement is able to bring a more sophisticated package of identity management jobs on the blockchain to provide a simplified package. Third-party applications use this third-party application based on guaranteed security to fully enjoy the convenience provided by blockchain encryption. Identity management, the identity of third-party in-app users, is often only relevant in the context of their own applications in the past world. After entering the blockchain event, the asset behavior of all users must be bound to one or more accounts in the blockchain.

6.  隐私管理。资产互联网协议，将为使用本协议的第三方用户所管理的各类资产提供加密。用户可以完全控制自己的资产在网络中的存储，去控制自己资产的信息向特定的人群或者应用开放。用户可以控制自己资产的转移路径是否公开，或者享有完全的隐私。在资产户联网的层面上，每一个应用内的用户和应用之间是互相隔离的，这样做的主要目的是为了保证用户的隐私。我们的通用数字钱包能够同时导入多个第三方的应用。因为每一个应用之间的互相隔离，实际上一一为着一个钱包可以同时导入用户所知道密码，多个第三方应用所对应的区块链账号。从用户的角度看来，这些账号都隶属于用户自己。能够从统一的资产钱包中，观察自己所拥有的所有的各类和现实世界绑定的加密化资产，以及那些纯粹的加密货币资产。

    Privacy management. Asset Internet Protocol, which will provide encryption for all types of assets managed by third party users using this Agreement. Users have complete control over the storage of their assets in the network and the information they control over their assets is open to specific populations or applications. Users can control their own asset transfer path is open, or have complete privacy. At the asset-user level, users and applications within each application are isolated from each other. The primary purpose of doing so is to ensure the privacy of users. Our universal digital wallet can import multiple third-party applications simultaneously. Because each application is isolated from each other, in fact, one by one for a wallet can be entered at the same time the user knows the password, multiple third-party applications corresponding to the blockchain account. From the user's point of view, these accounts belong to the user. From a unified asset wallet, observe all the types of real-world bond with their own possession of encrypted assets, as well as those purely encrypted currency assets.

7.  工作流支持。工作流的支持，主要体现在多重签名的支持上。关键性的资产的动作，例如资产的转移，资产的交换和资产的销售，往往需要多重签名的保护。应用可以非常简单的设置对关键性动作的签名保护，策略和规则。一旦受到保护的动作被发现或者调用的时候，用户所持的通用资产钱包会自动提示用户进行签名的处理。我可以在自己的资产钱包中实时地对其他人发起的需要多重签名对资产的操作，进行签字或者拒绝的处理。这种工作流，不仅仅可以简单的在持有通用资产钱包的个人用户之间进行，也可以在第三方的应用的界面和拥护者通用钱包之间进行。这一类的多点信息的交流和沟通，是由资产网络底层的基于P2P的消息协议所支持的。

Workflow support. Workflow support, mainly reflected in the support of multiple signatures. Key asset actions, such as the transfer of assets, the exchange of assets and the sale of assets, often require the protection of multiple signatures. Applications can be very easy to set the key action signature protection, strategy and rules. Once a protected action is discovered or invoked, the user's generic asset wallet automatically prompts the user for the signature. In my own wallet, I can sign, or refuse, the processing of assets by multiple signatures of other people in real time. This type of workflow can be done not just between individual users holding Universal Asset Wallets, but also between the third-party application's interface and the Advocate Universal Wallets. This type of multipoint communication and communication is supported by the underlying P2P-based messaging protocol on the asset network.

8.  立即的流动性。 协议和实现中将提供同类资产和跨类资产交易的能力， 特别是提供和成熟加密货币交易的能力。

Immediate liquidity. The agreement and implementation will provide the ability to trade similar assets and cross-border assets, especially to provide and mature cryptocurrency trading.

<!-- -->

## 5.  Protocol
A protocol is a specification of and a normative guide to the exchange and communication of information between and within systems. UDAP's asset protocol regulates how asset are presented, stored, communicated and interacted on the blockchain, how authenticity of assets is verified, and how consensus is reached.

#### 5.1.  On-Chain Asset Model

Traditional ERP systems have established their asset models based on centralized storage and computation. The asset model is an abstraction of the assets created by their issuers, which governs how the systems manage the attributes, operations, and security of assets. Unlike traditional ERPs, UDAP's asset model focuses on an on-chain standardization of the description, interaction, security, privacy, and authenticity of assets.

> Why assets need to be tracked and managed on the blockchain? In general, Crypto assets have the following advantages over digital assets (in this case, traditional ERP-managed assets):
>
1) Clear ownership: The rights and interests of asset issuers, asset owners and transaction signers can all be clearly defined and cryptographically protected. Asset owners can easily provide irrefutable proof of their rights and interests; without the consent of the transaction signers, the assets can not be exchanged and traded on the blockchain; meanwhile, asset issuers have the rights to determine some of the basic attributes of the assets, for example, an asset issuer can restrict the transfer and trading of assets.
>
2) Information Permanence: Digital assets requires a permanent storage to manage their lifecycle. The advent of blockchain and decentralized storage finally gives us confidence that we can save information for a long time.
>
3) Anti-counterfeiting and anti-tampering: Once the assets are on the chain, the relevant data and transaction records can be effectively protected. Anti-counterfeiting and anti-tampering goals can be achieved, and thus moral hazard and financial risks can be reduced.
>
>4) Liquidity Demand: The relationship between value and liquidity is inextricably correlated. Liquidity is the term used to describe how easy it is to convert assets to cash. The more liquid the assets are, the easier their values are to be recognized. So liquidity has a very important influence on asset's value. Money, as medium of exchange, has a very high liquidity. In facet, it is the most liquid asset compared to everything else. Assets with fair liquidity includes cash equivalents such as stocks, bonds and options. And assets such as houses, cars, or farms, factory equipments, etc., have relatively low liquidity and are difficult to value. Therefore their market values may differ significantly. Traditionally, liquidity and value realization are implemented through intermediaries like eBay and Taobao, however, through tokenization blockchain has more potential for liquidity optimization.
>
>
In addition to the above requirements, privacy is also a mandatory need that crypto assets must meet.

Most of the so-called crypto assets in current blockchain world are aimed at a special kind of fungible assets, that is, crypto-currency. Blockchain-based application protocols or platforms are mainly to facilitate the creation, distribution and exchange of crypto assets. Protocols that govern crypto-currencies include ERC20 and some of its simple extensions. For example, one famous third-party trading protocol for fungible assets is 0x protocol. This protocol assumes that digital currencies have been fully distributed among different owners, and that the problem this protocol addresses is to become a decentralized digital asset trading venue, especially for transactions between fungible assets.

Various efforts have been put on standardization and specifications of non-fungible assets, such as ERC721 protocol, which was implemented in the popular CryptoKitties game and its various clones.

UDAP defines a conceptual model based on the analysis and abstraction of various real-world assets in combination with efforts and achievements by MediaChain<sup>\[25\]</sup>, Digix<sup>\[16\]</sup>, BankEx<sup>\[14\]</sup> and other blockchain projects<sup>\[9\]\[10\]</sup>:

<p align="middle">
<img src="media/asset-model-diagram.png" alt="Asset Model" style="width: 500px;"/>
</p>

This on-chain asset model defines assets and related objects, as well as the relationships between these objects. This asset model is compatible with ERC721 but offers a richer set of attributes and operations as described below.

###### 5.1.1 Asset

Anything that is capable of being owned or controlled to produce value, is considered asset. For example, goods, services, trademarks, securities, warehouse receipts, purchase agreements, licenses, copyrights, music, videos, games, loyalty program points, game equipment, event tickets, collectibles and other physical assets and digital assets. Currency (including cryptocurrencies) is also an asset. When you see "asset" in the white paper of a blockchain project, it most likely refers to cryptocurrency.

Assets have attributes. Some common attributes, for example, asset identifier, namespace, issuer, fungibility, transferability, etc., are determined by asset issuers and can not be modified after assets are issued. Other attributes, such as name, description, owner, and states, can be modified during the life cycle of assets. Based on the fungibility of assets, UDAP presents a hierarchical model as described in the following diagram, which defines a standard interface, an abstract type that provides basic attributes and operations, and multiple derived asset types.

<p align="middle">
<img src="media/asset-hierarchy.png" alt="Asset Hierarchy" style="width: 500px;"/>
</p>

The UDAP protocol itself does not specify any implementation details, however, to better describe the model Solidity is used to illustrate the components and their relationships. We may use a more implementation-neutral interface description language to describe the component model in a later version of the protocol.

```
contract Asset is ERC721 {
  event AssetCreated(address indexed _asset, uint indexed _id);
  event AssetTransferred(address indexed _to, uint indexed _id);
  event AssetDestroyed(uint indexed _assetId);

  function id() public view returns (uint);
  function issuer() public view returns (address);
  function owner() public view returns (address);
  function namespace() public view returns (bytes);
  function transferrable() public view returns (bool);
  function fungible() public view returns (bool);
  function metadataHash() public view returns (bytes);

  function transfer(address _to) public;
  function destroy() public;
}
```

* Asset Issuer

  An asset issuer in UDAP refers to the address of a UDAP account that issues and registers assets on asset blockchains. This is a immutable attribute.

* Asset Owner

  An asset owner refers to the address of a UDAP account that owns crypto assets registered on the asset blockchains.

* Fungibility

 Fungibility refers to interchangeability of assets with the same amount and of the same type. Based on asset fungibility, assets are usually classified into two categories: that can be replaced and that can not be replaced. In the asset model, the two types correspond to FungibleAsset and StandardAsset, respectively. An non-interchangeable asset means that although both individual assets have similar attributes and external behaviors, their possession is not replaceable for a particular owner because they have different identities. This is analogous to the fact that although both have iPhones, there is no substitute between an iPhone and another iPhone because each iPhone has its own unique attributes that make it disappear if the iPhone is switched. Each iPhone has its own unique phone number and a unique purchase time, so between the two iPhone they are not interchangeable with each other, at least in most cases.

 In the physical world, there are a large number of assets that can not be easily interchanged. For example, most of the real estate properties can not be replaced during the transaction. Other examples include financial assets such as stocks and debts, which are non-fungible assets in many business scenarios.

 The most common of what we call fungible assets is money or digital currency (AssetToken in UDAP term, which is also an ERC20 token). In most cases, one hundred dollar bill is completely equal to and replaceable with another one hundred dollar bill because the main purpose of using one hundred dollar bill is to use one of its most prominent attribute, medium of exchange. Although each bill has some special attributes, such as its unique serial number printed on the the paper bill, it has no specific significance and influence in most cases. Therefore two hundred dollar bills are completely replaceable. Another example of fungible assets is commercial goods, such as apples in a warehouse. Although apples have some special attributes, such as origin, variety, grade, size, color, etc, however, when we say that we have 600 tons of Yantai-produced first class Red Fuji apples with a size of 85mm, these 600-tonne apples are traded as fungible assets because the 600-tonne apples are classified as one group according to industry specific standard. There is no difference to the buyer in the trade.

 One special type of non-fungible assets, which is referred as CompositeAsset in the asset hierarchical model, is composite asset or asset portfolio. This type of assets typically contains a number of other assets, for example, asset portfolio in the financial sector, warehouse receipts in the supply chain, and many asset bundles that require the packaging of different assets as a whole for trading. Below is the definition of the interface.

 ```
 contract CompositeAsset is StandardAsset {
   function getAmount() public returns (uint);
   function getAsset(uint idx) public returns (address);
 }
 ```

* Transferability

  The transferability of assets determines whether an asset can be transferred to other institutions or individuals after being issued. Transfer of asset can be done either by direct sale or through exchange. If an asset is not transferrable, then its ownership cannot be changed.

* Resellability

  Resellability is a special attribute that asset issuers can use to restrict the resale of assets. Although in most scenarios assets are re-sellable, in certain special cases, such as shopping vouchers, issuers can restrict the resale of vouchers. In this way, the vouchers can not be transferred or sold after the vouchers have been issued to them, thus limiting the circulation of such assets in the secondary market and ensuring that such assets are available only to recipients designated by the issuer.

* Namespace

  An asset namespace refers to the naming rules for asset classification and grouping so as to facilitate the distinction between different assets. Namespaces are commonly structured as hierarchies to allow reuse of names in different contexts, for example, a warehouse receipt can be identified via udap://xinong/wr/WR-12345678, where "xinong" is the registered app name (or chain name), "/wr/WR-12345678" is the namespace id given by the app (or chain) to identify a warehouse receipt coded as WR-12345678.

* Asset Identifier（AID）

  Asset identifiers are unique identification codes set by the UDAP platform for assets and are automatically created for each asset by a standard algorithm as follows:

  ```
  AID = uint(keccak256(issuer_address, namespace, metadata_multihash))
  ```
  This algorithm generates a unique AID for an asset with its issuer's account address, its namespace, and the hash value of the asset metadata description file in IPLD or JSON-LD format. Assets issued by different asset issuers, or assets issued by the same asset issuer but with different namespace id, or different asset metadata descriptions, will receive different AIDs.

* Metadata MultiHash

  It refers to the content-addressable MultiHash value that is generated from asset metadata to uniquely address the asset's metadata. See 5.1.2 for details about asset metadata.

* Other Attributes

  In addition to the above attributes that usually can not be changed once identified, assets also have mutable attributes that can be updated after issuance, such as the amount of fungible assets (e.g., 1 kg of gold, or 500 tonnes of apples), the state of the asset (leased, unused, listed, etc.), ownership, proof of assets, description, etc.

###### 5.1.2 Asset MetaData

Metadata is commonly referred to as "data about data." In UDAP asset metadata refers to the descriptive information applied to assets and is defined by asset issuers. The structure and meanings of these metadata are known to asset issuers and the associated applications. In UDAP, asset metadata is presented as JSON data in conformity with JSON-LD specification, and is stored off-chain, while on-chain crypto assets must hold Multihash values of their off-chain metadata. Smart contracts can obtain the multihash value through the metadataHash() method to address and retrieve the related asset metadata.

````
  function metadataHash() public view returns (bytes);
````
> JSON-LD, or JavaScript Object Notation for Linked Data, describes how linked data is represented in JSON as a directed graph, and how to represent interlinked and non-interlinked data in a single document. For example, metadata about a recipe asset can be recorded in JSON-LD format (shown below) and published to IPFS or other P2P storage. Typically, asset metadata can be encrypted before posted to P2P storage to enforce data privacy.

````
{
   "name": "Mojito",
   "ingredient": [
     "12 fresh mint leaves",
     "1/2 lime, juiced with pulp",
     "1 tablespoons white sugar",
     "1 cup ice cubes",
     "2 fluid ounces white rum",
     "1/2 cup club soda"
    ],
   "yield": "1 cocktail",
   "instructions": [
      {
        "step": 1,
        "description": "Crush lime juice, mint and sugar together in glass."
      },
      {
        "step": 2,
        "description": "Fill glass to top with ice cubes."
      },
      {
        "step": 3,
        "description": "Pour white rum over ice."
      },
      {
        "step": 4,
        "description": "Fill the rest of glass with club soda, stir."
      },
      {
        "step": 5,
        "description": "Garnish with a lime wedge."
      }
   ]
}
````
> The above metadata can be recorded as a merkle-link on the blockchain so that applications can address through merkle-link to obtain the relevant off-chain asset metadata.

```
{"md",{"/","QmdnuRNwdmZzHfHVUMVHZFXKXAe6DjvBvPdKy27HpJUN9H"}}
```

> UDAP adopts a simple method to record only the multihash value on the blockchain which points to the off-chain metadata. The specification defines how to obtain content-addressed objects through the hash value.

```
{"metadataHash","QmdnuRNwdmZzHfHVUMVHZFXKXAe6DjvBvPdKy27HpJUN9H"}
```

>Usually applications need to address each item of metadata to obtain the resolution of the related data. Therefore, the content-addressable network data model is used to address the asset metadata through the merkle-path. For example, IPFS DAG's javascript interface (ipfs.dag.put) can be used to upload metadata of the recipe asset to the IPFS so that each metadata item is available by invoking "ipfs.dag.get".

>Metadata on IPFS as DAG node:
```javascript
  ipfs.dag.put(metadata, { format: 'dag-cbor', hashAlg: 'sha3-512' },
    (err, cid) => {
      console.log(cid.toBaseEncodedString())
    // zdpuAz4HbUHTKQbdpnn42Zo4GUsU7yrBpvb2W9BF2NwvBaLn6
  })；
```
>DAG node through merkle-path:
```javascript
 ipfs.dag.get('zdpuAz4HbUHTKQbdpnn42Zo4GUsU7yrBpvb2W9BF2NwvBaLn6/name',
  (err,result)=>{
    if (err) {
      console.error('error:'+ err);
    }
    else {
      console.log(result.value);
    }
 });
```

###### 5.1.3 Ownership

The ownership of an asset is a type of asset metadata that tracks who owns an asset. An asset can have multiple owners. The ownership of assets can be changed over their lifecycle, for example, when an asset is transferred to another person from current owner, the ownership of this asset is changed. In UDAP asset protocol, while asset ownership belongs to a type of metadata, UDAP manages asset ownership as an independent attribute that can be tracked by a smart contract defined as follows:

```
contract Ownership {
  function ownerOf(address asset) public view returns (address);
  function ownerOf(address asset, uint asOf) public view returns (address);
}
```

The above interface gives the caller the capability of obtaining current owner account of an asset as well as the owner account as of a given time in the past.

###### 5.1.4 Asset State and Lifecycle

Asset states can be used to accurately track assets at a detailed level. In addition to a few pre-defined asset states such as CREATED, TRANSFERRED, PLEDGED, LEASED, applications can define and name their own states according to business needs and record asset states on the blockchain via UDAP.

The life cycle of an asset refers to asset state at different points in time. One of the main functions of UDAP is to provide asset lifecycle management APIs on the blockchain that allows applications to track the entire lifecycle of assets from issuance to destruction to meet various business needs.

Asset lifecycle can be represented with a smart contract as follows:

```
contract Lifecycle {
  // returns current state of a given asset
  function stateOf(address asset) public view returns (bytes32);
  // returns the state of asset at given asOf time
  function stateOf(address asset, uint asOf) public view returns (bytes32);
}
```

###### 5.1.5 Proof of Asset

Proof of Asset (PoA) is an important concept of the UDAP asset model. It is one of the key elements in determining the authenticity of assets. It is also a type of asset metadata in the UDAP asset model, represented as an array of JSON objects in JSON-LD or IPLD format. Each of the JSON objects defines a proof including name, description, and a content-addressable linkHash value of the "proof". The "linkHash" represents a MultiHash value that can pinpoint this proof, which may be a digitally signed PDF file or a scanned shopping receipt. Proofs are stored off-chain and can be obtained through the metadata's merkle-path.

```
"proofs":[
  {
    "name":"Storage Contract",
    "description":"Storage contract for warehouse receipt #123456",
    "linkHash":"QmWwr4ZfeLJfbWNAuCQfefwo1aHtxC5yjyU8C5WG4DYrYe"
  }，
  {
    "name":"Purchase Receipt",
    "description": "Purchase receipt for warehouse receipt #123456",
    "linkHash" :"QmXF4LR4QkuRVh3WQbB56seTX2aPm3Tz7b4Y8heoLAiTkk"
  }
]
```

Proof of Asset is an optional but important attribute of crypto assets. Usually asset buyers will require some sort of proofs, however, without a proof an asset can still be traded or exchanged on the market. More discussions about Proof of Asset can be found in 5.3.

Proof of Asset may have different forms in different use cases. For example, in the supply chain warehouse environment, a warehouse receipt is a proof to demonstrate the authenticity of the assets. Other relevant proofs include purchase agreement, storage contract, third-party certificates, etc. Who owns the warehouse receipt owns the rights of goods stored in the warehouse; in the manufacturing sector, manufacturers can use RFID tags or two-dimensional bar codes to uniquely identify their products. In this case, RFID of a product is a proof that demonstrates the authenticity of this product. As such, proofs are data defined and provided by crypto asset issuers to prove the authenticity of assets that can be either numbers or files or images, all in JSON-LD format.

###### 5.1.6 Tags

Asset tags are keywords or labels that are attached to assets to facilitate identification, classification, retrieval, and inventory control of assets. Multiple tags can be given to an asset by its issuer or owner. Asset tags enable applications in a variety of industries to track and monitor valuable assets.

###### 5.1.7 Asset Registry

An asset registry maintains a bi-directional binding between crypto assets and real-world assets on the blockchain. All assets posted to the UDAP blockchains need to be recorded in the asset registry by its issuer. At the same time, the asset registry also maintains a number of different data structures and indexes to simplify search and retrieval of assets. Different institutions or applications have their own proprietary registry of assets. Asset issuers can broadcast their assets across the entire network or just to some designated addresses, so that a proprietary registry has access to assets registered in other registries via listeners. For example, landlords can post rental information on multiple rental sites simultaneously, and sellers can initiate auctions on both Site A and Site E. When an asset on Chain A is transferred to an address on Chain B, UDAP must ensure the removal of this asset from the registry of Chain A, and the addition of this asset to the registry of Chain B.

###### 5.1.8 Account, Wallet, and Identity

Accounts are users' address on the blockchain. A user may have multiple accounts, while an account may have multiple assets. An asset may be associated with multiple accounts. For example, an asset can have multiple owners, an issuer, and multiple signatories. An account can also play different roles in different trading scenarios, e.g., asset issuer, asset owner, or transaction signer.

> Asset signatory refers to the account that signature of transactions is required before trading the asset on the UDAP blockchains.

An asset wallet, similar to a safe or a deposit box, is a universal wallet provided by UDAP to allows tracking and management of assets associated to a user's account. An asset wallet can manage multiple accounts, each associated with multiple assets on the blockchain.

Identity refers to the user's personal or social information, for example, ID card, Facebook account, e-mail address, phone number and other information that can represent the user's identity. Blockchain accounts are anonymous, but in some scenarios users have to provide proof of identity to complete the regulatory requirements for KYC and AML. UDAP, in conjunction with a self-governed third-party identity management system such as uPort, provides the application with a mapping of identities to UDAP accounts and asset wallets.

###### 5.1.9 Transactions and Events

Transactions refers to any operation on the assets on the UDAP blockchain. For example, issuance, exchange, ownership change, minting, recasting, pledge, approval and so on are all transactions. When a user initiates a transaction on the UDAP blockchain, the UDAP generates related events and broadcasts to related listeners, which are responsible for processing the transaction.

#### 5.2.  Asset Services

On top of the asset model, UDAP has defined a service model for asset operations and management.  Common services are exposed to application developers through micro-services (REST APIs and WebSockets). Unlike the traditional centralized cloud service model, UDAP provides a decentralized service architecture. In this decentralized service architecture, the API gateway and service host are a special type of miners that provide the host container for running UDAP asset services. The gateway is the entry point for third-party applications to connect to the UDAP blockchain, and is responsible for automatic routing application requests, and provides service metering capability as a basis for service charges. At the same time, the nodes that provide the service gateway and the service container are also rewarded by the network. Hosts providing asset services need to deposit a small amount of locked-in tokens and need to broadcast their identities to the UDAP blockchain. UDAP chooses the node serving the service based on the proof of the node.

<!-- 图 -->

###### 5.2.1 User Registration
User registration establishes the mapping between the user space of an application and the user space of UDAP blockchain. User accounts between different applications are completely isolated. See 5.4 for more description.

###### 5.2.2 Application Registration
The main purpose of application registration is that developers can get the App Key and App Secret to connect to the UDAP blockchain, and the registered app name is used as the level 0 namespace id of the managed assets.

###### 5.2.3 Asset Registration
Assets need to be registered on the UDAP blockchain for applications to query and manage their states on the blockchain. In the meantime, applications receive asset registration information broadcast by other applications, enabling cross-application and cross-chain asset transfer and trading. Assets registration is a two-way binding process between real world assets and crypto assets. Asset metadata is identified and uploaded to off-chain P2P storage network at this stage, and a hash value of the off-chain metadata is stored and associated to the crypto assets. In this process, asset issuers need to make detailed configuration of asset attributes, for example:

-   Transferability：an asset can be either transferrable or non-transferrable. If an asset is not transferrable, the asset is usually a warrant asset. The only meaningful operation is "delivery", which means that the warrant owner delivers to the original issuer the promised product or service.

-   Sellability：an asset can be either sellable or non-sellable, which defines the ability to be sold. If the asset is configured to be non-transferrable, the asset is essentially non-sellable.

-   Multi-signature requirements: A multiple signature (or multisig for short) requirement represents that a transaction requires multiple approvals from different participants. Multi-signature addresses and transactions broaden this model by creating identities on the chain which are managed collectively by multiple parties. UDAP uses “m-of-n” bitcoin-style multi-signatures, in which a multisig address A is defined as: Given n regular addresses, at least m of the private keys corresponding to those addresses must sign a transaction to perform an action for A.

###### 5.2.4 Tokenization

The purpose of asset tokenization is to make asset transfer and trading more easier. This is a fairly frequent operation that the asset issuer completes mapping from the real world to the crypto world after registering a real asset attached to the application context to UDAP. Token issuance allows assets to be traded in part rather than as a whole. For example, a painting can be tokenized as a certain amount of tokens through what is sometimes called "tokenization" (sometimes referred to as "minting,") so that the painting can be sold to multiple owners, where each owns a portion of the rights and interests of the painting.

As seen from the UDAP asset model, tokens are fungible assets. Fungible assets are usually tokenized at the time of registration, whereas non-fungible assets are traded as a whole in most scenarios and therefore do not require the issuance of tokens. It is only necessary for issuers to mint tokens when they want to trade their assets partially.

###### 5.2.5 Asset Recast
Recasting refers to the process of burning tokens for the rights to redeem goods or services, which creates new proof of asset for the token owner. This process is usually valid for physical assets in specific scenarios. This is because tokens themselves do not necessarily have the associated attributes of physical assets and the tokens are issued by the asset owner to enhance liquidity. When the physical asset is in the custody of a third party, the tokens issued by the asset owner may not always be accepted directly by the custodian of physical assets. Therefore, in many cases, tokens can not be used to directly redeem physical assets and new crypto assets need to be generated through the process of "recasting". For example, after Alice registers her 500-tonne apple on the blockchain to form a crypto asset (crypto warehouse receipt), Alice can issue a token per tonne. Alice then transfers 100 tokens (corresponding to 100 tonnes of apples) to Bob. After Bob receives 100 tokens, he can submit the tokens to the UDAP recast contract to generate a certificate to redeem asset (e.g., bill of lading) and destroy the corresponding tokens. Then Bob can redeem goods with this bill of lading. After redemption, the related crypto assets (warehouse receipts) are automatically destroyed on the blockchain to prevent double spending.

###### 5.2.6 Multisig
Multisig is an additional security protection mechanism in the process of asset trading. It refers to the process that multiple accounts digitally sign the same transaction before it is executed. Only when required signatures are collected will the transaction be broadcast to the chain. In many scenarios multiple signatures are required to complete a specific asset operations, for example:

- Registration: For expensive assets, the application may require signatures of the designated accounts be provided at the time of asset registration in order to prove the authenticity of the asset. Auditors and witnesses are possible co-signers in this process.
- State Change: Some key state changes may need to be confirmed by multiple parties.
- Trading: Co-ownership of assets requires the signatures of multiple owners when assets are transferred or sold to a third party.
- Pledging: Pledges usually require multiple approvals to ensure authenticity of assets, accuracy of price, and security of transaction.
- Asset freeze (冻结): The asset freeze may require the signature of the court and the parties involved.
- Asset write-off (核销): This operation usually requires the approval from multiple supervisors. For example, reimbursement process requires the signatures of direct managers and CFO to complete expense reimbursement.

###### 5.2.7 Other Asset Services

In addition to the basic services described above, UDAP provides the following services:

- transfer
- rent
- buy and sell
- C2C trade
- pledge
- auction
- escrow
- redemption and destruction

#### 5.3. Authenticity and Proof of Asset

UDAP assumes a few basic principles about the authenticity of assets:

- 任何资产的真实性必须在管理这种相关应用中的上下文里谈论才有意义。
- 资产的权威性和真实性可以由第三方的应用通过他们认为可靠的和足够的机制来确立。
-
- Authenticity is not protected by the UDAP protocol.
- Authenticity is only valuable in its application context.
- The authority and authenticity of assets can be confirmed through a mechanism that is considered to be reliable and adequate by participants.

UDAP is a distributed system. It does not have a single operating entity to verify the authenticity of assets. While asset verification may be done in a distributed and decentralized manner, UDAP currently does not design such mechanism.

However, if a person claims a crypto asset that he owns on the UDAP network is backed by a real-world asset, how could he prove this claim? UDAP proposes following guidance:

1）Proofs of Asset

Under normal circumstances anyone can issue assets on the blockchain via an app. At the time of asset issuance, the issuer has to provide a detailed description about the asset in the form of texts, images and other media. The issuer may also present some real-world confirmation of the asset, for example, a certificate of property, an impartial letter, a warehouse receipt, a purchase receipt, and so on. All of these supporting documents do not necessarily guarantee the authenticity of the assets, but these additional attributes to a certain extent increase the authenticity of the assets.

2）Guarantee or Insurance

Asset issuers or owners can guarantee the authenticity of the assets by providing some form of guarantees or insurance.

3）Multisig

Asset issuers can leverage the multi-sig mechanism in the registration process to enhance the authenticity of assets. In this process, multiple proofs from related parties are usually required.

The first step in enhancing the credibility of assets is when assets are mapped from the real world to the crypto world, which is what we mean by registration. With the support of UDAP, a multi-party signature must be provided when an issuer declares an asset on blockchain. The signature comes from the current owner of the asset. Other signatures may be obtained from current custodian of the asset, the notary and the third party auditor who verify and confirm the ownership of the asset.

If a third-party application considers that the registration of a user's asset is important, it can leverage the multi-signature mechanism provided by UDAP to allow the relevant guarantor (including asset custodian, notary and auditor) of the asset during asset registration to submit proofs of asset and sign the transactions. For example, if a person claims that he owns a gold bar himself, the application requires that the user must, at the same time as the declaration, submit a gold asset certificate issued and signed by a custodian that certifies such ownership, as well as the digital signatures and associated certificates from other third party auditors. In the absence of any of these digital signatures will result in the denial of asset registration.

4）Escrow

The ultimate value of assets is achieved through circulation. Escrow is a common method of trading assets between untrustworthy individuals. The owner of an online store may claim to own any goods. The platform does not recognize the credibility of such claims. Instead it offers a custodian mechanism that usually holds temporarily assets that are easily deposited by both parties in the transaction, for example, purchases of ordinary merchandise from an e-Mall, the money paid by the buyer does not go directly to the owner of the goods, but goes into the escrow contract first, and then the buyer must confirm the authenticity of the goods after the buyer receives the goods. The traditional e-commerce platform basically adopts this kind of mechanism. For example, on the localbitcoin.com platform (http://www.localbitcoins.com), the escrowed objects are the commodities to be traded, that is, bitcoin, while the money to buy bitcoin is paid offline.

For those products that are very expensive, there may be a need for multiple protection mechanisms, for example, a combination of above mechanisms, which prevents possible fraudulent activity during asset trading. UDAP provides API for third-party applications to establish a flexible mechanism to ensure the authenticity of assets and to ensure the reliability of the transfer process.

#### 5.4. Identity Management

The main purpose of UDAP is to manage real-life assets with blockchain technologies, and to use these technologies to increase their liquidity and thus enhance its permanent durability. At the same time, one important goal of UDAP is to allow these real world assets in the form of crypto assets to be easily transferred among owners.

The first and foremost problem is the identity of the participants in the asset related transaction. For real-world asset transfers, it may not be enough to know only the account numbers. Because the conversion of these assets may involve the requirements of the real identity, for example, a contractual relationship established by the two sides through the asset network, if traceability is important, then the identity of the parties have very clear requirements. The two parties to the contract need to know each other very clearly, that is, the individual that they want to make the transaction. Once the contract is in trouble during execution, there is always another way for the contract party to track and confirm the problem in the real world. Considering again that if third parties' law enforcement agencies are able to participate in this process, the identification of the identities of both parties to the contract is a prerequisite for their participation.

Each application will determine how much they need to be aware of the identity of the user in the real world. In more stringent applications, they may need to be fully aware of the ID of the user of the application in the real world, his address, and his contact details. For example, a cryptocurrency exchange may require users to submit their own proof of identity in real life, such as ID cards, passport photos, and to verify their phone number and EMAIL address. Moreover, proof of their places of residence may be required and fully verified. In fact, this is the basic verification process that most of the major crypto exchanges are conducting. Other applications may not have such KYL requirements. Maybe they just need to know the registered user's EMAIL address, or maybe they are not interested in knowing any of these information.

There are several types of identity management systems on the Internet:

- Fully centralized identity management system, such as citizen ID card system.
- Fully siloed authentication system, for example, each application has its own authentication system.
- Federation Identity System: Internet applications that have taken shape to a large scale provide authentication for other applications through OpenID, OAuth, or similar mechanisms. The provided process can add user's confirmation of identity and additional property exposure.
- Self-Sovereign Identity Management.

Given that UDAP provides an open ledger service to third-party applications, we decide to adopt an evolutionary path for UDAP to transition from a Siloed identity system to a Self-Sovereign identity system:

In the first phase of UDAP Identity Management:

- 一个人的身份由第三方的应用所确定。在应用之外没有抽象的身份。也就是每一个应用对应于一个 persona。 UDAP 不追求作为单一的identity provider。 应用身份的独立性能够提供隐私保护和账号的安全。
- 在应用级别的用户的创建是应用自身的工作， UDAP不参与。
- 应用用户需要注册到UDAP体系中也是通过相应的应用完成。
- identity认证过程和资产认证一样留给应用或第三方认证机构。identity认证对某些场景来说是必须的，但是不是UDAP的责任，应用只需要保证提交给UDAP存放的hash和提交给第三方认证的是一致的，这样一旦第三方认证机构认可了用户的identity，那么UDAP就可以确认这个用户是他所申明的身份。

- A person's identity is provided by a third-party application. There is no abstract identity outside of the application. That is, each application corresponds to a persona. UDAP does not pursue as a single identity provider. The independence of application identity can provide privacy protection and account security.
- Applications are responsible for user account setup. UDAP is not involved in this process.
- Applications are also responsible for creating UDAP blockchain accounts for their users.
- Identity verification is the responsibility of applications or third-party certification organization. Applications need to ensure that the hash value submitted to UDAP is the same as the one submitted to the third-party certification organization. Once the third-party certification organization has approved the identity of the user, then UDAP can confirm that the user is his identity.

In the second phase of UDAP Identity Management:

- UDAP provides a decentralized PKI interface (dPKI) to third party apps.
- UDAP integrates a Self-Sovereign identity system that allows users to have multiple identities and have full control over the use of their identities across applications.
- Asset Wallet (UAW) provides Hierarchical Deterministic account creation and management mechanisms.
- UDAP supports account recovery to prevent users from losing their identities if their devices or passwords are stolen or lost.

We are looking closely at the development of some third-party identity management systems and will consider the possibilities of integrating their services into UDAP network. These systems include (but not limited to) uPort, ShoCard, Civic, Mooti, ​​and others.

## 6.  通用资产钱包 (Universal Asset Wallet， UAW)

![](media/image3.png)

作为平台的一个非常重要的部分，钱包扮演了一个整个协议和系统和用户之间交互的关键角色。一般加密货币的钱包是单一功能的钱包，展示的是某一种特定的加密货币的数量。多功能的钱包同时能够支持多种数字加密货币的结余展示和资金发送和收取。

As a very important part of the platform, wallet plays a key role in the entire agreement and interaction between system and user. The usual crypto-wallet is a single-function wallet that shows the amount of a particular cryptocurrency. Multi-functional wallets can also support the display of multiple balances of digital cryptocurrencies and the sending and receiving of funds.

UAW作为通用资产钱包，他的角色被更加的扩大。 把它想象成是一个个人的保险箱，其中不仅有各种各样的货币，同时还有各种各样的有价证券，文件，以及任何被个人认为是理解成资产的物件的代币。
通用资产钱包不仅仅是资产的存储空间，同时也非常方便的用于支持对资产的一些通用的操作，例如资产的转移，销售， 交易， 拍卖，注销等。

UAW as a general-purpose assets wallet, his role has been more expanded. Think of it as a personal safe, not only in a wide variety of currencies, but also in a wide variety of securities, documents, and any tokens that individuals perceive as objects of understanding.
General Assets Wallets are more than just the storage of assets, but are also very handy for supporting common operations on assets such as asset transfers, sales, trading, auctions, cancellation and more.

UAW包含以下资产内容：

1.  从第三方App沉淀的资产： 例如各种票券， 各种权证， 各种契约。
2.  个人创建的加密资产： 例如个人契约。
3.  账单和债务： 例如各种应付账单， 借债。

UAW contains the following asset content:

1. From the third party App settling assets: such as various tickets, all kinds of warrants, all kinds of contracts.
2. Encrypted assets created by individuals: for example, personal contracts.
3. Bills and debts: such as various bills payable, debt.

#### 6.1.  从第三方App沉淀的资产
Assets precipitated from third party App

UAW沉淀的是用户在各种第三方应用中得到的资产.
各种第三方应用中都有独特的帐号， 账号之间没有关联。这被称之为账户隔离。
每一个应用自身有一个独特的用户管理体系，它所产生的用户账号对应于区块链上的一个独特的账号。账号在应用之间不会重用。
一个账号只在第三方应用的上下文环境中才有安全意义和身份，这样做的目的是保证，用户的隐私。在这样的前提下，一个钱包，实际上必须从每一个用户所使用到的第三方应用中导入自己的资产。导入资产的过程。和支持ERC20协议的Ethereum链上的发行的加密货币的原理是一样的。导入账号以后，在第三方应用中对应用户的资产，会，分门别类的呈现在通用资产钱包中。用户可以理解使用第三方应用资产发售者所许可的各种操作，例如转移，提交到市场销售，竞价拍卖，或者给第三方发送拷贝。

UAW is the user of the assets obtained in a variety of third-party applications.
A variety of third-party applications have a unique account, there is no correlation between accounts. This is called account segregation.
Each application has its own unique user management system that generates user accounts that correspond to a unique account on the blockchain. Account will not be reused between applications.
An account only in the context of third-party applications have a security significance and identity, the purpose of doing so is to ensure that the user's privacy. In this context, a wallet, in fact, must be from each user to use third-party applications to import their assets. The process of importing assets. The same principle applies to cryptocurrencies issued on the Ethereum chain that supports the ERC20 protocol. After the account is imported, the assets of the corresponding user in the third-party application are displayed in the general-purpose assets wallet in different categories. Users can understand the various actions licensed by third-party application asset vendors, such as transferring, submitting to marketing, auction auctions, or sending copies to third parties.

#### 6.2.  资产来源之二：个人创建资产
Second sources of assets: individuals to create assets

UAW不仅仅从第三方的应用导入各种用户的在第三方应用上下文中积淀的资产，同时它允许用户直接在钱包中创建个人化数字加密资产。

UAW not only imports assets from various third-party application contexts from third-party applications, but it also allows users to create personalized digitally encrypted assets directly in the wallet.

个人创建资产分为两类：

Individuals create assets into two categories:

1)  一种场景是用户可以直接在通用资产钱包中创建[借条]{.underline}或者[欠条]{.underline}这一类的"[加密合同]{.underline}"或者"加密契约"。借条和欠条在日常生活中的目的是表明A用户因为借贷的原因欠B用户某种特定的资产，并且相约在某个时间可以进行偿付。在现实生活中，可能人们会在一张纸上写下这种关于资产的约束和承诺。它的法律意义是由这种签名所决定的，一旦出现争执，需要进行权威机构的验证和仲裁。通用资产钱包是基于区块链的取证和仲裁，从钱包中开出的借条和欠条，因为其无法篡改和无法凭空捏造的能力，其证据能力实际上优于现实生活中的手写的欠条或者借条，字据的真实性一目了然，所以加密合同是更为方便和更有约束力的契约。

    One scenario is that users can create either [Encryption Contracts] {.underline} or Encryption Contracts in the generic asset wallet directly under {IOU} {underline} or {IOU} {underline}. The purpose of IOUs and IOUs in daily life is to show that A users owe a particular asset to a B user because of borrowing and can pay for it at some time. In real life, people may write down this kind of restraint and commitment about assets on a piece of paper. Its legal significance is determined by such a signature, in the event of a dispute, the need for verification and arbitration authority. General Assets Wallets are based on blockchain forensics and arbitration. IOUs and IOUs are derived from wallets because they can not be tampered with and can not be invented, and their evidence capabilities are actually superior to real-life handwritten IOUs or IOUs , The authenticity of the document at a glance, so encrypted contract is more convenient and more binding contract.

![](media/image4.png)

创建用户打开个人功能然后点击书写借条或者欠条。描述发生的借贷关系和偿还安排。然后就可以发送给债权人。债权人确认签名后就成为自己个人资产的一部分。等到未来的某个时刻交割，就完成了这个借条或者欠条的生命周期。

Create a user to open personal features and then click to write IOUs or IOUs. Describe the loan relationships and reimbursements that take place. Then it can be sent to creditors. Creditors confirm the signature became part of their personal assets. Wait until sometime in the future delivery, to complete the IOU or IOU life cycle.

在个人打借条或者欠条的过程中，还可以利用钱包所提供的多重签名的属性。例如在做一张借条或欠条的时候，可能需要一个第三方的见证人见证这张欠条额内容有增强的，这个可靠性和有第三方的在场，那么在书写欠条借条的过程中，他可以把原始的欠条发送给见证人，然后见证人进行签收以后，最后发送给债权人。

In the process of personal loans or IOUs, you can also use the wallet to provide multi-signature properties. For example, when making a IOU or IOU, a third-party witness may be required to witness the increase, the reliability and the presence of a third party, so that he can Send the original IOU to the witness, who then signs the receipt and sends it to the creditor.

甚至引入[担保人]的角色。和[见证人]不同，担保人和，债务人，要承担，相应的担保的义务，如果债务人不能。约定的时间进行债务的偿还，那么担保人要负连带的偿还义务。能和通常的。见证人的多方签名的流程相似，使用的都是相似的机制。从侧面表明了通用资产钱包所自带的多重签名的功能的强大性。

Even introduce the [guarantor] role. Unlike the [witness], the guarantor and the obligor have to assume the corresponding obligation of security if the debtor can not. The agreed time for debt repayment, then the guarantor to bear the repayment obligations. Can and usual. Witness multi-signature process is similar, using a similar mechanism. From the side of the common asset wallet that comes with the power of multiple signatures.

如果合同的资金交付方式选择系统支持的加密货币，那么合约的交割方式更为便捷，用户只需向合约汇入相应的款项，合约即可自动执行完毕，债务债权关系自动解除。基于加密货币的偿还安排还可以支持利息处理，合约会按照双方约定的利息在触发条件（例如，出现偿还逾期）满足以后， 自动开始计息。

If the contract's funds are delivered in the form of cryptocurrencies supported by the system, the delivery method of the contract is more convenient. The user only needs to import the corresponding payment into the contract, the contract can be automatically executed and the debt claims are automatically released. Reimbursement arrangements based on cryptocurrencies can also support the treatment of interest and the contract automatically begins to accrue interest upon satisfaction of the trigger conditions (eg, overdue repayments) as agreed between the parties.

加密契约可以是高度格式化的， 也可以是用高度灵活形式，例如除了文字以外， 可以使用图片， 语音甚至视频。所有的这些媒体形式都会被签名加密，具有高度的隐私和高度的安全性。

Encryption contracts can be highly formatted or highly flexible, for example, pictures, voices and even video can be used other than text. All of these forms of media are signed and encrypted with a high degree of privacy and high security.

仔细思考这个功能， 这是一个极为强大的功能设计，

Think carefully about this function, which is an extremely powerful functional design,

    a.  节省了公证的繁琐和成本

    b.  保存极为方便

    c.  个人债务可以转让流通

    d.  合约交割及其简单。



     a. Saving notarization and costs

     b. Very convenient to save

     c. Personal debt can be transferred and circulated

     d. Contract delivery and its simplicity.


2)  个人物件资产代币化。 此种模式下, 用户可以自己通过文字或者图片或者视频的描述，产生一个用户资产登记卡。完成以后可以把它进行转移，或者放到市场进行销售，就和普通的电子商务平台的产品上架的过程一样。个人用户完全可以把，通用资产钱包，当成一个电子商务平台来对待。

    Personal property assets tokenization. In this mode, the user can create a user asset registration card by himself or herself through the description of words or pictures or videos. After the completion of the transfer can be carried out, or put on the market for sale, and ordinary e-commerce platform products on the shelves of the same process. Personal users can put, general-purpose assets wallet, as an e-commerce platform to treat.

#### 6.3.  负债：the Bills

UAW除了管理财务意义上的资产，同时还管理负债， 或者称之为"负资产"。

UAW manages assets in the financial sense while also managing liabilities, or "negative assets."

通常我们所说的资产一般是指的对自己有价值的部分，但是在很多场景下。一个人不仅需要知道自己拥有多少资产，同时也需要拥有多少负债，以及这些负债的偿还要求和条件。
从严格的意义上来说，UAW
呈现的不仅仅财务记账中的体现"资产"的一半，而且体现了自己的整个财务状况，包括资产和负债。

Often, what we mean by assets is something that is valuable to ourselves, but in many scenarios. A person not only needs to know how much assets he owns, how many liabilities he also owns, and the reimbursement requirements and conditions for those liabilities.
In a strict sense, UAW
Present not only half of "assets" in financial books but also one's own financial position, including assets and liabilities.

当一个人向第三者开出一张借条，或者欠条的时候，对方作为债权人拥有的是正资产，而己方作为债务人拥有的是负资产。作为负资产，虽然你希望它消失，
或者倾向于把它忘掉，但是实际上债务人需要经常提醒自己不能违约。

When a person places an IOU or IOU with a third party, the other person owns a positive asset as a creditor and the other person owns the negative asset as a debtor. As a negative asset, though you want it to disappear,
Or tend to forget it, but in fact the debtor needs to constantly remind himself that he can not default.

在UAW中，
当使用者开出一张欠条或者借条的时候，他/她会在钱包中看到一个代表这个债务的负资产。

In UAW,
When a user places an IOU or IOU, he or she will see in the wallet a negative equity representing the debt.

负资产最常见的例子就是每月如期到来的各种"utility bills":
水/电/气/电话账单。 电力公司， 电话公司，
甚至信用卡公司通过我们标准的借口，
可以把用户的各种账单直接投资到用户手中。
用户可以利用钱包自带的支付能力（法币的或者加密货币的）直接在UAW中支付，
或者可以转给其他人代为支付， 例如夫妻之间可以商量选择支付人，
孩子可以让父母为自己的电话或者信用卡支付账单。

The most common example of negative equity is the various types of "utility bills" that arrive on a monthly basis:
Water / electricity / gas / telephone bills. Power companies, telephone companies,
Even credit card companies through our standard excuse,
Users can invest various bills directly to the user.
Users can use the wallet comes with the ability to pay (legal currency or cryptocurrency) to pay directly in the UAW,
Or can be transferred to other people to pay on behalf of, for example, the couple can negotiate the choice of payers,
Children can have their parents pay bills for their phone or credit card.

不仅如此， 电子商务网站产生的支付账单也可以被导入到钱包进入支付流程，
虽然可以想像法币的电子商务网站可能不愿意这么做，
因为通常他们已经有自己的支付通道， 例如PayPal或者Alipay。

Not only that, e-commerce sites pay bills can also be imported into the wallet into the payment process,
Although it is conceivable that the e-commerce website of the French currency may not be willing to do so,
Because usually they already have their own payment channels, such as PayPal or Alipay.

通用资产钱包，即使在没有第三方应用的上下文中，也是各人处理自己财务的一个非常强有力的工具。它不仅仅像刚才一样可以处理一些日常生活中的个人的借贷行为，同时也可以供小型企业，例如家庭旅馆或者家庭餐馆作为发送折扣卷或者代金券的一种工具。

Universal Asset Wallets, even in the absence of third-party applications, are a very powerful tool for everyone to handle their finances. Not only does it handle some of the personal lending activities of everyday life just as it is, but it can also be used by small businesses such as family hotels or family restaurants as a tool for sending discount coupons or vouchers.

![](media/image5.png){width="1.975in" height="4.277777777777778in"}

#### 6.4.  多重签名 （Multi-Sig）

UAW内置多重签名所需要的用户界面的支持。

AW built-in multi-signature required user interface support.

但一笔交易被提出并且需要多重签名，UAW 会发消息到相应的签名者的钱包，
提示制定的签名者审核交易细节， 然后作出 "同意"或者"拒绝"的动作。
UAW消息队列中会呈现需要签字的交易清单。 签字的历史也将被保留。

However, a transaction is made and requires multiple signatures, UAW will send a message to the appropriate signer's wallet,
Prompts the developer to review the transaction details and then "agree" or "reject" the action.
The UAW message queue presents the list of transactions that need to be signed. The history of the signature will also be preserved.

交易的发起可以是从另外一个UAW， 也可以是从已经加入 UDAP
生态的第三方APP。 这对第三方APP是非常方便的，
它们不需要再建设自己的多重签名的工作流，
就可以获得数字签名的强大安全性支持。

Initiation of the transaction can be from another UAW, can also be from has joined UDAP
Eco third-party APP. This is very convenient for third-party APP,
They do not need to build their own multiple-signature workflow,
You can get a strong digital signature security support.

#### 6.5.  Plugin Store

![](media/image6.png){width="2.0229166666666667in"
height="4.38125in"}

UAW是一个powerful的可扩展的插件架构，实际上它的主要目的是支撑大量的能产生各类资产的第三方App。它在UDAP为第三方App提供后台整合的功能上提供了一个统一的用户端体验的整合。这些用户端的plugin构成了用户能体验到的整个资产互联网的生态。所有的第三方应用集中地出现在UAW的Plugin Store 中， 用户已经开户的plugin和尚未使用过的plugin均在这里出现供用户快速进入。

UAW is a powerful and extensible plugin architecture, and its main purpose in fact is to support a large number of third-party apps that generate a wide range of assets. It provides a unified user experience integration with UDAP's ability to provide background integration for third-party apps. The plugin for these clients constitutes the ecology of the entire asset Internet that users can experience. All third-party applications appear in the Plugin Store of the UAW, and the plugin and unused plugin that the user has already opened account for the user to quickly enter here.

技术上UAW是一个分层的架构体系， 相当多的用户体验部分已经固化在UAW中，另外的可展示部分由第三方plugin 提供。 例如演出票务是一个plugin，个人资产管理是一个plugin，微合同是一个plugin，甚至个人所拥有的大宗商品资产是plugin。

Technically UAW is a hierarchical architecture, a considerable part of the user experience has been cured in the UAW, the other part of the display is provided by a third-party plugin. For example, the show ticket is a plugin, the personal asset management is a plugin, the micro contract is a plugin, and even an individual owned commodity asset is a plugin.

并非所有的第三方应用会提供一个UAW的plugin。 一个App可以有自己的原生的App， 或者只有基于PC 的网站。 这个在UAW的App用UDAP提供的API和整个计算链和存储链发生关联。

Not all third-party applications provide a UAW plugin. An App can have its own native app, or only a PC-based web site. This API provided by UAW's UDAP is associated with the entire compute and storage chain.

![](media/image7.png){width="6.5in" height="3.013888888888889in"}

UAW 是一个生态系统。他提供可编程的借口让第三方的应用可以开发完整的用户体验。当然UAW本身提供内置的一系列的功能能够节省大量的第三方应用推向自己的用户群所需要的时间。

UAW is an ecosystem. He provides a programmable excuse for third-party applications to develop a complete user experience. Of course, the UAW itself provides a series of built-in features that save the time it takes for a large number of third-party applications to reach their own user base.

1.  简单资产转移：用户就像发送email一样， 或者像通常的转移Crypto Currency一样吧加密资产从一个账户发送到另外一个账户。

    Simple Asset Transfers: Users are like sending emails, or as usual Crypto Currency. Encrypted assets are sent from one account to another.

2.  获得接受许可的转移： 为了防止垃圾资产充斥钱包，用户可以设置自己的账号要求发送方在获得许可的情况下才能发送资产。

    Obtain permission to transfer: In order to prevent the rubbish assets flooded wallets, users can set their own account requirements to send the sender in the case of permission to send assets.

3.  检票： 这是通用资产钱包中所自带的[交割]{.underline}工具。
    所为交割是指一些资产发行方提供的未来的服务的许诺，他们都需要在一定的时间内进行最终的产品或者服务的兑现。一个对未来的资产承诺书的兑现过程，实际上是承诺的回收的过程，我们简单称之为"检票"。一旦交割发生完毕以后。一个在"期货"形式资产就完成了它的生命周期。这样的场景，非常适用于例如演出会的门票电影票，餐馆的优惠券折扣券以及个人的债务。

    Ticketing: This is the [Deliver] {. Underline} tool that comes with the General Assets wallets.
     Deliveries refer to the promise of future services provided by asset issuers who need to deliver the final product or service within a certain period of time. A process of redemption of a future asset commitment is actually a promised process of recovery, which we will simply call a "ticket examination." Once the delivery has taken place. An asset in the "futures" form has its life cycle completed. Such scenes are ideal for tickets such as ticket tickets for shows, coupon coupons for restaurants and personal debts.

    某种票证的持有人，在进行服务的兑现的时候，点击，对线或者验票的按钮，出示给服务厅工整，服务提供者使用验票或者验证的按钮，就完成了，对这笔债务的回收，然后他可以在线下提供，这笔债务的纸面所指定的服务，或者产品。也就是说，通用资产钱包也可以拿来作为演出会的门票，或者电影院工作人员使用的验票工具。

    When a holder of a certain type of ticket clicks on a line or a check-out button to present the service, he / she presents the button for the service hall to be neat and the service provider uses the ticket or the verification, and this is done The debt is recovered, and then he can be offered offline, on the paper designated by the debt service, or product. In other words, the Universal Wallet can also be used as a ticket for a show or a ticket checking tool used by movie theater staff.

4.  售卖： UDAP自带市场工具，提供资产拥有者在市场销售资产。
    交易使用的货币可以是任意的加密货币，这是所谓的[场内交易]{.underline}。市场同时提供线上交易和线下交易混合的模式，使用escrow服务来促成使用法币购买资产的交易，这和 localbitcoins 这样的[场外交易]{.underline}模式类似。

    Sell: UDAP comes with market tools that provide asset owners to market assets in the market.The currency used for the transaction can be any cryptocurrency, which is called [OTC] {.underline}. The market offers a mix of both online and offline transactions, using the escrow service to facilitate transactions that use the French currency to buy assets, similar to the [off-market] {.underline} mode, such as localbitcoins.

5.  多重签名：检测操作的签字需求，并且自动推送签字通知到相应签字人的钱包消息队列。

    ultiple Signatures: Detects signature requirements for operations and automatically sends sign-off notifications to the wallet message queue of the appropriate signatory.

UAW为第三方的应用使用系统提供的标准plugin 的JavaScript API，
主要函数如下（都在操作都在App沙盒上下文中）：

UAW uses the standard plugin's JavaScript APIs for third-party applications,
The main functions are as follows (both in action in the sandbox context):

1.  getCurrentUser: 获得当前用户的身份信息， 包括链上地址。Get the current user's identity information, including the chain address.

2.  getAssetCollection: 获得当前用户的资产列表。Get the current user's list of assets.

3.  initTransfer：转移特定资产。激发UAW的多重签名机制，如果资产转移需要多重签名的话。Transfer specific assets. Stimulate UAW's multi-signature mechanism if asset transfer requires multiple signatures.

4.  offerToSellInMarket：在market中挂价销售，指定货币类型。Sale in the market price, the designated currency type.

5.  offerToSellInExchange: 在exchange 中挂价销售。In exchange for sale price.


用户的购买行为统一发生在UAW中。 一个用户在某个 App plugin中发现想购买的资产，点击详情后统一进入UAW提供的详情页面并且下单购买。

The user's purchase behavior occurs uniformly in the UAW. A user found in an App plugin want to buy the assets, click on the details unified into the details page provided by UAW and place an order to buy.

更多的API将分批提供， 包括各种auction方式，escrow 方式的P2P交易。

More API will be provided in batches, including various auction methods, escrow P2P transactions.

## 7.  实现

在UDAP中, address分为account address, asset address和assetProto address。其中account代表现实中的用户, 组织, 服务方等的账户. Asset是代表一个资产. AssetProto是代表一类资产的原型. 一个资产必须和一个资产原型做一一对应的关联.

In UDAP, address is divided into account address, asset address, and assetProto address. Where account represents the actual account of the user, organization, service provider, etc. Asset represents an asset, AssetProto is a prototype of a type of asset, and an asset must be associated with an asset prototype in a one-to-one correspondence.

这3类address都具有具有一个versionHash和lastCommitTimestamp属性. versionHash代表这一个地址的改动状态,
一个地址的每一次改动都将产生一个新的随机且永不重复versionHash值. lastCommitTimestamp则记录一个地址最后一次接到交易处理后完成的时间点.

These three types of address have a versionHash and lastCommitTimestamp property. VersionHash represents the changing status of this address,
Each change of an address will generate a new random and never duplicate versionHash value.lastCommitTimestamp will record the last point in time when an address was received after the transaction was processed.

UDAP的交易总是关联着规则(rule). 规则是寻求一系列满足给定address的数字签名的逻辑. UDAP的各种操作都有着权限管控, 权限的管控就是由规则来实现的. 在UDAP中,需要对地址进行一系列的操作, 等同与对地址发起一系列的交易.
一个交易, 通常包括以下数据

UDAP transactions are always related to rules (rules) is to find a series of logic to meet the given address of the digital signature UDAP various operations have permission control, permission control is achieved by the rules in the UDAP , Need to address a series of operations, equivalent to the address and initiate a series of transactions.
A transaction usually includes the following data

-   交易的发起者The originator of the transaction

-   交易的接受者Recipient of the transaction

-   交易的方法The method of trading

-   交易方法的参数Trading method parameters

-   满足条件的数字签名Meet the conditions of digital signatures

-   可选的交易接受者的versionHash.Optional transaction acceptor versionHash.

其中交易的发起者必须是account address, 交易的接受者可以是asset address或者assetProto address. 数字签名的签名人通常情况下是account address, 但也可是是自己设置的地址. 数字签名是针对包括交易的发起者, 交易的接受者, 交易的方法, 交易方法的参数, 签名时间, 签名有效期和可选的交易接受者的versionHash在内但不限于其中的摘要的签名.

The originator of the transaction must be an account address, and the recipient of the transaction can be an asset address or an assetProto address. The digitally signed signer is usually an account address, but it is also an address that you set yourself. The initiator of the transaction, the recipient of the transaction, the method of the transaction, the parameters of the transaction method, the signature time, the validity period of the signature, and the versionHash of the optional transaction recipient but not limited to the signature of the digest therein.

当UDAP接受到交易时, 规则匹配器会校验签名是否是对该交易请求的签名, 签名是否过期, 签名时间是否晚于交易接受者的lastCommitTimestamp, 若给出versionHash则交易接受者的versionHash是否满足给出条件,所有合法签名的签名人能否满足规则等等. 如果满足, 则接受这次交易请求, 完成操作, 交易接受者的lastCommitTimestamp改为该次交易结束的时间, 并且产生新的versionHash. 如果不满足, 则驳回.

When the UDAP accepts the transaction, the rule matcher verifies whether the signature is a signature of the transaction request, whether the signature is out of date, whether the signature time is later than the lastCommitTimestamp of the transaction acceptor, and if the versionHash of the transaction acceptor is given if the versionHash is given Given conditions, all legitimate signatory signers can meet the rules, etc. If so, then accept the transaction request to complete the operation, the lastCommitTimestamp of the transaction recipient to the end of the transaction, and generate a new versionHash. If not, then rejected.

例如, 某个资产的所有者O需要将该资产抵押给A, 抵押资产这种操作的权限对应的规则是需要B, C, D这3个人物中至少2个人的签名.发起这个请求的是app应用. App将这个请求交易的发起者, 接受者, 以及所有方法参数设置完毕, 然后将这段数据求情的发送给B, C, D三人展示意图并请求审批. 其中交易的发起者为O, 交易的接受者为资产A, 方法是抵押, 参数依照方法而定. B, C, D三人审阅后决定是否就批准该交易请求的摘要进行数字签名.

For example, the owner O of an asset needs to mortgage the asset to A. The rule corresponding to the right of the mortgage asset operation is to sign the signature of at least two of the three characters B, C and D. The request App App App will be the initiator of the transaction, the recipient, and all the method parameters are set, and then this data is forbidden to send to the B, C, D three intents and requests for approval.The transaction was initiated by O, the recipient of the transaction is the asset A, the method is mortgage, and the parameters are determined according to the method B, C, D After review, the trio decides whether to sign the digest that approves the transaction request.

签名里包括了签名的时间, 签名的有效期, 以及可能包含当前资产的versionHash. 当App收集齐足够的签名后,就向UDAP发起交易, UDAP通过解读方法参数, 验证列出的签名是否满足规则. 若满足, 改变资产的状态, 将资产抵押出去, 同时生成新的versionHash,所有签名时间里最晚的时间记录为新的lastCommitTimestamp. 因为签名是针对交易方法参数,可选的versionHash, 又有lastCommitTimestamp在时间上保证, 故签名一次使用就作废, 为Replay Attack做出了充分的保证. versionHash在交易请求和数字签名内是可选的, 它的设计是为了保证资产数据不会被幻影读, 是一种类似的乐观锁. 是否需要验证versionHash的主动权掌握在交易的发起方, 并需要批准人的认可.

The signature includes the time of signature, the signature's validity period, and the versionHash that may contain the current asset.When the app collects enough signatures, it initiates the transaction to the UDAP, which UDAP verifies if the listed signature satisfies the rule by interpreting the method parameters. If satisfied, change the state of the asset, mortgage out the asset, generate a new versionHash, and record the latest lastCommitTimestamp in all signatures as the signature is for the transaction method parameters, optional versionHash, and lastCommitTimestamp Time guarantee, so the signature of a use of obsolete, Replay Attack made full guarantee. VersionHash transaction request and digital signature is optional, it is designed to ensure that the asset data will not be phantom read, is a Similar optimistic locking. Whether you need to verify that versionHash is in the hands of the originator of the transaction and requires approval from the approver.

我们的使用者要注意的是，作为我们的概念网络，我们第一期的产品推出的时候，将以Ethereum作为基础的依托架构， 集合Tendermint 作为consensus机制。虽然我们的计划建设一个体现以太网或者比特币关键属性的一个崭新的资产网络，这个属于中期的目标。在我们第一期推出给用户使用的环境中，我们的运行环境将主要依赖于现有的以太网环境所能给我们提供的能力，取决于和以太网的智能合约环境相兼容的一些其他技术的发展和成熟的速度，我们也不排除我们第一期的目标考虑使用和以太坊兼容，或者相似的其他的平台技术。

Our users should note that as part of our conceptual network, the first phase of our product launch will be based on Ethereum's reliance on the architecture, bringing together Tendermint as the consensus mechanism. Although our plan to build a brand new asset network that reflects the key attributes of Ethernet or bitcoin is a mid-term goal. In our first-of-its-kind environment for our users, our operating environment will depend primarily on the capabilities our existing Ethernet environment can deliver to us, depending on a few other technologies that are compatible with Ethernet's smart contract environment We also do not rule out the goals of our first phase to consider using other platform technologies that are compatible with Ethereum, or similar.

## 8.  和类似平台比较分析
With similar platforms for comparative analysis

|       | UDAP  | BankEx | Bytom | Digix | 0x    | Achain | Selfsell | Linkeye |
|-------|-------|-------|-------|-------|-------|-------|-------|-------|
| 简介Introduction  | 一个专精于实现广义资产管理的区块链A blockchain that specializes in generalized asset management | 银行资产管理服务区块链Bank Asset Management Services Blockchain | 包含资产业务逻辑的重量级资产链Heavyweight asset chain with asset business logic | 只做黄金资产管理平台Only gold asset management platform | 基于ERC20的资产交易协议ERC20-based asset trading agreement | 和以太坊类相似的图灵完整区块链Similar to the Ethereum Turing complete blockchain | 针对个人能力投资的区块链，基于AChainBlockchain for Individual Capacity Investment, based on AChain | 针对征信业的区块链应用Blockchain application for credit information industry |
| 支持智能合约Support smart contracts |  | ？  | Yes  | Yes  | Yes  | Yes | Yes| Yes |
| 能否接受通用型资产Can accept generic assets | Yes |    | Yes   |       | ERC20 | Yes   |       |       |
| 支持分布式文件存储Support for distributed file storage | Yes | ？ |       | Yes   | N.A.  |       |       |       |
| 链属性Chain attributes | 联盟链Alliance chain | ？  | 公有Public  | 公有Public  | 公有Public  | 公有Public  | 公有Public  | 公有Public  |
| 共识consensus  | PoS   | 特有Unique  | PoW   | 特有Unique  | PoA/PoS | DPoS  | DPoS  | DPoS  |
| 固化常见抽象方法Curing the common abstract method | Yes | Yes |      |       | N.A.  |       |       |      |
| 第三方提交代码Third-party submission code |  | Yes   | Yes   | Yes   | Yes   | Yes   | Yes   | Yes   |
| 原生Multisig Native Multisig | Yes |       |       |       |       |       |       |       |
| 资产存在形态The existence of assets | 地址address | ？ | UTXO | 合约内token Contract within the token | 合约内token Contract within the token | 合约内token Contract within the token | 合约内token Contract within the token | 合约内token Contract within the token |
| 双花保证Double flower guarantee | 资产地址nonce Asset address nonce | ？ | UTXO特性 UTXO features | 地址nonce Address nonce | 地址nonce Address nonce | 地址nonce Address nonce | 地址nonce Address nonce | 地址nonce Address nonce |



## 9.  应用案例分析

<!-- -->

1.  各类演出、实况表演、体育活动、线下的各种聚会的票务管理。
    一个第三方的专注于各种票务发行流转服务提供等完整的票务，全生命周期的第三方应用平台。经常会发生这样的情况，持有演唱会票的观众可能因为什么原因不能出席演出，他需要能够以最能体现票面价值的方式把票转移给他人，反方向来说，另外一类人在他们看到某个演唱会的时候，可能已经错过了演唱会门票发售的时间，他们没有一个合理便捷的方式能够获得这个活动的门票，就是说这一类资产缺乏一个便捷的二级市场。演出市场相对而言还算一个较好的市场，因为私下里，我们称之为黄牛的人扮演了一个流动性的角色，虽然不是通过一个正规的渠道，但是他们的确起到了通过流通性来确认特定的活动的价值和满足供需对接的目的，他们从中获得了中间的差价。

    Various performances, live shows, sporting events, ticket management for various gatherings under the line. A third-party third-party application platform that focuses on the complete ticketing and full lifecycle offering of various ticketing distribution and streaming services. It is often the case that viewers who hold concert tickets may not be able to attend the show for whatever reason, and that they need to be able to transfer the votes to others in the best way possible, in the opposite direction, When you see a concert, you may have missed the time of the concert tickets, they do not have a reasonable and convenient way to get tickets for the event, that is, this type of asset lacks a convenient secondary market. The performance market is still a relatively good market, because in private, the people we call the ox play a liquidity role, though not through a formal channel, but they did indeed confirm through the liquidity The value of the specific activity and the purpose of meeting the supply and demand, they get the middle of the difference.

    可以利用我们提供的API为他们每一次活动数字化和加密资产化或者代币化后的，各种票券可以在朋友之间赠送、转让，也可以放到资产钱包所提供的标准的资产市场，进行二级市场的交易。在加密化资产的交易流通过程中，资产的原始发行方可以控制资产交易的频率，流动性，以及在资产交易中价格的浮动范围。他们还可以控制每一个资产是否允许进行转手、转让等刺激市场的交易。这为票务管理的app提供了极为方便的特性，同时有一般的票务系统中不可比拟的安全性和流动性。我们的数字资产钱包，甚至包括了灵巧的资产转移的功能，完全可以直接用来完成演出演唱会，电影票等票务所需要的现场验票和交割环节的基本手续。因为我们的资产钱包把这一类资产所需要的交割，或者称之为已资产支付进行了抽象化。这样第三方应用叫至需要进行数字资产的铸造代币化。并且对这些资产的二级市场流通性进行配置，以后的后续工作都可以被消费者试用数字资产钱包。

    After we digitize and encrypt each of their events using our API for asset or tokenization, various tickets can be donated, transferred between friends, or put in the standard asset market provided by the wallet, Conduct secondary market transactions. During the transaction flow of encrypted assets, the original issuer of the asset can control the frequency of asset transactions, liquidity, and the range of price fluctuations in asset transactions. They can also control whether each asset is allowed to be resold, transferred, etc. to stimulate market transactions. This provides an extremely handy feature for ticket management apps with the unparalleled security and fluidity of a typical ticketing system. Our digital asset wallets, even including the smart asset transfer function, can be used directly to complete the basic procedure of on-site ticket inspection and delivery of tickets for concerts, movie tickets and other ticketing needs. Because our asset wallets abstracted from the delivery of what is required for this type of asset, or what is called asset payout. This third-party application is called tokens for casting that requires digital assets. And the secondary market liquidity of these assets to configure, follow-up work can be consumer trial digital asset wallets.

2.  个人形象，品牌代币（或者叫个人品牌"上市"）。
    在加密数字资产世界中，人们逐渐意识到，代币是一个崭新的经济模式。代币的核心其实就是把现实世界中形形色色的各类可触及的以及不可触及的资产进行数字化，并且纳入到了严格的计算机密码学和区块链技术的约束范畴。这些资产对应的代币，可以充分利用区块链以及围绕区块链的交易所所提供的巨大的流动性，形成一个崭新的代币经济。这其中一个非常有创新性的构思，就是出现了一种新的可能，让每一个人都能够发行代表自己的声誉和形象的代币。我们设想在未来的世界中，每一个人都可以发行自己的数字货币，以自己个人的形象和声誉、信誉，为自己的代币承诺。个人的代币可以代表了个人对世界及周边其他相关人群的某种信用和承诺。同时因为代币带来的流动性，能够比较准确的两个人的价值得到准确的体现。由此避免了个人自我价值确认过程中发生的自我估值过高，所带来的有价无市或者是自我估值偏低，形成的对自己的实质上的损失。有了我们平台的支持，个人非常容易的能够创建自己的粉丝俱乐部或者会员俱乐部，能够控制其所发行的会员证的数量以及流通的方式，能够为社会提供服务的个人，你把自己的服务包装成个人代币的形式，投放到市场中。并且，随着市场对个人服务需求的变化，浮动的定价。这种场景，对于服务提供方的充分就业和服务需求方的充分满足来说，都提供了一个前所未有的可能性。

    Personal image, brand tokens (or personal brand "listing").In the world of encrypted digital assets, people are gradually realizing that tokens are a brand new economic model. The essence of tokens is actually to digitize all kinds of accessible and inaccessible assets of all kinds in the real world and to include the strict constraints of computer cryptography and blockchain technology. The tokens corresponding to these assets can make full use of the huge liquidity provided by the blockchain and the exchanges around the blockchain to form a brand new tokens economy. One of these very innovative ideas is the emergence of a new possibility for everyone to issue tokens that represent their reputation and image. We envision that in the future world, everyone will be able to issue their own digital currency, with their own personal image and reputation, credibility, promises for their token. Personal tokens represent some kind of credit and commitment individuals make to the world and other related people in the neighborhood. At the same time because of the mobility of tokens, two people can be more accurate value accurately reflected. This avoids the self-worth of individuals in the process of confirmation of self-valuation is too high, resulting in a priceless market or self-valuation is low, the formation of their own substantive losses. With the support of our platform, individuals can easily create their own fan clubs or clubs, have the ability to control the number of membership cards they issue and the means of distribution, individuals who can serve the community, and you package your services Into the form of personal tokens, put on the market. And, as the marketplace demands for personal services change, floating pricing. This scenario offers an unprecedented possibility of full employment of service providers and full satisfaction of service demand side.

3.  供应链金融。典型的供应链，b2b的商业模式中存在着大量的大宗商品仓储，转运，销售，治一治呀。等等常见的业务流程。本平台提供的API将使得供应链上下游的资产确认、公正、交易、传于、和交割真正的非常容易。尤其是，我们平台提供的有包含关系的资产管理工具和方便的多签名机制和工作流支持，能够对b2b资产的流动服务提供极为便捷的、安全的、高效率的支撑。并列的上下游以及参与到共赢流转的资金方，例如银行是资金借贷方，我可以把自己的资产形成加密数字化以后，在上面方便的进行交易。

supply chain finance. Typical supply chain, b2b business model there is a lot of bulk warehousing, transportation, sales, cure it. Etc. Common business processes. The APIs provided by this platform will make it easy to identify, justify, trade, deliver, and deliver assets upstream and downstream of the supply chain. In particular, our platform includes relational asset management tools and easy multi-signature mechanisms and workflow support that provide extremely convenient, secure and efficient support for mobile services for b2b assets. Side by side with the upstream and downstream and participate in win-win flow of funds, for example, the bank is the lender of funds, I can encrypt their own assets after the formation of digital, convenient to carry out the above transactions.

4.  零售行业。零售行业中，经常使用的各种现金券，打折券，会员优惠凭证，促销手段均可数字化和加密货币化以后，形成更方便的，刺激流通的资产。通过平台的交易和提供的中间货币，虚拟货币的调节作用，消费者甚至可以在不同的服务提供商之间实现积分的兑换和服务的置换。

    Retail industry. In the retail industry, frequently used cash vouchers, discount coupons, membership vouchers and promotional tools can be digitized and encrypted for monetization to create a more convenient and stimulating circulation asset. Through the platform of trading and the provision of intermediate currency, the role of virtual currency regulation, consumers can even achieve integration between different service providers exchange and replacement of services.

5.  旅馆行业。旅馆的房间是一个非常适合于数字加密资产化的一个应用场景。因为旅馆房间的价格的波动性随着节假日和季节，天气等因素的变化非常平凡。由于流动性不足，旅馆的房间经常没有得到充分的销售。从消费者的角度看。在突发的时间经常订不到旅馆的房间，也是一个经常面临的生活障碍。通过本平台，我们可以构建一个崭新的旅馆订阅平台。通过二级市场提供大量的流动性，使得旅馆房间的销售和消费者对于旅馆房间的需求都得到充分的准确的定价和满足。

    Hotel industry. The hotel room is a very suitable application for digital asset encryption. Because the hotel room price volatility with the holidays and the seasons, weather and other factors change is very ordinary. Due to lack of liquidity, hotel rooms are often not fully sold. From the consumer's point of view. In unexpected times often can not set the hotel room, but also a living often face obstacles. Through this platform, we can build a brand new hotel subscription platform. Through the secondary market to provide a lot of liquidity, making the hotel room sales and consumer demand for hotel rooms have been fully accurate pricing and satisfaction.

6.  数字游戏中的虚拟资产交易。市面上流行的各种电子竞技游戏中的数字资产有一个灰色的市场，供玩家们进行道具人物的转让，游戏的发行商也许不愿意让玩家们能够自由的进行武器道具的交易，这样总能保证需要新武器和额外设备的玩家总是从游戏设计者的商店中购买。但是也有不少的游戏意识到，提供一个标准化的游戏道具的交易市场，是提高用户体验，获得更多用户的一种手段。我们的资产服务平台，能够提供标准化的API，够第三方游戏开发者登记他们所发行的数字资产的类型，管理这些类型在交易中的交易规则。同时，资产交易的生态符合游戏设计者所期待的动态模型。

    Virtual game in digital games. There is a gray market for digital assets in all kinds of e-sports games that are popular in the market, for players to transfer the characters of the props. The publisher of the game may be reluctant to allow the players to freely trade the weapon props, so that the total energy Players who promise new weapons and extras are always purchased from the game designer's store. However, there are quite a few games that realize that providing a standardized marketplace for game props is a way to enhance the user experience and get more users. Our asset services platform offers a standardized API that enables third-party game developers to register the types of digital assets they issue and manage the trading rules for those types in the transaction. At the same time, the ecology of asset trading conforms to the dynamic model expected by game designers.

7.  古董字画艺术品资产管理交易。艺术品的现货交易是我们资产管理网络的一个非常有前景的应用。我们的平台不仅仅提供基本的计算功能，同时还提供了艺术品收藏信息保存所需要的文件存储和多媒体存储能力，所以在艺术品流通中所需要的数字化、加密化和代币化的各种手段，都可以被用来直接对艺术品交易周期进行直接的管理。古董字画以及工艺和其他类的艺术品交易，过去存在着两种主流的交易方式：一种是文物艺术品商店直接向个人收购，或者滥授他们的作品，然后提供给消费者选购；另外一种交易模式发生于民间，自由市场的模型，艺术品的拥有者和艺术品的潜在买主直接进行交易和销售；艺术品还有一个常见的销售模型是拍卖模式，因为艺术品是一个流动性不足的产品，对于艺术品的定价有着巨大的分歧，而且有着巨大的灰色空间，有时候艺术品还被用于从事洗钱和非正当的经营活动，区块链技术将有助于把这些交流程中的欺诈行为去除掉，并且在满足非常灵活的交易模型的前提下，保证艺术品交易中最重要的数源保真担保。

    Antique Crafts Art Asset Management Trading. Spot trading of artwork is a very promising application of our asset management network. Our platform not only provides basic computing functions, but also provides the file storage and multimedia storage capabilities required for the preservation of art collection information. Therefore, all kinds of digitization, encryption and tokenization required in the circulation of artwork Means can be used to directly manage the art trade cycle directly. There are two main types of transactions that existed in the past: antique art shops, direct acquisitions from individuals or overprofessionals, which were then offered to consumers for purchase. In addition, A trading model takes place in the private, free-market model where art owners and potential buyers of artwork trade and sell directly; a common selling model for art is the auction model because artwork is a liquidity Insufficient products have huge disagreements about the pricing of artwork, and have huge gray spaces, sometimes used for money laundering and improper business activities, and blockchain technology will help put these exchanges In the fraud to get rid of, and to meet the very flexible transaction model under the premise of ensuring the art auction the most important source fidelity guarantee.

8.  ICO。 平台支持公司通过把公司的权益或者产品使用的权利代币化，
    并且立即通过平台提供的交易能力获得流动性。

    Platform Support Companies through the company's rights or the right to use the product tokenization, And immediately get liquidity through the trading capabilities provided by the platform.

<!-- -->

10. 总结summary

资本是经济的发动机， 无论对于商业实体和个人而言皆是如此。
资产的资本化是从经济中获利的主要途径。

Capital is the engine of economics, both for business entities and individuals.
Capitalization of assets is the main way to profit from the economy.

我们在这里所倡导的"通用资产"资产的本性是存留和价值实现。

The nature of the "general assets" asset we are advocating here is the survival and the realization of the value.

区块链通过不可篡改的特性来支撑资产信息的永久存留。某种意义上也就是资产的永久存留。

Blockchain supports permanent retention of asset information through tamper-evident features. In a sense, it is the permanent existence of assets.

同时区块链衍生的代币经济以及作为代币经济核心的流动性为资产提供了价值确认的关键性渠道。

At the same time, the blockchain-derived tokens economy and the liquidity as the core of the tokens economy provide the key channel for the value recognition of assets.

资产的流动性对于整个行业的健康而言，是一个类似于人体的血液循环系统的通畅性和人体健康的关系的相等、重要的地位。整个经济学中所研究的大部分的内容其实都是研究如何提高一个局部系统的流动性，虽然有部分经济学家过分地夸大了流动性的重要性和流动性的神奇的功能，以至于被冠以流动性幻觉，但是仔细考察我们身边的各种行业，流动性的不足，几乎始终是所有的行业都面临的持续挑战，即使我们已经满足于某种体系提供的流动性，单如果考虑到更高的层面和未来，可能这种流动性又变得非常不足。所以我们认为。在现有的现实情况下，把流动性增加是无论如何也不能过分的表达其重要性的。


The liquidity of assets is an equal and important position for the health of the entire industry, similar to the patency of the human circulatory system and human health. Much of what is studied in economics as a whole is actually about how to improve the liquidity of a local system. Although some economists overstate the importance of liquidity and the magical function of liquidity, Is a hallucination of liquidity, but a closer examination of the various industries around us, the lack of liquidity, is almost always a continuing challenge for all industries, even if we are already content with the liquidity provided by a system that, if taken into account At a higher level and in the future, this liquidity may become very inadequate again. So we think. In the current realities, increasing the liquidity can not overemphasize its importance anyway.

流动性并不是一个万能的良药。其实，流动性本身有可能会带来系统的不稳定和伤害，就像人体的血液循环系统一样，顺畅的血液流通并不代表无所节制的血液流通。所以整个市场的流动性的控制和优化，实际上是一个行业面临的第二个挑战。

Liquidity is not a panacea. In fact, liquidity itself may bring system instability and harm, just as the body's blood circulation system, smooth blood circulation does not mean that there is no control of blood circulation. So controlling and optimizing liquidity throughout the market is actually the second challenge for an industry.

许多行业的圈子内部有一个很大的课题。要让资产的拥有者，或者资产流动方能够对资产的流通有所控制，这是资产拥有者或者大批资产的登记和发布者所面临的课题。过去是没有好的手段来解决这些问题，技术或者是公开的去中心化记账技术的出现，使得这些需求第一次有可能得到满足。

Many industries have a big problem within the circle. Enabling asset owners, or asset flowrs, to control the flow of assets is a challenge for registrants and publishers of asset owners or large numbers of assets. In the past there was no good solution to these problems, and the advent of technology or open decentralized accounting techniques made these needs likely to be met for the first time.

本篇白皮书所描述的正在进行的项目，就是通过以下几个方面，对我们所认识的真正的我们称之为价值或者资产的互联网，作出我们独特角度的贡献，这些角度包括：

Ongoing projects described in this paper are our unique perspectives on what we know about the true Internet we call value or assets, from the following perspectives:

1.  现实世界的资产，如何能够非常方便的，在不需要知道区块链技术的情况下，在任何第三方的应用通过调用标准化的协议而得到定义登记和确认。我们提供的方案是建立一个把区块链以及分布式存储技术隐藏在后面的、简单的统一的API，供第三方程序调用。第三方的商业应用程序，可以在不需要知道区块链技术和分布式文件存储技术以及分布式计算技术的前提下，就像使用传统的客户服务器或者云技术一样使用我们的API，但是却获得试用去中心化的计算和存储所带来的所有的价值。

    Real-world assets, how it can be very convenient, without the need to know the blockchain technology in any third-party applications by calling a standardized protocol to get the definition of registration and confirmation. The solution we provide is to build a simple, unified API that hides the blockchain as well as distributed storage technologies for later use by third-party programs. Third-party business applications that use our APIs the same way as traditional client-server or cloud technologies without the knowledge of blockchain technology and distributed file storage technology and distributed computing technology, Try to centralize all the value that comes with computing and storage.

2.  我们的API把区块链、分布技术和第三方应用隔离，原因之一是，我们将提供对区块链写入确认以及各种非常昂贵操作的缓冲，使得用户的性能和简洁性有较大幅度的提升。同时，用户用于资产全周期管理的API完全可以超过现在的以太坊，这样技术智能合同提供的数据类型和有时候令人迷惑和烦恼的、不成熟性都隐藏在后面。可是登录的时候，用户在不需要自己进行更新的情况下，我们的后盾可以切换到更为先进的、随时都在发生着剧烈性能提升和架构提升的区块链或者类似区块链的去中心化的公开记账本。

    One of the reasons that our APIs segregate blockchain, distribution technology and third-party applications is that we will provide a buffer for blockchain writes validation and various very expensive operations that will make the user's performance and simplicity even greater Amplitude increase. At the same time, users' APIs for asset lifecycle management can outweigh current Ethereum so that the data types provided by technology smart contracts and the sometimes confusing and annoying, immature ones are hidden behind. However, when you log in, our users can switch to the more advanced blockchain or similar blockchain that is undergoing dramatic performance improvement and architecture upgrade at any time without the need to update itself. The public bookkeeping.

3.  我们的API服务器把区块链的安全模型也转换成常见的app开发中的安全模式。

Our API server also translates the blockchain's security model into a common security model for app development.

4.  作为我们中期的工作之一，我们正在建设一个原生支持公用资产互联模式的，新的分布式或者去中心化的记账和计算系统。现有的类似于以太坊这样的智能合同的模式，我们认为对编程者而言，提供了过大的随意性和暴露了大量的可被攻击的表面面积。这就导致，对于资产管理而言，产生了一个最为关心的安全性的重要隐患。我们正在设计的原生支持资产的新的网络，将我们认为资产管理的必要的功能环节完全固化在网络本身的协议之中，而不需要用户用自己书写的代码来维护各种资产。这可能在性能和安全上，都会出现一个新的飞跃。

     As part of our mid-term effort, we are building a new distributed or decentralized accounting and computing system that natively supports the public asset-networking paradigm. Existing patterns of smart contracts like Ethereum, we think, provide too much randomness to programmers and expose a lot of surface area that can be attacked. This has led to an important hidden danger to asset management that is of the utmost concern for safety. The new network of native support assets we are designing allows us to fully cure the necessary functional aspects of asset management in the network's own protocol without the need for users to maintain the assets in their own written code. This may be a new leap in performance and safety.

5.  API网关将把通用型的资产生命周期管理所需要的所有的API都包括在内。这种抽象，使得用户不需要通过人工的方式，就能像使用标准化数据库一样，使用基于区块链的服务。这是对现有的区块链作为一种服务的升级，我们称之为自动化的资产管理，作为一种服务，这种模式有别于当前世界上另外一些团队所出的资产管理模型，其中包括了大量的人工审核和客户化的成分，我们的API就因为其管理的抽象性和完备性，而不需要人工的介入，使得几乎我们所知道的现实世界中处理各种形形色色资产的app，都可以像使用标准化服务一样使用我们提供的接口。

    The API Gateway will include all the APIs required for a generic asset lifecycle management. This abstraction allows users to use blockchain-based services the same way they would with a standardized database, without manual means. This is an upgrade to the existing blockchain as a service that we call automated asset management as a service that is different from the asset management models that are currently available in other teams around the world, Including a lot of manual review and customization components, our API because of its management abstraction and completeness, without the need for human intervention, making almost all we know in the real world to deal with all kinds of assets app, Can use the same interface we provide as standard services.

6.  Universal Asset
    Wallet。我们将创建一个我们新的资产统一接口标准。通过这个标准，我们将提供一个资产钱包。这个钱包包含了像数字货币一样的加密资产，同时可以包含符合我们定义的资产生命周期，API的各类用户自定义的加密资产。在这个钱包中，用户可以浏览使用我们的标准服务的各种API所能创建和维护的形形色色的各类加密化资产，能够通过我们的资产钱包，在不同的用户之间进行转账、转移、赠送，并且我们的钱包将支持签名和安全机制，能够把你见的牵涉到多签名的资产转移过程，内置在资产钱包中。这样第三方应用基本上就不需要再开发专门的钱包，他们的用户可以通过他们各个第三方应用的app，获得数字资产以后，直接在我们通用的资产钱包中浏览、转移甚至是交易。钱包还允许用户动态的自定义个人虚拟化资产，并且在个人之间进行转移。可以理解为，个人用户之间的应用资产的非常简便的流通平台。资产钱包同时将提供和本地化相关的直接支持国家货币的购买和交易。由于本平台所销售的资产都是现实世界中的可理解的资产，而不是在各国的政策中可能引起较大敏感度的虚拟货币资产，将能方便地接入本地化的法币支付通道，供消费者直接通过法币购买app开发商提供的满足本平台协议的数字资产的需求。

     Wallet.We will create a new unified standard for our assets. Through this standard, we will provide an asset wallets. This wallet contains cryptocurrency like digital currency and can contain a variety of user-defined, encrypted assets that fit our defined asset life cycle, API. In this wallet, users can browse a wide variety of encrypted assets created and maintained by APIs that use our standard services and can transfer, transfer, and donate between different users through our wallet , And our wallet will support signatures and security mechanisms that can embed the asset transfer process you see involving multiple signatures into an asset wallet. Such third-party applications basically do not need to develop a special wallet, their users can access their digital assets through their various third-party app, browse, transfer or even trade directly in our common asset wallet. Wallets also allow users to dynamically customize individual virtualized assets and transfer between individuals. Can be understood as a very simple platform for the circulation of assets between individual users. Asset wallets will also provide direct support for the purchase and trading of national currencies in relation to localization. As the assets sold in this platform are all understandable assets in the real world, and not virtual currency assets that may cause greater sensitivity in national policies, they will have easy access to localized legal currency payment channels for Consumers purchase the digital assets that app developers provide to meet the Platform Agreement directly through the French currency.

7.  我们所设计的资产网络，支撑其他所有的协议和平台所部支撑的层次化的资产复杂关系。在现实世界中，资产之间经常出现较为复杂的关系，现实世界的资产不是一个平面化的、相互之间完全独立对等的关系，我们把现实世界的资产模型化为一种树状的包含关系，我们的资产协议将原生的支持多层级的资产关系。这样在资产的转移中。可以用非常简单的API就能完成较为复杂的资产交易流程。

    The asset network we designed supports all the layers of complex relationships between assets that all other protocols and platforms support. In the real world, assets often appear more complex relationships, the real world assets is not a flat, completely independent and reciprocal relationship between each other, we model the real-world assets into a tree-like contains Relationship, our asset agreement will natively support multi-tiered asset relationships. This is the transfer of assets. You can use a very simple API to complete the more complex asset transaction process.

8.  分布式交易系统（DEX）。 应用产生加密资产后立即面临的需求是流动性。
    我们的通用资产钱包将内置资产交易能力，
    这种能力不局限在同一种性质的资产之间，
    而且支持各类资产和通用加密资产的交易， 例如和BTC， ETH
    等加密货币资产的交易。

     Distributed Transaction System (DEX). The immediate need for an application to generate encrypted assets is liquidity.Our General Assets Wallets will have built-in asset trading capabilities,This ability is not limited to the same nature of the assets, It also supports the trading of various assets and general-purpose cryptographic assets such as BTC and ETH Encryption of monetary assets such as transactions.

最终UDAP将运行一个专注于全球资产的专门化分布式计算和存储的网络，
这个网络和比特币网络， 以太坊网络等等区块链网络并存，
并且有可能通过跨链技术实现网络之间的资产的流动。

Ultimately UDAP will run a network of specialized distributed computing and storage focused on global assets,
This network and bitcoin network, Ethereum network, etc. blockchain network co-exist,
And it is possible to cross-link the flow of assets between networks.

我们相信这个一个具有高度针对性的网络对于大量的能沉淀各类资产的应用领域提供前所未有的新技术平台。


We believe this highly targeted network offers an unprecedented new technology platform for a large number of applications that can precipitate a wide range of assets.