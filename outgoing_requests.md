# Outgoing Requests
These are the requests the sending school recevied.

## Example Record Before Request Transmission
This is the `Request` record state before the response is to be transmitted to the requesting school.
```json
{
    "RequestId": "fd60c580-aaa5-4319-9aba-9362cfee29ec",
    "EducationOrganizationId": "aba6d628-257d-4444-810f-2a9509161434",
    "Student": {
        "OregonNexus.Broker.Connector.EdFiAlliance.EdFi.Student": {
            "id": "000000",
            "studentUniqueId": "0000000"
        }
    },
    "RequestManifest": null
    "RequestProcessUserId": null,
    "ResponseManifest": {
        "RequestId": "fd60c580-aaa5-4319-9aba-9362cfee29ec",
        "ResponseType": "OregonNexus.Broker.Connector.Payload.StudentCumulativeRecord",
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
        "Note": "Note to receiving school's registrar.",
        "Contents": [
            "EdFiData.json",
            "StudentPermanentRecord.pdf",
            "OfficialTranscript.pdf"
        ]
    },
    "ResponseProcessUserId": "5b97e5a2-b39e-48b5-9dd3-97ef855bea22",
    "InitialSentDate": "2023-09-11 05:03:20.462908+00",
    "RequestStatus": 3
}
```
