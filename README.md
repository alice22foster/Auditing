# Callisto Smart-contract auditing department.

## Callisto Auditing Department is encouraging the DAPP development community to queue the audit requests: any audit requests submitted before 7 / 12 / 2022 will receive a 25% discount. Audit requests will be processed starting at 7 / 13 / 2022 according to the standard workflow

Callisto Security department performs security audits of smart-contracts. Our security auditors are paid from [Callisto Treasury](https://github.com/EthereumCommonwealth/Roadmap/issues/48). Anyone can submit a request for security audit of a smart-contract following the rules described below.

# Security Audit options

There are three options of the security audit workflow suitable for small-, medium- and large-scale projects:
 - Standard (standard projects such as ICOs, ERC20, ERC223, ERC721, ERC721A tokens and NFTs fall in this category - 2 auditors. $500 + $1 per line of code / minimum $1000)
- Advanced (non-standard projects requiring more careful review - 3 auditors. $1000 + $1.25 per line / minimum $2000)
- Corporate (projects that require post-launch support - 3 auditors - Callisto Team will handle the bugbounty and provide a 1 month long period of technical support regarding the necessary security enhancement procedures and track/highlight any issues and potential threats - this plan allows to further apply for Callisto DAPP Insurance program)

# Submitting an audit request

Audit request can be submitted directly via [Github Issues](https://github.com/EthereumCommonwealth/Auditing/issues) or [open telegram channel](https://t.me/CallistoAudits) :

1. Go to Auditing/issues section and click a [New Issue](https://github.com/EthereumCommonwealth/Auditing/issues/new) button.
2. Fill the form and click a "Submit New Issue" button.
3. Follow the comments in the corresponding "issue" discussion.
4. The result of a security audit will be published at the comment thread with the `Security Audit Report` header once auditors complete their task.

# Applying for free-of-charge audit.

In order to get your project audited consider announcing the audit request for the public with any social media platforms (twitter/ reddit/ bitcointalk/ facebook) after submitting the audit request. Provide the links to the public audit request announcement in the comment thread of the audit request in order to help us track your audit recognition. Those projects whose announcements gain more traction and social media recognition will be audited for free within the month while the rest will be left for the next month or processed on paid basis.

If you are using our audit report or announcing it for the general public, then proper attribution is required: 

"Smart Contract Security Audit by Callisto Network" 

alternatively you can use our verified badge:

![alt text](https://github.com/sneg55/Auditing/blob/master/callisto-badge.png)

Anyone can submit a request of a security audit for an open-source smart-contract. After the creation of a security audit request, we will contact the developers of the smart contract. However the confirmation from the developers is **NOT** required. The callisto team will conduct an audit even if the project team does not confirm the request. Thus, any user can request an audit of any project, and the Callisto team will conduct this audit when the queue does not contain audit requests with higher priorities.

## Callisto Network is not a debugging tool!

Although we provide free audits, we ask our customers to understand that real people work in our organization, but not automated tests. We strongly recommend using specifically designed tools for debugging and testing. We also recommend using automated tests to verify minor changes and fixes.

Please, only submit your code for review once the development of the smart-contract is in its final stage and the contract is ready for deployment.

Only the first audit of a smart-contract code is free. If a customer submits an updated smart-contract for re-audit then it will be necessary to pay for the re-audit ($0,6 per line of code).

Re-auditing of a smart-contract includes a full check of the smart-contract code, as any minor changes could affect the overall behavior of the smart-contract. Even if 10 lines of code were changed, the entire smart contract will be re-audited.

There are two ways to avoid a complete re-audit if the contract is updated:

- break your smart-contract into modules so that they can be audited separately from each other

- cover the smart-contract code with [automated tests](https://www.trufflesuite.com/docs/truffle/testing/writing-tests-in-solidity) to prove that the update did not affect a behavior of the smart-contract

### Audit request payments

#### We accept ETH, ETC, CLO and EOS as payments.

Callisto Network adheres to the [policy of financial transparency](https://github.com/EthereumCommonwealth/Roadmap/issues/48). All the received payments are recorded, described, stored and represented publicly.

The requester can provide the payment for an audit request by sending a certain amount of CLO, ETH or ETC to the [0x74682Fc32007aF0b6118F259cBe7bCCC21641600 (Treasury address)](https://explorer.callisto.network/address/0x74682Fc32007aF0b6118F259cBe7bCCC21641600/transactions). EOS can be sent to this address [callistotokn](https://bloks.io/account/callistotokn).

| Priority | Payment formula |
| ---: | ---: |
| High | 500 USD + (0.5 USD per line of code) |

- Highest priority audits are processed before of any audits in the queue.

- High priority audits are processed before any audits in the queue, except for the highest priority audits.

The payment amount will be calculated based on the exchange rate of the currency that was used for the payment (calculated at [CoinMarketCap](https://coinmarketcap.com/) rate). The amount of payment depends on the length of the code of the auditable contract. Empty lines of code and comments can be excluded and it is not necessary to pay for them. It is recommended to use [SLOC counter](https://agingcoder.com/tool/2014/04/22/sloc-counter/) to calculate the accurate amount of lines of code that require payment. The overpaid amount of CLO, ETH, EOS or ETC will be returned to the sender's address after the completion of the security audit. Highest priority audit requests are processed ahead of queue.

NOTE: Requester can attach the hex-encoded Data to the payment transaction to help us identify the validity of payment. [ASCII-To-Hex converter](https://www.rapidtables.com/convert/number/ascii-to-hex.html) can be used for this purpose. Example: "Payment for CryptoKitties audit request" will be encoded as `0x5061796d656e7420666f722043727970746f4b6974746965732061756469742072657175657374`. EOS transactions should include the description as transaction `memo`. In case of EOS payment no encoding is needed.

Example:

If a user is willing to submit `MyToken.sol` (210 lines of code) contract for the audit and increase the priority of this request then he need to send $605 equivalent of CLO to Treasury address. He can attach the `0x5061796d656e7420666f72204d79546f6b656e206175646974` data to the transaction to prove that this is the payment for the MyToken audit priority.

![alt text](https://github.com/EthereumCommonwealth/Callisto-Media-Kit/blob/master/logo-official-twitter_506x253.png)

## Callisto Security Department workflow.

There are two types of participants in the Security Department:
- auditing manager
- security auditors

### Audit requests order (auditing manager)

For smart-contracts, the following order of audits is determined:
- Contracts that are important for the whole cryptocurrency industry, can have the highest priority.
- Contracts intended for deployment in the ETC/CLO network have the highest priority (with the exception of previous paragraph).
- Contracts of the ETH network have medium priority.
- Other contracts have low priority.
- If the audit of the smart contract is already started, then it continues until it is completed, regardless of the availability of other contracts with higher priority in the queue.

After the audit request has been created, it is viewed by the audit manager. If the request meets the requirements, then the auditing manager assigns it `approved` status. `approved` label means that the audit request is available for auditors for picking.

If there are several requests with different priorities in the queue, then the manager **should** assign the `approved` status only to contracts with the highest priority. The remaining contracts will be checked after the audit of the contracts with the highest priority has been performed. If there are several contracts in the queue with the highest priority, then the audit manager **should** assign the status of `approved` to all these contracts simultaneously. In this case, the contract that auditors will begin to check first will be checked earlier.

Audit requests that remained in "awaiting payment" status for more than 2 weeks must be closed.

### Performing an audit (security auditor)

After an audit request with an `approved` label appears, an auditor can pick it by commenting the issue and indicating how much time it should take to audit this smart-contract (roughly/ in days). After that, the auditor can start reviewing the code immediately. Other community members **may** also pick the request and submit their audit reports. These reports **must** be reviewed by auditor manager at the end of the auditing process. If the audit request was approved, but none of the auditors picked it, then the audit manager can appoint auditors to check this request if they are not engaged in checking another smart-contract.

Auditing manager **must** comment that the audit is successfully started and mention github nicknames of all the auditors which will be responsible for the check of the corresponding contract after several auditors have picked the issue-request. The audit manager **must** also comment his contact email, to which the auditors will send their secret gists (audit reports).

After the auditor began to check the code, he **must** create a **secret** [github gist](https://gist.github.com/) and send it to the auditing manager by email. An auditor **must not** reveal the audit report gist or publish it anywhere, so that only auditing manager and auditor (gist owner) could review it during the auditing process.

After the auditor has completed the verification of the code, he should comment to the appropriate issue that his audit report is completed. NOTE: An auditor **must not** reveal his report gist!

### Performing an audit (security auditing manager)

Security Auditing manager is allowed to participate in the audit process alongside assigned auditors. In this case he should create his own Audit Report gist as if he was an auditor and perform the review of the contract code. Since the manager sees all the auditors' reports in the process, he should only describe those findings that the other auditors failed to report.

Security Auditing manager is not obligated to participate in the auditing process.

There are two possible scenarios for rewarding Security Auditors and Auditing Manager:

1. In case the Auditing Manager found any "medium" or higher severity issues that other auditors failed to report then these "medium" severity issues must be used in the reward calculation formula (see [Auditing Department reward calculation v2](https://github.com/EthereumCommonwealth/Roadmap/issues/57)). Auditing Manager is paid for the finding of this issue upon completing of the audit as if he was an active auditor.
2. In case the Auditing Manager did not found any "medium" or higher severity issues that other auditors failed to report then the Auditing Manager is excluded from the process of reward calculation.

### Completion of the audit

After all the responsible auditors have completed their reports, the audit manager must compare the reports.

If there are no significant discrepancies in the reports and no critical errors were found, then the audit manager **must** complete the audit by summarizing the reports and submitting secret gist urls in the comment thread of the corresponding audit request-issue. The audit is considered complete after all the responsible auditors have submitted their reports, and the audit manager has summarized the results of these reports and published report gist urls.

If one of the community members has expressed a desire to participate in the audit of this contract and also sent his report to the audit manager, then the audit manager **must** review the report and comment its secret gist url to the corresponding github request-issue regardless of whether the audit was already completed or not.

If any of the auditors described findings that were not included in the final report, then the auditing manager **must** describe the reason for excluding these findings in the comment thread of his fork of the auditor's report-gist.

### Disclosure policy

Read more here: [Standard disclosure policy of Callisto](https://github.com/EthereumCommonwealth/Auditing/blob/master/Standard_disclosure_policy.md)

After the audit was completed, the audit manager **may** inform the customer about the results without revealing the reports. After 15 days from the date of informing the customer about the findings, the reports should still be published and the results summed up.

## Security Auditor's Salary

Security auditors are paid based on the results of their work. Depending on the payment scheme for audit requests (free auditing campaign or paid audit), the auditor's salary is calculated using the methods described below.

In the Security Department of Callisto, smart-contract auditors are paid once a month.

The total amount of payment is calculated based on the amount of tasks performed during the last month. Each security audit is evaluated separately and a security auditor receives payment for each audit performed.

Each finding has a certain weight in points. The following values will be used to evaluate findings according to its severity: 

| Severity | Weight in points |
| ---: | ---: |
| Critical | 100 |
| High| 45 |
| Medium | 8 |
| Owner privileges | 2 |
| Low/Note | 1 |

The following formula is used to calculate the auditor's reward for the assigned task:

![image](https://user-images.githubusercontent.com/26142412/54073247-6ea3b800-429e-11e9-9d74-4a5c2073da0e.png)

Where:

`reward` - the amount of CLO that will be paid to the auditor for his(her) contribution to this security audit.

`audit reward` = $500 + $0.5 * `[number of lines]`

`sum (auditor points)` - all points earned by the auditor.

`sum (total points)` - sum of the all points earned by each auditor individually.

The `[number of lines]` of code in the source code of the auditable smart-contract which is calculated excluding empty lines and comments. [SLOC Counter](https://agingcoder.com/tool/2014/04/22/sloc-counter/) will be used for this purpose.

Auditors will receive the reward depending on the quality and quantity of the work done.
If a contract has only low severity issues or no issues then it’s reward will be divide equally between all auditors who worked at the security audit of this contract.

# Security Auditor's guide

## What the auditor of smart-contracts should do.

The main task of each security auditor is to check the code for security-related mistakes and write a report on the detected errors after the audit is completed.

1. All the work will be coordinated through github. Each auditor **must** visit the [Auditing/issues](https://github.com/EthereumCommonwealth/Auditing/issues) repository section every (working) day.

If an audit request (issue) which is labeled `approved` appears in the list,  the auditor **may** pick it. The audit manager can also appoint an auditor if he is not currently engaged in any smart contract checking, by mentioning their github nicknames in the corresponding issue. If the auditor was appointed to a certain issue by the auditing manager, then the auditor **must** perform a verification of the corresponding contract.

2. After the auditor has received the objective of his work, he **must** comment the time that, in his opinion, will be required to verify this smart-contract. 

3. The auditor **must** create a **secret** gist (audit report template) and send it to the auditing manager by email. WARNING: the auditor must never reveal the gist url. It will be revealed by auditing manager at the end of the auditing process. The secret gist should be named as follows: `NETWORK_contract_name_report.md`

Example: `ETH_the_dao_report.md`

4. The auditor **must** check the contract code, perform necessary testing and describe findings at the secret gist (audit report).

Other auditors, community members and the audit manager will also check this smart contract, so the auditor is not incentivised in hiding the errors found or trying to exploit them.

5. After the auditor has completed the verification of the code and supplemented his report with a description of the findings, he should comment the corresponding issue that his report is finished.

# Audit Report template

The audit report name should start with a capital letter. Use underscores instead of spaces between words, write reports in `.md` format.

The report should contain a title describing to which contract or contract system the report belongs.

The report should contain the following sections:

## 1. Summary

Briefly describe the audit report, the purpose of a contract (or contract system) that was reviewed and key features of the contract.

*This may be important to understand the inner logic of the contract or a contract system.*

## 2. In scope

Specify the range of contracts, the version of the contracts that have been verified. If the source code was published on Github, then specify the commit hash.

#### 2.1 Excluded (optional)

Specify which files or contracts were not checked during the audit if there were any contracts/files that were excluded for some reason.

## 3. Findings

Summarize the total amount of mistakes and their severity.

## 3.x Error ( `severity` )

*Describe each bug/mistake/error separately*

Severity assigning:

- high - vulnerability can be exploited at any time and cause a loss of customers funds or a complete breach of contract operability. *(Example: [Parity Multisig hack](https://medium.com/@Pr0Ger/another-parity-wallet-hack-explained-847ca46a2e1c), a user has exploited a vulnerability and violated the operability of the whole system of smart-contracts (Parity Multisigs). This could performed regardless of external conditions at any time.)*

- medium - vulnerability can be exploited in some specific circumstances and cause a loss of customers funds or a breach of operability of smart-contract (or smart-contract system). *(Example: [ERC20 bug](https://gist.github.com/Dexaran/ddb3e89fe64bf2e06ed15fbd5679bd20), a user can exploit a bug (or "undocumented opportunity") of `transfer` function and occasionally burn his tokens. A user can not violate someone else's funds or cause a complete breach of the whole contract operability. However, this leads to millions of dollars losses for Ethereum ecosystem and token developers.)*

- low - vulnerability can not cause a loss of customers funds or a breach of contracts operability. However it can cause any kind of problems or inconveniences. *(Example: [Permanent owners of multisig contracts](https://gist.github.com/Dexaran/2389d5e7290ab69709d33abfe0485bec#1-permanent-ownership), owners are permanent, thus if it will be necessary to remove a misbehaving "owner" from the owners list then it will require to redeploy the whole contract and transfer funds to a new one.)*

- minor observation - other code flaws, not security-related issues.

- owner privileges - a specific severity class for findings which provide the owner with the ability to manipulate the contract in such a way that it could theoretically harm users in case the owner will act maliciously or the owners account get compromised.

#### Code snippet

Give a link to a fragment of code that can lead to an error that you describe.

#### Description

Describe this finding in detail.

#### Recommendation (optional)

Write down how the bug can be fixed if you know how to do it. However, fixing bugs is not the primary goal of the security auditor.

## 4. Conclusion

Describe the most important findings and their relationship to the main purpose of the contract. Describe how the internal logic of the contract is related to its purpose.
Indicate whether the contract is safe or any critical problems needs to be resolved.

# Example: ETC multisig audit report

https://gist.github.com/Dexaran/2389d5e7290ab69709d33abfe0485bec

