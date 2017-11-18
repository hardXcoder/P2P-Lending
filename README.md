# P2P-Lending (RAINBOW)

Our project is a decentralised Lending solution for SMEs, Individuals, Cooperatives and Self-Help Groups.
SMEs are the financial cornerstones for every developing economy. The idea behind these loans would be to Support entrepreneurship , Encourage the people of Africa towards starting their own businesses and attaining Financial independence
These loans would be especially geared towards the “Unbanked” people who would typically lack in -Collateral, Steady employment, and/or a verifiable credit history
We have devised a comprehensive plan where every customer can easily apply for a loan , provided the presence of a working business plan. The solution adopts adopts to various methods of repayments, making it flexible for the customer as well as the investor.
All the transactional details like the approval of the loan, making payments/purchasing equipments and supplies as well as making repayments on the loans occurs via our Blockchain based banking platform.


Link to the presentation :
(https://goo.gl/xfPnhg)

# Members of the network

# Engines

Engines hosts the logic and the state of all the loans using them; they can implement any custom rules about interest, due times, cancelable timestamp, or more parameters. However, we recommend following a standard interface and specifications.

# Oracle

Oracles provide equivalencies between our platformm and other currencies; they should implement the oracle.sol interface to be compatible with other members of the Network.

Maintaining a Oracle could be a relatively costly task, so it's a suggested practice add a little fee to deliver the rate.

# Contracts

NanoLoanEngine

A NanoLoan is a Loan whose entire principal value is paid all at once on the maturity date dueDate, as opposed to amortizing the bond over its lifetime.

The lifetime is divided in two periods by a parameterizable date called cancelableAt. Before that date, the Borrower must pay the nominal value of the credit to cancel the obligation. After that date and until the expiration, the amount to be paid for redeem the obligation is composed of the principal value and interest accrued between the origination date and the due date.
