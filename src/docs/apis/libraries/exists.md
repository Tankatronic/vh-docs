# **GET**   /libraries/{libraryId}/cmd/exists

TODO

## Request

### Query Parameters

| Name | Type | Format | Required | Description |
| ---- | ---- | ------ | -------- | ----------- |
--8<-- "_partials/schemas/path_param.md"
--8<-- "_partials/schemas/tenantId_param.md"

### Path Parameters

| Name | Type | Format | Required | Description |
| ---- | ---- | ------ | -------- | ----------- |
--8<-- "_partials/schemas/libraryId_param.md"

## Responses

### HTTP 200

#### Response Schema

| Name     | Type      | Format | Required | Description |
| -------- | --------- | ------ | -------- | ----------- |
| `exists` | _boolean_ |        | ✔        |             |

### HTTP 400

--8<-- "_partials/schemas/error.md"

## Examples

### Requests

!!! note
    Authentication is not shown in these examples. For details refer to the [Authentication](../auth.md) page.

=== "cURL"

    ```bash
    curl --location --request GET 'https://api.vendorhub.io/libraries/d31d18d9-43d6-4ab5-a10a-bd39402c1fb2/cmd/exists?path=/test.txt&api-version=2019-09-01'
    ```

=== "C#"

    ```csharp
    IDocumentLibraryClient client = ...;
    Guid libraryId = Guid.Parse("d31d18d9-43d6-4ab5-a10a-bd39402c1fb2");
    ExistsResponse exists = await client.ExistsAsync(libraryId, "/test.txt");
    ```

=== "C# (Raw)"

    ```csharp
    HttpClient httpClient = new HttpClient();
    string url = "https://api.vendorhub.io/libraries/d31d18d9-43d6-4ab5-a10a-bd39402c1fb2/cmd/exists?path=/test.txt&api-version=2019-09-01";
    HttpResponseMessage response = await httpClient.GetAsync(url);
    ```

### Response

```json
{
    "exists": true
}
```
