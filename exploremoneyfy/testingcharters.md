## Exploratory Testing Charters for *Monefy App*

<br><br>

|Charter 1	| Navigate different areas of the app to find further explore options	| 
|:-------| :-------- |
|Areas | General / All|
|Duration| Short (30 mins)|
|Test Notes| <li>Navigate through various areas to see everything is displayed</li>  <br> <li>To check different entities available and their usage</li> <br> <li>Check basic functionality </li>|
|Bugs| None|

<br/> <hr/> <br/>

|Charter 2	| Adding different expenses records on home quickly with + and - image clicks	| 
|:-------| :-------- |
|Areas | Expenses|
|Duration| Short (30 mins)|
|Test Notes| <ul><li>Adding expenses under different selected categories</li> <br> <li>Verifying the expenses are added shown in the home pie chart properly</li> <br> <li>Expense chart is indicated with direction and percentage of the category</li></ul>
|Bugs| None|

<br/> <hr/> <br/>


|Charter 3	| Balance details with Amounts Spent By Category or alphabetically| 
|:-------| :-------- |
|Areas | Balances|
|Duration| Short (30 mins)|
|Test Notes| <li>Adding expenses under different selected categories</li> <br> <li>Verifying the Balnces details list in Balances</li> <br> <li>Order by Category or chronologically </li>|
|Bugs| None|


<br/> <hr/> <br/>

|Charter 4	| Add various Incomes, different category Expenses and check balance | 
|:-------| :-------- |
|Areas | Balances|
|Duration| Short (30 mins)|
|Test Notes| <li>Adding different types of income</li> <br><li> Verifying the Balances & balance details list</li> <br><li> Add expenses with different categories</li> <br><li> Verifying the Balances & balance details list </li>|
|Bugs| None|

<br/> <hr/> <br/>

|Charter 5	| Managing New Category and creating expense against new category | 
|:-------| :-------- |
|Areas | Categories|
|Duration| Short (30 mins)|
|Test Notes| <ul><li>Adding New Category</li> <br> <li>Verifying new expense is created for new category</li> <br> <li>Editing and deleting existing category</li> <br> <li> Verifying "Merge" category updates expense records and  "Disable" does not showup</ul>
|Bugs| 1. Category name by default showing popup of address details|

<br/> <hr/> <br/>

|Charter 6	| Adding multiple range of spending amounts for number of expenses| 
|:-------| :-------- |
|Areas | Expenses|
|Duration| Long (90 mins)|
|Test Notes| <ul><li>Adding number of spending amount for expenses including very small and very large amounts</li> <br> <li>Verifying Spending chart is reflected properly with percentages</ul>
|Bugs| 1. When adding a major expense and all other very minor expenses (with same amount) then percentage pie chart is added with 000 image and improper direction line<br/> one directing is pointing one minor expense image and nothing pointing to 000 image<br/>Expected: As msg is given initially (only one time) all very minor expenses should be grouped and pointed to 000 images|

<br/> <hr/> <br/>

|Charter 7	| Changing Main Currency & updating exchange rates of used currencies| 
|:-------| :-------- |
|Areas | Currencies|
|Duration| Normal (60 mins)|
|Test Notes| <li>Creating two accounts with different currencies</li> <br> <li>Change main currency to another different</li><br/> <li> Verify the totals and balances
|Bugs| 1. Changing Main Currency to Other currency is directly showing total value of different accounts which are in different currencies <br/>No provision to add new exchange rates without adding accounts in another currencies<br />	Currency exchange rates are to be added in bi-directional to reflect the proper changes|

<br/> <hr/> <br/>

|Charter 8	| Add & Edit new account with Exchange Rates & without Exchange rates| 
|:-------| :-------- |
|Areas | Accounts|
|Duration| Normal (60 mins)|
|Test Notes| <li>Create different accounts with different currencies but not adding exhange rates</li> <br> <li>Verify the totals and balances</li><br/><li>Create different accounts with different currencies with adding exchange rates</li><br/><li> Verify the totals and balances</li>
|Bugs| 1. Amount is added to total without prompting for adding exchange rates when selected currency is different from Main currency<br/>Balance also reflects the same<br />	Ex: Main Currency = USD <br/>Account1 : 100 USD ,Account2 : 200 Euros  (no exchange rate defined)<br/>Total - Shown as 300 USD instead of 314 USD [ 100 USD + (200 * 1.07) USD] <br/><br/> 2. Total is not reflecting immediately when exchange rate is added after adding the account , need to revisit again to see the update|

<br/> <hr/> <br/>

|Charter 9	| Multi-currency display in balance details with different currency Accounts| 
|:-------| :-------- |
|Areas | Accounts, Balance|
|Duration| Normal (60 mins)|
|Test Notes| <li>Adding expenses different from base currency</li> <br> <li>Verify the balance details</li><br/><li>both currency amounts are shown in balance</li>
|Bugs| None |

<br/> <hr/> <br/>

|Charter 10	| User preferences and data options in settings | 
|:-------| :-------- |
|Areas | Settings, Data |
|Duration| Short (30 mins)|
|Test Notes| <li>Password protection checking with pin </li> <br> <li>Exporting data to csv file</li><br/><li>Data backup and restore with drive</li><br/><li>Clearing all Data
|Bugs| None |

<br/> <hr/> <br/>

### Prioritizing Charters
<li>First:  Charter 2 - Adding different expenses records on home quickly with + and - image clicks  (with buget option)
This one immediately picture of how the expenses are distributed in various categories , the total buget amount which is main goal of any customer to check the amount spendings and then looking for saving options
<li>Second: Charter 10 - Password and data protection options
<li>Third: Charter 8 - Accounts

<br/> <hr/> <br/>

### Risks to mitigate

<li> App requires manual feeding of Exchange rates but exchange rates change very often </li>
<li> User need to remember the every expense and need to input into app, no app notificatio to user </li>
<li> Synchronization between andriod and ios devices needs proper compatibility </li>
<li> Multi-currency conversion are not very transparent and confusing to user , could be error prone </li>
