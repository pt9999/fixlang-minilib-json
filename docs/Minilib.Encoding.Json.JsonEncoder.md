# Minilib.Encoding.Json.JsonEncoder

Defined in minilib-json@0.5.1

Encodes a JSON value to a string.

## Values

### namespace Minilib.Encoding.Json.JsonEncoder

#### _encode

Type: `Minilib.Encoding.Json.JsonEncoder::EncodeParam -> Std::Array Std::String -> Minilib.Encoding.Json::Json -> Std::Array Std::String`

#### _encode_array

Type: `Minilib.Encoding.Json.JsonEncoder::EncodeParam -> Std::Array Std::String -> Std::Array Minilib.Encoding.Json::Json -> Std::Array Std::String`

#### _encode_number

Type: `Minilib.Encoding.Json.JsonEncoder::EncodeParam -> Std::F64 -> Std::String`

#### _encode_object

Type: `Minilib.Encoding.Json.JsonEncoder::EncodeParam -> Std::Array Std::String -> Minilib.Collection.OrderedMap::OrderedMap Std::String Minilib.Encoding.Json::Json -> Std::Array Std::String`

#### _encode_string

Type: `Std::String -> Std::String`

#### _escape_table

Type: `Std::Array Std::U8`

#### _hex_table

Type: `Std::Array Std::U8`

#### encode

Type: `Minilib.Encoding.Json::Json -> Std::String`

Encodes JSON and converts it to a string.

#### encode_pretty

Type: `Minilib.Encoding.Json::Json -> Std::String`

Encodes JSON and converts it to a string. (pretty-printing)

#### encode_with_param

Type: `Minilib.Encoding.Json.JsonEncoder::EncodeParam -> Minilib.Encoding.Json::Json -> Std::String`

Encodes JSON and converts it to a string using the specified parameter.

### namespace Minilib.Encoding.Json.JsonEncoder::EncodeParam

#### default

Type: `Minilib.Encoding.Json.JsonEncoder::EncodeParam`

#### increment_indent

Type: `Minilib.Encoding.Json.JsonEncoder::EncodeParam -> Minilib.Encoding.Json.JsonEncoder::EncodeParam`

#### pretty_print

Type: `Minilib.Encoding.Json.JsonEncoder::EncodeParam`

## Types and aliases

### namespace Minilib.Encoding.Json.JsonEncoder

#### EncodeParam

Defined as: `type EncodeParam = unbox struct { ...fields... }`

##### field `space`

Type: `Std::String`

##### field `newline`

Type: `Std::String`

##### field `indent`

Type: `Std::String`

##### field `indent_incr`

Type: `Std::String`

##### field `number_prec`

Type: `Std::U8`

## Traits and aliases

## Trait implementations