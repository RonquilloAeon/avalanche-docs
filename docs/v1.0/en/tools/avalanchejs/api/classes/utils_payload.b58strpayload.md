[avalanche](../README.md) › [Utils-Payload](../modules/utils_payload.md) › [B58STRPayload](utils_payload.b58strpayload.md)

# Class: B58STRPayload

Class for payloads representing Base58 encoding.

## Hierarchy

* [PayloadBase](utils_payload.payloadbase.md)

  ↳ **B58STRPayload**

  ↳ [SECPSIGPayload](utils_payload.secpsigpayload.md)

  ↳ [SECPENCPayload](utils_payload.secpencpayload.md)

  ↳ [IPFSPayload](utils_payload.ipfspayload.md)

## Index

### Constructors

* [constructor](utils_payload.b58strpayload.md#constructor)

### Properties

* [payload](utils_payload.b58strpayload.md#protected-payload)
* [typeid](utils_payload.b58strpayload.md#protected-typeid)

### Methods

* [fromBuffer](utils_payload.b58strpayload.md#frombuffer)
* [getContent](utils_payload.b58strpayload.md#getcontent)
* [getPayload](utils_payload.b58strpayload.md#getpayload)
* [returnType](utils_payload.b58strpayload.md#returntype)
* [toBuffer](utils_payload.b58strpayload.md#tobuffer)
* [typeID](utils_payload.b58strpayload.md#typeid)
* [typeName](utils_payload.b58strpayload.md#typename)

## Constructors

###  constructor

\+ **new B58STRPayload**(`payload`: any): *[B58STRPayload](utils_payload.b58strpayload.md)*

*Overrides [PayloadBase](utils_payload.payloadbase.md).[constructor](utils_payload.payloadbase.md#constructor)*

*Defined in [src/utils/payload.ts:323](https://github.com/ava-labs/avalanchejs/blob/a2feb77/src/utils/payload.ts#L323)*

**Parameters:**

Name | Type | Default | Description |
------ | ------ | ------ | ------ |
`payload` | any | undefined | Buffer or cb58 encoded string  |

**Returns:** *[B58STRPayload](utils_payload.b58strpayload.md)*

## Properties

### `Protected` payload

• **payload**: *Buffer* = Buffer.alloc(0)

*Inherited from [PayloadBase](utils_payload.payloadbase.md).[payload](utils_payload.payloadbase.md#protected-payload)*

*Defined in [src/utils/payload.ts:166](https://github.com/ava-labs/avalanchejs/blob/a2feb77/src/utils/payload.ts#L166)*

___

### `Protected` typeid

• **typeid**: *number* = 3

*Overrides [PayloadBase](utils_payload.payloadbase.md).[typeid](utils_payload.payloadbase.md#protected-typeid)*

*Defined in [src/utils/payload.ts:316](https://github.com/ava-labs/avalanchejs/blob/a2feb77/src/utils/payload.ts#L316)*

## Methods

###  fromBuffer

▸ **fromBuffer**(`bytes`: Buffer, `offset`: number): *number*

*Inherited from [PayloadBase](utils_payload.payloadbase.md).[fromBuffer](utils_payload.payloadbase.md#frombuffer)*

*Defined in [src/utils/payload.ts:204](https://github.com/ava-labs/avalanchejs/blob/a2feb77/src/utils/payload.ts#L204)*

Decodes the payload as a [Buffer](https://github.com/feross/buffer) including 4 bytes for the length and TypeID.

**Parameters:**

Name | Type | Default |
------ | ------ | ------ |
`bytes` | Buffer | - |
`offset` | number | 0 |

**Returns:** *number*

___

###  getContent

▸ **getContent**(): *Buffer*

*Inherited from [PayloadBase](utils_payload.payloadbase.md).[getContent](utils_payload.payloadbase.md#getcontent)*

*Defined in [src/utils/payload.ts:186](https://github.com/ava-labs/avalanchejs/blob/a2feb77/src/utils/payload.ts#L186)*

Returns the payload content (minus typeID).

**Returns:** *Buffer*

___

###  getPayload

▸ **getPayload**(): *Buffer*

*Inherited from [PayloadBase](utils_payload.payloadbase.md).[getPayload](utils_payload.payloadbase.md#getpayload)*

*Defined in [src/utils/payload.ts:194](https://github.com/ava-labs/avalanchejs/blob/a2feb77/src/utils/payload.ts#L194)*

Returns the payload (with typeID).

**Returns:** *Buffer*

___

###  returnType

▸ **returnType**(): *string*

*Overrides [PayloadBase](utils_payload.payloadbase.md).[returnType](utils_payload.payloadbase.md#abstract-returntype)*

*Defined in [src/utils/payload.ts:321](https://github.com/ava-labs/avalanchejs/blob/a2feb77/src/utils/payload.ts#L321)*

Returns a base58 string for the payload.

**Returns:** *string*

___

###  toBuffer

▸ **toBuffer**(): *Buffer*

*Inherited from [PayloadBase](utils_payload.payloadbase.md).[toBuffer](utils_payload.payloadbase.md#tobuffer)*

*Defined in [src/utils/payload.ts:217](https://github.com/ava-labs/avalanchejs/blob/a2feb77/src/utils/payload.ts#L217)*

Encodes the payload as a [Buffer](https://github.com/feross/buffer) including 4 bytes for the length and TypeID.

**Returns:** *Buffer*

___

###  typeID

▸ **typeID**(): *number*

*Inherited from [PayloadBase](utils_payload.payloadbase.md).[typeID](utils_payload.payloadbase.md#typeid)*

*Defined in [src/utils/payload.ts:172](https://github.com/ava-labs/avalanchejs/blob/a2feb77/src/utils/payload.ts#L172)*

Returns the TypeID for the payload.

**Returns:** *number*

___

###  typeName

▸ **typeName**(): *string*

*Inherited from [PayloadBase](utils_payload.payloadbase.md).[typeName](utils_payload.payloadbase.md#typename)*

*Defined in [src/utils/payload.ts:179](https://github.com/ava-labs/avalanchejs/blob/a2feb77/src/utils/payload.ts#L179)*

Returns the string name for the payload's type.

**Returns:** *string*