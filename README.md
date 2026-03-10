# kromerTapToPay

A simple NFC payment standard that allows shops to communicate payment
information to a pocket computer using an NFC reader with the simple goal
of improving user experience through a quick payment method. 

# Data Format

The NFC payload contains a string with the following format:

address|amount|meta

Each field is separated by a pipe (|)

Fields:
- address: Where the Kromer should be sent
- amount: The amount of Kromer required for the transaction.
- meta: Optional metadata for the transaction

Rules:
- The address and amount fields MUST be present.
- The meta field MAY be empty.
- The meta field MUST NOT contain pipes (|).
  
Example:

k93figka3|0.25|diamond
