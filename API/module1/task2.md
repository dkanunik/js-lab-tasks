# Module 1

## Task 1

### Description
For this task you have to create API test for Yahoo public API.

The Model should support ability to define values for HTTP request parameters

The tests should contain the following verifications:
- HTTP response code
- HTTP headers

### Preparation
1. Clone the template project https://github.com/dkanunik/api-test-with-jest
1. Install dependencies ```npm install```

### Project stuff
- Finance model https://github.com/dkanunik/api-with-jest-simple/blob/main/model/FinanceModel.mjs
- Tests https://github.com/dkanunik/api-with-jest-simple/blob/main/tests/finance.test.mjs
- Endpoints descriptions https://github.com/dkanunik/api-with-jest-simple/blob/main/configs/AppConfig.cjs

### Specification
Develop 4 test cases and tests for them to verify that the HTTP response code equals 200 when the following parameters
are put to Finance.getFinanceData():
- company
- region
- interval
- range

As example:
```
    ...
     let { status } = await Finance.getFinanceData({company:'AAPL'});
    ...
```

### Test run
``` npm test```

### Expected result
```
...
```

### Documentation
Please, use the following manuals to perform tasks:
- https://jestjs.io/docs/getting-started
- https://www.npmjs.com/package/axios
- https://developer.mozilla.org/en-US/docs/Web/HTTP/Status
- https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers