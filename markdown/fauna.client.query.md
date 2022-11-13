<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [fauna](./fauna.md) &gt; [Client](./fauna.client.md) &gt; [query](./fauna.client.query.md)

## Client.query() method

Queries Fauna.

<b>Signature:</b>

```typescript
query<T = any>(request: QueryRequest | QueryBuilder, headers?: QueryRequestHeaders): Promise<QueryResponse<T>>;
```

## Parameters

| Parameter | Type                                                                               | Description                                                                                                                                                                                                                                                                                                       |
| --------- | ---------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| request   | [QueryRequest](./fauna.queryrequest.md) \| [QueryBuilder](./fauna.querybuilder.md) | a [QueryRequest](./fauna.queryrequest.md) or [QueryBuilder](./fauna.querybuilder.md) to build a request with. Note, you can embed header fields in this object; if you do that there's no need to pass the headers parameter.                                                                                     |
| headers   | [QueryRequestHeaders](./fauna.queryrequestheaders.md)                              | <i>(Optional)</i> optional [QueryRequestHeaders](./fauna.queryrequestheaders.md) to apply on top of the request input. Values in this headers parameter take precedence over the same values in the request parameter. This field is primarily intended to be used when you pass a QueryBuilder as the parameter. |

<b>Returns:</b>

Promise&lt;[QueryResponse](./fauna.queryresponse.md)<!-- -->&lt;T&gt;&gt;

Promise&amp;lt;[QueryResponse](./fauna.queryresponse.md)<!-- -->&amp;gt;.

## Exceptions

[ServiceError](./fauna.serviceerror.md) Fauna emitted an error. The ServiceError will be one of ServiceError's child classes if the error can be further categorized, or a concrete ServiceError if it cannot. ServiceError child types are , [AuthorizationError](./fauna.authorizationerror.md)<!-- -->, [QueryCheckError](./fauna.querycheckerror.md) [QueryRuntimeError](./fauna.queryruntimeerror.md)<!-- -->, [QueryTimeoutError](./fauna.querytimeouterror.md)<!-- -->, [ServiceInternalError](./fauna.serviceinternalerror.md) [ServiceTimeoutError](./fauna.servicetimeouterror.md)<!-- -->, [ThrottlingError](./fauna.throttlingerror.md)<!-- -->. You can use either the type, or the underlying httpStatus + code to determine the root cause.

[ProtocolError](./fauna.protocolerror.md) the client a HTTP error not sent by Fauna.

[NetworkError](./fauna.networkerror.md) the client encountered a network issue connecting to Fauna.

A [ClientError](./fauna.clienterror.md) the client fails to submit the request due to an internal error.