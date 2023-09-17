# Incoming Requests
These are the requests the receiving school is making.

## Example Record Before Request Transmission
This is the `Request` record state before the request is to be transmitted to the sending school.
```json
{
    "RequestId": "fd60c580-aaa5-4319-9aba-9362cfee29ec",
    "EducationOrganizationId": "aba6d628-257d-4444-810f-2a9509161434",
    "Student": {
        "OregonNexus.Broker.Connector.EdFiAlliance.EdFi.Student": {
            "id": "000000",
            "studentUniqueId": "0000000",
            "firstName": "John",
            "middleName": "T",
            "lastSurname": "Doe"
        }
    },
    "RequestManifest": {
        "RequestType": "OregonNexus.Broker.Connector.Payload.StudentCumulativeRecord",
        "Student": {
            "OregonNexus.Broker.Connector.EdFiAlliance.EdFi.Student": {
                "id": "000000",
                "studentUniqueId": "0000000",
                "firstName": "John",
                "middleName": "T",
                "lastSurname": "Doe"
            }
        },
        "From": {
            "District": "Washington School District",
            "School": "George High School",
            "Email": "registrar@washingtonsd.example"
        },
        "To": {
            "District": "Washington School District",
            "School": "George High School",
            "Email": "registrar@washingtonsd.example"
        },
        "Note": "Note to sending school's registrar.",
        "Contents": [
            "ParentRelease.pdf"
        ]
    },
    "RequestProcessUserId": "5b97e5a2-b39e-48b5-9dd3-97ef855bea22",
    "InitialRequestSentDate": "2023-09-11 05:03:20.462908+00",
    "ResponseManifest": null,
    "ResponseProcessUserId": null,
    "RequestStatus": 3
}
```
