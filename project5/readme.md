# Connect to and consume Azure services and thirdparty services
Resources used:
- Azure API Management (APIM)
- Azure Event Grid
- Azure Event Hub
- Azure Service Bus
- Azure Queue Storage queues

## Project - Event-Driven Bookstore Notification System
An event-driven bookstore appp that notifies subscribers when a new book is added to the inventory. This system integrates Azure's event-based and message-based solutions to handle the real-time notifications.

### Infrastructure used:
- Azure API Management (APIM): To manage and secure the API endpoints.
- Azure Event Grid: To trigger events when new books are added.
- Azure Service Bus: To send out notification messages to subscribers.
- Azure Cosmos DB: To store book inventory and subscriber details.

### Implementation guide
1. Initialize Azure API Management (APIM):
- Set up an APIM instance.
- Create and secure API endpoints to add books and register subscribers.
2. Design Bookstore Inventory System:
- Store new book entries in Azure Cosmos DB.
- When a book is added, trigger an event in Azure Event Grid.
3. Set Up Azure Event Grid:
- Configure it to watch for new book additions in Azure Cosmos DB.
4. Notification Mechanism with Azure Service Bus:
- When an event is triggered by a new book addition, push a notification message into Azure Service Bus.
- Subscribers will pull their notifications from here.
5. Subscriber Management in Azure Cosmos DB:
- Store details of subscribers.
- Maintain a list of books they are notified about, to prevent duplicate notifications.

### Additional info
Adding books and triggering events:
- when a book is added through the API, the data is stored in azure cosmos db.
- this addition triggers an event in azure event grid.

Notification to subcribers:
- azure event grid, upon capturing the event, instructs azure service bus to send out a notification.
- subscribers retrieve their notifications from azure service bus, ensuring they are informed of the new book.