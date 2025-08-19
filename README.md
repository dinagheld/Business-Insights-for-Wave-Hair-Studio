# Business Insights for Wave Hair Studio
## Business context
The Waves salon has been on the market for six months, delighting clients with curly hairstyles. Like any business, they are focused on increasing profitability. Their reporting is managed manually in Google Sheets, and they provided us with exported data. The goal is to analyze the structure of income and expenses: how much is spent on operations, what revenue is generated, the main expense categories, and the key sources of income. <br/>

Additionally, the analysis should address the following questions: <br/>
How much the salon spends on promotions and whether these investments pay off: <br/>
a. analyze promo campaigns to see which bring the greatest effect in attracting clients — which promo codes are used most often; <br/>
b. measure how much revenue the salon loses due to discounts; <br/>
c. calculate the average check amount for each promo campaign. <br/>

## Data structure and its description
The log the salon has provided us with is stored in Google Sheets and has 2 sheets: export and promocodes. In the 'export' sheet we have all the transactions the salon encountered with, containing both income and expense content for the 6 months of operation. The 'promocodes' sheet holds information about marketing campaigns employed to support the sales, revealing data about the campaign that was used and the discount given to customers.  <br/>
 <br/>
Here is the list of the fields disclosed in the log: <br/>
<br/>
**EXPORT Sheet:** <br/>
 <br/>
**ID** - A unique identification code is assigned to both income and expense transactions. The identifier is entered manually and represents a sequential transaction number. <br/>
<br/>
**Transaction** - Information indicating whether the transaction relates to income or expenses <br/>
<br/>
**Payment type** - Information about the payment method: cashless or cash payment  <br/>
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
**PROMOCODES Sheet:**  <br/>
<br/> 
**Promocode** - Promocode for a discount<br/>
<br/>
**ID campaign** - Unique identifier of the marketing campaign associated with the promo code<br/>
<br/>
**Discount** - The discount rate (in percent) that the client receives when applying a promo code<br/>
<br/>
**Campaign name** - Name of the marketing campaign
<br/>
<br/>
## Data cleaning and preprocessing
Prior to working with the dataset it was cleaned from duplicates, manual errors and anomalies. The NULL values in the *Standard price* column were replaced with corresponding values based on the price list after consulting with the stakeholders who confirmed it's the right way to proceed. The cells containing blank spaces were trimmed, and the formatting was fixed. 
<br/>
<br/>
## Data enrichment
The new attributes and calculated fields were added to the initial dataset for further analysis. The new fileds are colored in blue while initial ones are marked green. 
Since the salon renders hair services as well as sells hair products, the categorization between service and physical product was introduced to understand the content of revenue (Item type).
In order to dive into analysis of promo campaigns the information about applied discount (percent and absolute value) was mapped to each transaction. Based on that we were able to derive the amount after discount - the net amount received by the salon. 
<br/>
<br/>
## Executive summary report
<br/>
<img width="489" height="302" alt="Revenues consistently exceed expenses, keeping the business profitable" src="https://github.com/user-attachments/assets/ac92724f-8ebf-4c10-8db5-c4f1ff76e189" />

<img width="489" height="302" alt="Only 3% of total revenue comes from products" src="https://github.com/user-attachments/assets/2a83c3df-223e-41ed-881b-f5eea6d0135a" />

<img width="990" height="607" alt="Haircuts and styling services represent the primary source of revenue" src="https://github.com/user-attachments/assets/ecc226d0-07ba-492d-b281-32c1e8607bad" />

<img width="990" height="602" alt="Payroll constitutes the largest expense category, making up 75% of total costs" src="https://github.com/user-attachments/assets/e6da5453-6dc3-4c7c-87b7-ce10d79e8af6" />
<img width="610" height="283" alt="Lowest-performing promo campaigns by lost revenue" src="https://github.com/user-attachments/assets/8a4a9bb2-7a1d-499e-a11c-8a58c2c4c556" />
<img width="971" height="514" alt="Demand for haircuts and styling services remains steady with a slight decrease from April to May due to vacation of some employees" src="https://github.com/user-attachments/assets/f0820ca1-9e0c-4f3d-876e-4c32060d1fc1" />
<img width="971" height="522" alt="Demand for hair products remained stable  The increasing trend for hair gel might indicate that more people may have become aware of the importance of gel for styling curly hair" src="https://github.com/user-attachments/assets/0f12e442-ca23-4dcf-bf9d-aa3d04201d86" />



