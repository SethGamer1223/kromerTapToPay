# kromerTapToPay

A simple NFC payment standard allowing shops to communicate payment
information to a pocket computer using an NFC reader.

# Data Format

The NFC payload contains string with the following format:

address;amount;meta

Each field is separated by a semicolon (;)

Fields:
- address: Where the kromer should be sent
- amount: The amount of Kromer required for the transaction.
- meta: Optional metadata for the transaction

The address and amount fields MUST be present.
The meta field MAY be empty.
When parsing the meta field everything after meta MUST be parsed as a string


Example:

k93figka30;0.25;diamond
