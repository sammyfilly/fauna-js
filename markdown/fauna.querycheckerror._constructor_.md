<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [fauna](./fauna.md) &gt; [QueryCheckError](./fauna.querycheckerror.md) &gt; [(constructor)](./fauna.querycheckerror._constructor_.md)

## QueryCheckError.(constructor)

Constructs a new instance of the `QueryCheckError` class

<b>Signature:</b>

```typescript
constructor(error: {
        code: string;
        message: string;
        httpStatus: 400;
        summary?: string;
        failures: QueryCheckFailure[];
    });
```

## Parameters

| Parameter | Type                                                                                                                                           | Description |
| --------- | ---------------------------------------------------------------------------------------------------------------------------------------------- | ----------- |
| error     | { code: string; message: string; httpStatus: 400; summary?: string; failures: [QueryCheckFailure](./fauna.querycheckfailure.md)<!-- -->\[\]; } |             |