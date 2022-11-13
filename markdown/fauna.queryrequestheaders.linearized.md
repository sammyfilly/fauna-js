<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [fauna](./fauna.md) &gt; [QueryRequestHeaders](./fauna.queryrequestheaders.md) &gt; [linearized](./fauna.queryrequestheaders.linearized.md)

## QueryRequestHeaders.linearized property

If true, unconditionally run the query as strictly serialized. This affects read-only transactions. Transactions which write will always be strictly serialized. Overrides the optional setting for the client.

<b>Signature:</b>

```typescript
linearized?: boolean;
```