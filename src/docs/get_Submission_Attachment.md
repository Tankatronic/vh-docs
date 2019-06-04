# **GET**  /tenants/{tenantId}/forms/{formId}/submissions/{submissionId}/attachments/{attachmentName}

## __Request Parameters__

### Path Parameters

   | Property     | Description          | Type     | Format | Is Required |
   | ------------ | -------------------- | -------- | ------ | ----------- |
   | tenantId     | The ID of the tenant | _string_ | guid   | ✔           |
   | FormId       |                      | _string_ | guid   | ✔           |
   | submissionId |                      | _string_ | guid   | ✔           |
   | attachmentName |                      | _string_ |    | ✔           |

## __Responses__

### __200__

### Schema

| Property     | Description | Type          | Format | Is Required |
| ------------ | ----------- | ------------- | ------ | ----------- |
| _object_     |             |               |        |             |

## 400

See [Error's response page](errors.md)

##### Examples

Example of "innererror":

## __Test Requests__

```cURL tab= 
Example1
```

```C# tab=
Example2
```

## __Test Responses__

```cURL tab= 
Example1
```

```C# tab=
Example2
```
