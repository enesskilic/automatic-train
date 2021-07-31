## Utility class generator for CSS.

### Installation

> $ git clone https://github.com/enesskilic/automatic-train.git

### Usage

> Compile the **main.scss** file and link it to your file.

### How to expand

>  **Step 1:** Add your new variables and maps to **_variables.scss** file.

    // Your new variable
    $space-unit: 1rem;
    
    // Your new map
    $spaces: (
	    1: $space-unit * 1.25,
	    2: $space-unit * 1.50
    );

>   **Step 2:** Add a new map to the `$utilities` list in the **_utilities.scss file.**

    $utilities:
    (
	    "class": margin-y,
	    "property": margin-top margin-bottom        // You can use multiple properties like this.
	    "values": $spaces                           // The map in the _variables.scss file.
    ),
    .
    .
    .

>   **Output:** 
    
    .margin-y-1 { margin-top: 1.25rem; margin-bottom: 1.25rem }
