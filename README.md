# UMADeveloperOnboardingEducationRollOut
The broad aims of this proposal are to improve developer onboarding of UMA products into already existing platforms.  Such as decentralized exchanges or DAOs.

# Value Proposition
UMA offers technologically advanced services across a range of product needs in the decentralized ecosystem.  

These include highly secure oracle services - data feeds

Key Performance Indicator (KPI) Options - for use in DAOs for example.  These are options whose payouts are made to token holders if key key performance indicators are reached.  The optimisitc nature of UMAs oracle provides a strong game theoretic basis for unbiased provision of the underlying KPIs.

And a range of other products including success tokens, range tokens, synthetic tokens, call options (ok, this is one enough people should already know), and protected tokens.


# Challenges

The documentation and presentation is done as if the underlying mechanismm and value propositions of these products and their corresponding terms (e.g. success tokens) are well understood.  While the naming is intuitive, it is still very confusing for someone who is not already part of the ecosystem.  More specifically for those who have not already invested their time to overcome the barrier of understanding.  It is written as if the meaning of these terms and their potential application should be easily grasppable.  The reality is, it is not.

A core challenge in offering sophisticated services in an already sophisticated space is clarity of communication.

It needs to be clear what each  service does and how it can be used to expand an existing organizations product offering or offer incremental (and hopefully subtstantial value) over existing alternatives.

For example, what a KPI option is, or how it works for that, and how it can be incorporated into a DAO is hard to grasp without a concrete and tangible example.  It is possible to grasp what it is in essence from the existing documentation for an expert, however, seeing the true value and having examples that make the developer feel that implementation and execution is within reach a key requirement for developer onboarding.  It is especially important to stand out as the lowest hanging fruit in this space when there are so many other solutions and opportunities available.

Furthermore, the documentation does not show the pathway for integration.  It assumes the developer already knows how they will want to use UMAs products rather providing a template or an environment for discovery.


# The Paradigm for Product Adoption and Integration and Improvements to Product Communcation and Clarity
This can be done through a variety of mechanisms.  One common, though less effective approach, is through the provision of developer docs that do not have fully worked examples, videos, or git hub repos.

The current state of the opportunities for developers is seemingly one of endless opportunities.  In an environemnt of abundant opporunities, many players will be initially attracted to a product offering but when faced with even a modest level of challenge for onboarding will become disuaded from pursuing further.  This should not even be viewed as a weakness or deficiency.  It may even be even be close to game theoretically optimal behavior - the likelihood of finding an opporunity which can in the end provide similar value to the developer but with substantially less risk of lost time and effort is high.

It is critical to address this by improving the value propostion.  The most successful products for onboarding new developers offer open source code repos of fully working examples with clear instructions on how to stand up projects.  The worked examples are often carefully curated to onboard developers whose interests align with the protocols ambitions for expansion.
 
A suite of examples will be developed across the range of UMA products.  Covering not just calls to the contracts where UMAs products may be deployed for example, but also demonstrating novel use cases with the intention of inspiring innovative developer onboarding.

Some potential examples are further touched on below.

# Rolling out an UMA integartion into an existing and DeFi application
DFX offers an extremely strong platform for decentralized trading of fiat back crypto currencies across a range of underlying currencies e.g. CAD, USD, etc...

Delivering a worked example in the form of a clear and easy to understand example that is available through different forms of media including documentation, a video walkthrough of development, and most importantly a full working github repo with complete stups on how to stand up the project and interact with all its functions.

This worked example would go through the processes of:
  1. market and objective identificaiton (in this case an FX spot for example)
  2. implementation of the price oracle (if there are multiple ways of deployment these should be covered)
  3. Development of a smart contract which interacts with the deployed price oracle
  4. Integration of the smart contract into an iterative development platform like Scaffold-Eth
  5. A web portal which list all of the active UMA oracles being used by DFX 

Not only would this provide considerable value to the DFX platform, it would further serve in disseminating understanding of UMAs products within the developer community.  This dissemination would at least be partially fueled by potential financial gains from contributing to a successful project such as DFX.

UMA could also be futher used for the development of a KPI tied to the provision of liquidity, execution of liquidations, or TVL that would support the use of the DFX platform.  For example, previous attempts have been made to use KPIs to incentivize adoption of DFX by offering KPI options on TVL.  One issue with the initial appraoch was that these KPIs were set at an extremely high level of TVL, once it became doubtful about the ability to meet these thresholds interest in the community began to wane.  An improved approach would be to offer a sort of laddered KPI options offering increasing payoff amounts at successively high TVL thresholds.

# Example of Workflow for Scaffold-Eth
Simplest Examples - The simplest possible example would be to use https://solidity-by-example.org/defi/chainlink-price-oracle Scaffold-eth example using chainlink and carry that over to UMA.  This could be easily accomplished with the following workflow:

1. clone scaffold-eth repo from: https://github.com/scaffold-eth/scaffold-eth
2. modify the solidity file 'YourContract' to the .sol file in https://solidity-by-example.org/defi/chainlink-price-oracle.
3. Change the address of the oracle in the AggregatorV3Interface to the addres of a known UMA oracle
4. Provide int the project read me a clear description of the interface of the UMA oracle, in addition to reference to the source solidity documentation.
5. Include some additional calls in the main solidity file of the project to explore the interface
6. launch the contract and dynamically generated front end using the following commands

install dependencies

   yarn install
   
start the hardhad chain

   yarn chain
   
deploy the contract

   yarn deploy
   
launch the front end

   yarn start
   
7. Provide some examples of what to do once the application is launched.  Provide a series of additional challenges in the spirit of speed run https://medium.com/@austin_48503/%EF%B8%8Fethereum-dev-speed-run-bd72bcba6a4c

Additional workflow steps to below to mainnet:
modify the 


# Rolling out UMA integration of KPIs into DAOs operations
For example, providing a working example of how KPIs could be set through DAO consensus to student developer projects.  Furthermore, KPIs that could be generated to measure the performance of DAO participants and provide rewards for their engagement in DAOs.

# Onboarding of UMA services and the development of knew products
Once it is better understood by developers and decentralized market participants how UMAs products work the sky really is the limit.  For exammple, it would be possible to develop market for options on KPIs that parallel the traditional finance and defi derivative markets.  Existing methodology for valuing options that uses metrics of volatility for example could be developed and this could spawn an entirely new area of research.
