# Solution for preventing potential corrpution of community managers in ImpactMarket

## Description 

This proposal aims to improve the utility of funds raised from donors and the public by preventing potential corruption of community managers. Here I have introduced the formula proposed by Robert Klitgaard to illustrate how to solve the problem of corruption by reducing discretion as well as monopolisation of power, and elevating accusation afterwards.

## Scope

### Preventing the potential corruption in ImpactMarket

Here were also some poverty elimination projects in China but nearly all of them failed because of corruption. I believe that it is also necessary for ImpactMarket to prevent abuses of power. In 1988, Robert Klitgaard, a sociologist proposed a famous formula to describe the factors of corruption: 

$C = D + M - A$

where $C$ stands for corruption, $D$ represents for discretion, $M$ is for monopolisation of power and $A$ is for accusation afterwards. I believe that this formula can still be referred to the case of ImpactMarket.

#### Reducing D: add limiting parameters to managers' operations

According to the present documentation of ImpactMarket, community managers can submit the community for approval and manage all the community's beneficiaries on their discretions. However, this power can be abused, which may result in an issue that a manager may drag in a beneficiary to get more funds from the DAO and then remove him/her right after getting access to the funds. This can be achieved by setting up a lock-down mechanism, that we regulate a period, for example, a week, before the end of which the managers can not remove any beneficiaries. Plus, we need also limit the number of beneficiaries that one manager is allowed to add in a certain length of time, for example, 24 hours.

#### Reducing M and Promoting A: assign and reward community managers according to their contribution

Different from traditional banks or other financial institutions, ImpactMarket does not conduct KYC, which may compromise the system to smurf accounts. In the current version of protocol, the managers can be selected by other managers, which could lead to monopolisation of power. For example, a manager could create many smurf accounts and select them as new managers, as a result, a single person could control many communities with a bunch of fraudulent identities. To solve this problem, I believe that we can set up metrics as contribution indicators of these managers based on behavioral logics. 

Given that the project aims to help with people in extreme poverty, we can try to identify some unique characteristics of the target group. For example, people in extreme poverty (1.90 USD per day) are not likely to deposit their fund into banks, instead they will spend the money on foods and other living necessities. So that we can make full advantages of blockchain, tracking on the final destination to which the cUSD flows to. For instance, if we allocate 1000 cUSD to one of the managers, we can investigate how much flows to the authorized merchants eventually and use the ratio as a metric. In this case, if 900 cUSD finally flows to the authorized merchants, we can see that the ratio is 0.9 or we can say that 90% of the fund to this manager is used to improve the living quality of poverty (maybe the rest of 10% are transferred to other places, which is not likely the behavior of poverties). If a manager's metric is below than a certain level, let's say 0.9, then he/she will be disqualified to be a manager. Of course, if a manager maintains his/her score above a certain level, like 0.95 for a period long enough, like 6 months, then he/she will be rewarded by an amount of $PACT token and has a louder voice in the governance.

## Metric of community managers

$FRM/FAR$: fund received by authorized merchants/fund allocated to this manager
