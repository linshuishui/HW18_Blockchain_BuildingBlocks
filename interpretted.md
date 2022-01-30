# PyChain Ledger

Build a blockchain-based ledger system, complete with a user-friendly web interface

Update the provided Python file, which already contains the basic `PyChain`:

1. Create a new data class named `Record`. It a blueprint for the financial transaction records that the ledger blocks will store.

2. Modify the existing `Block` data class to store `Record` data.

3. Add Relevant User Inputs to the Streamlit interface.

4. Test the PyChain Ledger by Storing Records.

## Instructions

### Step 1: Create a Record Data Class

Define a new Python data class named `Record`. Give this new class a formalized data structure that consists of the `sender`, `receiver`, and `amount` attributes.

1. Define a new class named `Record`.

2. Add the `@dataclass` decorator immediately before the `Record` class definition.

3. Add an attribute named `sender` of type `str`.

4. Add an attribute named `receiver` of type `str`.

5. Add an attribute named `amount` of type `float`.

### Step 2: Modify the Existing Block Data Class to Store Record Data

Rename the `data` attribute in your `Block` class to `record`, and then set it to use an instance of the new `Record` class.

1. In the `Block` class, rename the `data` attribute to `record`.

2. Set the data type of the `record` attribute to `Record`.

### Step 3: Add Relevant User Inputs to the Streamlit Interface

Update Streamlit code. Create input areas to capture the sender, receiver, and amount for each transaction that you’ll store in the `Block` record.

1. Delete the `input_data` variable from the Streamlit interface.

2. Add an input area where you can get a value for `sender` from the user.

3. Add an input area where you can get a value for `receiver` from the user.

4. Add an input area where you can get a value for `amount` from the user.

5. As part of the “Add Block” button functionality, update `new_block` so that `Block` consists of an attribute named `record`, which is set equal to a `Record` that contains the `sender`, `receiver`, and `amount` values. The updated `Block` should also include the attributes for `creator_id` and `prev_hash`.

### Step 4: Test the PyChain Ledger by Storing Records

Run it in Streamlit.

1. Enter values for the sender, receiver, and amount, and then click the Add Block button. Do this several times to store several blocks in the ledger.
2. Verify the block contents and hashes in the Streamlit dropdown menu. Take a screenshot.

3. Test the blockchain validation process by using the web interface. Take a screenshot.

## Submission

Upload to GitHub.

* Make sure to update the `README.md` file to **include an explanation of the Steamlit application**, a s**creenshot or video of your deployed Streamlit** application, and any other information that’s needed to interact with your project.

* Submit the link to your GitHub project to Bootcamp Spot.

---

© 2021 Trilogy Education Services, a 2U, Inc. brand. All Rights Reserved.
