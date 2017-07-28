Blockpass is a block chain based passbook application that serves the need of every millennial to have all his financial details ready for access in a simple, intuitive yet secure way.

The new age millennial spends more every month than what the average person used to make in a year. This has led to the rise of financial applications like Acorn, Moneyview, Walnut etc. to help manage finances. But the problem with these applications is that they are offered by third parties whose best interests may or may not be aligned with that of their users. Apart from financial management applications, there are also in-house application offered by banks which while might be secure lack any sense of UI perspective or intuitiveness.

The way we at Blockpass see it, there are three major problems plaguing the banking industry.

Extreme reliance on third party applications to help manage your day to day, weekly and monthly finances that might compromise on security or allow sale of anonymized user data.+

In house banking applications that cannot compete with the third-party applications in terms of user friendliness and sheer functionality.

The rising threat of cyber attacks : As computers become faster and more advanced, despite having the most sophisticated security protocols at our disposal, we become more vulnerable.

The solution to this lies in the most elegant decentralized data structure that has been invented : The blockchain.

The blockchain is a decentralized ledger that lets people send and keep track of a either a single type of asset or any type of asset depending on the design. The blockchain is the most sophisticated cloud based peer to peer ledger there is.

Blockpass plans to use the blockchain to solve a problem faced by the newest generation, namely by offering them the highest level of security possible while keeping the user transactions simple and hassle free. Every transaction that is performed is recorded, authenticated by the user’s peers and then added to the blockchain as seen in the flowchart in figure 1.

The blockchain, i.e. the backend attempts to get all the user information necessary to perform a transaction, namely the account number, the amount of money being sent etc as the headers to perform the transaction. Once the account details are obtained by the web application, it performs a quick block height calculation. It connects all the trailing blocks, downloads them and attempts to write the transaction to the downloaded block set. If the newly modified block chain is better than the old chain, then the new chain is written to the db and the transaction is committed.

Once a transaction is committed onto the blockchain, it can neither be modified nor deleted without having to perform an enormous amount of calculations. Thus, ensuring that the blockchain cannot have its integrity compromised.

Figure 2, gives a high level overview of the entire application. The web application allows the General User, The admin, the bank staff etc access to the blockchain. The business logic is encapsulated as rest services using spring boot to allow access to basic CRUD Operations to external databases and the blockchain by means of creating smart contracts. Web3.js is a mixture of Angular 2, HTML 5, CSS 3 and Bootstrap 4 that allows the creation of a completely customizable and unique stream lined user experience that encourages users to return to the application on a regular basis. In the beginning we plan to have 5 screens with the following capabilities :

The account summary screen : This displays all the accounts that are held by a single person or tied to a single bank provided id, which might be savings, current or otherwise.

The Passbook Screen : This screen provides all the transactions that were committed against the account including the date, the particulars of the transaction, whether it was debit or credit, the mode of transaction, i.e. physical or digital, the currency with which the transaction occurred, i.e. bitcoin, Australian Dollar, Indian Rupee etc and finally the balance after performing that particular transaction.

The Cards Screen : Another high level overview screen that shows all the credit/debit/authorized mobile payment devices that are linked to the ID provided by the bank.

The Cards Transactions Screen : Upon clicking on one of the linked cards, the user is redirected to another page where the outstanding balance on the card along with all the transactions that are committed by the card are displayed. This includes the date on which the transaction was committed, the particulars of the transaction, the amount for the transaction and finally the outstanding balance after committing the transaction.

The Funds Transfer Screen : Allows the user to send and receive various kinds of currency using the application.

Apart from these, we’ll also have the regular login screen, the offer screen and a budget management screen that allows users to set their monthly budget and try to maintain it using the account details provided.

Currently we have the front end in place for the application and we are refining some of the UI elements. If selected we plan to build the entire application using spring boot and web 3 technologies.

List of technologies used :

· Angular JS : The front end framework favoured by many.

· HTML 5

· CSS 3

· Bootstrap 4

· Spring Boot : To allow us an annotation based backend service where convention is more important than configuration.

· IBM Bluemix Blockchain Prototype : We are currently using IBM’s blockchain prototype to simulate all transactions, we plan to replace this with a blockchain of our own design if given the opportunity.

· PostgreSQL : For all CRUD operations as shown in Figure 2, we plan to make use of a postgresql database owing to it’s multitude of features from ease of use to security.

By solving these problems, we hope to create a more stable and easy to use financial application than anything else available in the market currently and thereby usher the world of banking into the millennial generation.
