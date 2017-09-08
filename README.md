# Roy Lee Kiat - Validate NRIC Chatbot implementation in Python

This is an NRIC Validation implementation that gets Api.ai classification JSON (i.e. a JSON output of Api.ai /query endpoint) and returns a fulfillment response.

# What does the service do?
It's a NRIC Validity fulfillment service that takes in an NRIC number where both alphabets have to be in capital letter.
The services takes the `NRIC` parameter from the action, are returns a validity status to Api.ai.

The service packs the result in the Api.ai webhook-compatible response JSON and returns it to Api.ai.

