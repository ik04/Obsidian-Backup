# Import csv:

``` javascript
const handleFileUploadPortfolios = (e) => {

const file = e.target.files[0];

if (!file) return;

  

Papa.parse(file, {

header: true,

skipEmptyLines: "greedy",

complete: (results) => {

console.log("Parsed Results:", results);

  

// Filter out entries with missing or empty required fields

const invalidEntries = results.data.filter(

(entry) =>

entry.name.trim() === "" || entry.investmentMonth.trim() === ""

);

  

console.log("Invalid Entries:", invalidEntries);

  

if (invalidEntries.length > 0) {

console.error("Invalid entries found in the file:", invalidEntries);

message.error("Invalid entries found in the file.");

return;

}

  

setImportedPortfolios(results.data);

message.success("Startups imported successfully.");

// router.reload();

  

// const validEntries = results.data.filter(

// (entry) => entry.name.trim() !== ""

// );

  

// if (validEntries.length === 0) {

// console.error("No valid entries found in the file.");

// message.error("No valid entries found in the file.");

// return;

// }

  

// setImportedPortfolios(validEntries);

// message.success("Portfolios imported successfully.");

// router.reload();

},

});

};
```

# Export Csv:
## template:
```javascript
const [initialPortfolioData, setInitialPortfolioData] = useState([

{

name: "ik",

description: "",

investmentMonth: 1000,

totalInvestmentByFund: 100,

currentEquityStatus: "",

ValueFundInvestedAt: 1000,

currentPostMoneyValuation: 10000,

currentValueOfInvestment: 10000,

moic: 1000,

followOnInvestor: "",

coInvestors: "",

arrOnEntry: "",

arrNow: "",

fundAssociated: "",

},

]);
```

## Execution:
```javascript
const items4 = [

{

key: "1",

label: (

<Button type="text" onClick={() => importPortfoliosRef.current.click()}>

Import CSV

</Button>

),

},

{

key: "2",

label: (

<CSVLink filename="my-file.csv" data={initialPortfolioData}>

<Row justify="center">Export CSV</Row>

</CSVLink>

),

},

];
```
