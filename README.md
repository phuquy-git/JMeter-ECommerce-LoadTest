# Load Testing for [Test Store](https://teststore.automationtesting.co.uk/)

This repository contains resources and instructions for performing load testing on the [Test Store](https://teststore.automationtesting.co.uk/) website using Apache JMeter.

## Test Type
- **Load Testing**

## Website
- **URL**: [https://teststore.automationtesting.co.uk/](https://teststore.automationtesting.co.uk/)

## How to Open a Load Test with .jmx File in JMeter

1. **Download and Install JMeter**:
   - Download Apache JMeter from the [official website](https://jmeter.apache.org/download_jmeter.cgi).
   - Extract the downloaded archive to a suitable location.

2. **Open JMeter**:
   - Navigate to the `bin` directory within the JMeter folder.
   - Execute the `jmeter` script (`jmeter.bat` for Windows, `jmeter` for Unix/Linux).

3. **Open the .jmx File**:
   - In JMeter, go to `File` > `Open`.
   - Navigate to the directory containing your `.jmx` file and open it.

## How to Run by Command Line

1. **Navigate to the JMeter `bin` Directory**:
   ```bash
   cd /path/to/jmeter/bin
2. **Run the Test**:
   ```bash
    ./jmeter -n -t /path/to/your_test.jmx -l /path/to/results.jtl
**Options:**  
`n`: Runs the test in non-GUI mode (headless).  
`t`: Specifies the location of the JMX test script (<test_script.jmx>).  
`l`: Sets the location to store the generated test results (<results_folder>).  
## Features
### Think Time  
Simulates realistic user behavior by introducing a configurable delay (default: 500ms) between test actions.
### Test Fragments  
Enables the reusability of frequently used test components like login and logout procedures.
### Config Elements  
- HTTP Request Defaults: Streamlines configuration by setting default values for HTTP requests.
- User Defined Variables: Enhances test flexibility by allowing parameterization and reuse of variables across the test plan.
### Intuitive Reporting  
Generates a comprehensive report that provides valuable insights into the load test's performance and the stability of the tested system under load.
### Summary Report  
Following a successful load test execution, a detailed and user-friendly summary report is generated. This report offers crucial metrics to evaluate the load tolerance and performance characteristics of the system being tested.
