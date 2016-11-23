# EIP Frameworks comparison

## Application flow diagram

![Send confirmation email flow][flow-diagram]

[flow-diagram]: eip-frameworks-resources/doc/SendConfirmationMailFlow.png

## Running the application

### Spring Integration

1. Check the email settings in the OrderConfirmationFlowConfiguration class
2. Build the application war and deploy it to your favourite servlet container
3. Use Curl too POST the request (use appropriate host name and port if needed):

```curl -i -H "Content-Type: text/xml; charset=UTF-8" -X POST -T order.xml http://localhost:8080/eip-frameworks-spring-integration/order/confirmation```