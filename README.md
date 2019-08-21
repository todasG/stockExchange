# stockExchange

A .NET Library for retrieving Companies' data from different Stock Exchanges.

## Installation:

Install package via Nuget: https://www.nuget.org/packages/stockExchange/<br><br>
PM> Install-Package stockExchange<br><br>

## Instructions:

Create a stockExchange object.<br>
var exchange = new StockExchange([ProductId]);<br>

The library does not cache calls. You can change cache option.<br>
var exchange = new StockExchange([ProductId], RequestCacheLevel.BypassCache); //Default Option)

## Sample:

var exchange = new StockExchange([ProductId], RequestCacheLevel.BypassCache); //Default Option)<br>
<Company> comps = exchange.GetCompanyInfo(Exchange.NYSE, null, Region.North_America, Industry.Finance)<br>
foreach(Company comp in comps){} 
 
