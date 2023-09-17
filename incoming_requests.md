# Incoming Requests
These are the requests the receiving school is making.

## Data Model

```mermaid
erDiagram
    Requests ||--|{ PayloadContents : has
    Requests {
        guid RequestId
        text RequestDetails
        datetime RequestDate
        guid EducationOrganizationId
        guid ProcessUserId
        text Student
        enum RequestStatus
    }
    PayloadContents {
        guid PayloadContentId
        guid RequestId
        text ContentType
        byte BlobContent
        json JsonContent
        xml XmlContent
    }
```

## Persistence
* Incoming requests are persisted in the `IncomingRequests` table.
* Their counterpart in the sending school's broker are persisted in the `OutgoingRequests` table.

From the perspective of the broker itself, records in the IncomingRequests table represent new students coming in and records in the OutgoingRequests table represent students that are leaving it.

When the receiving records clerk makes the initial incoming request, that record is persisted in IncomingRequests. After the receiving school's broker transmits the request to the sending school's broker, the sending schoo's broker will persist the request in OutgoingRequests.
