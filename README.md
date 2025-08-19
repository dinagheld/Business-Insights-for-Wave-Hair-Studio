# Business-Insights-for-Wave-Hair-Studio
## Business context
The Waves salon has been on the market for six months, delighting clients with curly hairstyles. Like any business, they are focused on increasing profitability. Their reporting is managed manually in Google Sheets, and they provided us with exported data. The goal is to analyze the structure of income and expenses: how much is spent on operations, what revenue is generated, the main expense categories, and the key sources of income. <br/>

Additionally, the analysis should address the following questions: <br/>
How much the salon spends on promotions and whether these investments pay off: <br/>
a. analyze promo campaigns to see which bring the greatest effect in attracting clients — which promo codes are used most often; <br/>
b. measure how much revenue the salon loses due to discounts; <br/>
c. calculate the average check amount for each promo campaign. <br/>

## Data structure and its description
The log the salon has provided us with is stored in Google Sheets and has 2 sheets: export and promocodes. In the 'export' sheet we have all the transactions the salon encountered with, containing both income and expense content for the 6 months of operation. The 'promocodes' sheet holds information about marketing campaigns employed to support the sales, revealing data about the campaign that was used and the its discount given to customers.  <br/>
 <br/>
Here is the list of the fields disclosed in the log: <br/>
'export': <br/>
 <br/>
**ID** - A unique identification code is assigned to both income and expense transactions. The identifier is entered manually and represents a sequential transaction number. <br/>
<br/>
**Transaction** - Information indicating whether the transaction relates to income or expenses <br/>
<br/>
**Type** - Information about the payment method: cashless or cash payment  <br/>
<br/>
**Category** - Name of the product or service being paid for <br/>
<br/>
**Order date and time** - Despite its naming the field disclosed only date, no time specified <br/>
<br/>
**Promocode** - Promocode for the discount if used <br/>
<br/>
**Standard price** - The cost of the product or service before discount <br/>
<br/>
 <br/>
'promocodes': <br/>
**promocode** - Promocode for a discount<br/>
<br/>
**id_campaign** - Unique identifier of the marketing campaign associated with the promo code<br/>
<br/>
**discount** - The discount rate (in percent) that the client receives when applying a promo code<br/>
<br/>
**campaign_name** - Name of the marketing campaign<br/>
