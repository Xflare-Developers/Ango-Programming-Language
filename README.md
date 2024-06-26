# Ango-Programming-Language
# Ango is a Programming language that can help for making database such as MySQL
 

# Ango Programming Language Documentation
# Overview
# Ango is a simplified programming language designed for setting up and managing databases. It combines elements from JavaScript, Ruby, and HTML to provide an easy-to-use syntax for database operations.

Key Features
Variable Declaration and Assignment

Syntax: let variableName = value;
Example: let name = "John";
Database Setup

Syntax: setupdatabase.(databaseName, version);
Example: setupdatabase.(cloudiadatabase, 1);
Store Data

Syntax: store variableName in databaseName;
Example: store name in cloudiadatabase;
Retrieve Data

Syntax: retrieve from databaseName where condition;
Example: retrieve from cloudiadatabase where name == "John";
Ango Script Example
ango
Copy code
lng = <ango>

run.true

setupdatabase.(cloudiadatabase, 1)
=call= (cloudiadatabase, 1) -// storages, set ,gb, 4 , run.

-<savedata>-
root.5 = datasave
(savedata, true)
Integration with JavaScript
index.js
javascript
Copy code
const { exec } = require('child_process');

// Function to run Ango script
function runAngoScript() {
  return new Promise((resolve, reject) => {
    exec('ango run hello_ango.ango', (error, stdout, stderr) => {
      if (error) {
        reject(error);
      } else {
        resolve(stdout);
      }
    });
  });
}

// Function to run JavaScript script
function runJavaScriptScript() {
  return new Promise((resolve, reject) => {
    exec('node hello_js.js', (error, stdout, stderr) => {
      if (error) {
        reject(error);
      } else {
        resolve(stdout);
      }
    });
  });
}

// Run Ango script
runAngoScript()
  .then(angoOutput => {
    console.log("Output from Ango script:");
    console.log(angoOutput);
    // Run JavaScript script after Ango script completes
    return runJavaScriptScript();
  })
  .then(jsOutput => {
    console.log("\nOutput from JavaScript script:");
    console.log(jsOutput);
  })
  .catch(error => {
    console.error("Error occurred:", error);
  });
Integration with Bash
script.sh
bash
Copy code
#!/bin/bash

# Function to run Ango script
run_ango_script() {
    echo "Running Ango script..."
    ./ango run hello_ango.ango
}

# Function to run JavaScript script
run_js_script() {
    echo "Running JavaScript script..."
    node hello_js.js
}

# Main execution flow
run_ango_script
run_js_script
By following these steps, you can effectively share and promote Ango with a global audience



# THIS CODE IS FOR SIMPLICITY

 Ango Script Example

lng = <ango>

run.true

setupdatabase.(cloudiadatabase, 1)
=call= (cloudiadatabase, 1) -// storages, set ,gb, 4 , run.

-<savedata>-
root.5 = datasave
(savedata, true)
Integration with JavaScript
index.js
javascript
Copy code
const { exec } = require('child_process');

// Function to run Ango script
function runAngoScript() {
  return new Promise((resolve, reject) => {
    exec('ango run hello_ango.ango', (error, stdout, stderr) => {
      if (error) {
        reject(error);
      } else {
        resolve(stdout);
      }
    });
  });
}

// Function to run JavaScript script
function runJavaScriptScript() {
  return new Promise((resolve, reject) => {
    exec('node hello_js.js', (error, stdout, stderr) => {
      if (error) {
        reject(error);
      } else {
        resolve(stdout);
      }
    });
  });
}

// Run Ango script
runAngoScript()
  .then(angoOutput => {
    console.log("Output from Ango script:");
    console.log(angoOutput);
    // Run JavaScript script after Ango script completes
    return runJavaScriptScript();
  })
  .then(jsOutput => {
    console.log("\nOutput from JavaScript script:");
    console.log(jsOutput);
  })
  .catch(error => {
    console.error("Error occurred:", error);
  });
Integration with Bash
script.sh
bash
Copy code
#!/bin/bash

# Function to run Ango script
run_ango_script() {
    echo "Running Ango script..."
    ./ango run hello_ango.ango
}

# Function to run JavaScript script
run_js_script() {
    echo "Running JavaScript script..."
    node hello_js.js
}

# Main execution flow
run_ango_script
run_js_script
