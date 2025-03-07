# Minilib.Encoding.Json.JsonDecoder

Defined in minilib-json@0.5.1

Decodes a JSON value from a string.

## Values

### namespace Minilib.Encoding.Json.JsonDecoder

#### _DOUBLEQUOTE

Type: `Std::U8`

#### _begin_array

Type: `Minilib.Text.SimpleParser::Parser ()`

#### _begin_object

Type: `Minilib.Text.SimpleParser::Parser ()`

#### _end_array

Type: `Minilib.Text.SimpleParser::Parser ()`

#### _end_object

Type: `Minilib.Text.SimpleParser::Parser ()`

#### _json_text

Type: `Minilib.Text.SimpleParser::Parser Minilib.Encoding.Json::Json`

#### _match_quoted_char_u16

Type: `Minilib.Text.SimpleParser::Parser Std::U16`

Parse a quoted character. ("\n", "\uD83D" etc.)
NOTE: Escape sequences of the form "\uXXXX" can only represent
the range U+0000 to U+FFFF. Characters in the range U+10000 to U+10FFFF
become surrogate pairs and are split like "\uD83D\uDE38".
Therefore, we first interpret these strings as UTF16. Later convert it
to UTF32 and join the surrogate pair, then convert it to UTF8.

#### _match_quoted_str

Type: `Minilib.Text.SimpleParser::Parser Std::String`

#### _match_str_inner

Type: `Minilib.Text.SimpleParser::Parser Std::String`

#### _match_unquoted_char

Type: `Minilib.Text.SimpleParser::Parser Std::U8`

#### _match_unquoted_str

Type: `Minilib.Text.SimpleParser::Parser Std::String`

#### _name_separator

Type: `Minilib.Text.SimpleParser::Parser ()`

#### _parse_array

Type: `Minilib.Text.SimpleParser::Parser (Std::Array Minilib.Encoding.Json::Json)`

#### _parse_bool

Type: `Minilib.Text.SimpleParser::Parser Std::Bool`

#### _parse_null

Type: `Minilib.Text.SimpleParser::Parser ()`

#### _parse_number

Type: `Minilib.Text.SimpleParser::Parser Std::F64`

#### _parse_object

Type: `Minilib.Text.SimpleParser::Parser (Minilib.Collection.OrderedMap::OrderedMap Std::String Minilib.Encoding.Json::Json)`

#### _parse_string

Type: `Minilib.Text.SimpleParser::Parser Std::String`

#### _parse_value

Type: `Minilib.Text.SimpleParser::Parser Minilib.Encoding.Json::Json`

#### _unescape_table

Type: `Std::Array Std::U8`

#### _value_separator

Type: `Minilib.Text.SimpleParser::Parser ()`

#### _wrap_whitespaces

Type: `Minilib.Text.SimpleParser::Parser a -> Minilib.Text.SimpleParser::Parser a`

#### _ws

Type: `Minilib.Text.SimpleParser::Parser ()`

#### decode

Type: `Std::String -> Std::Result Std::ErrMsg Minilib.Encoding.Json::Json`

Parses JSON text and returns a JSON value.

## Types and aliases

## Traits and aliases

## Trait implementations