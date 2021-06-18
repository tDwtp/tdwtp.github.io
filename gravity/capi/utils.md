# `utils`
Utility functions to help developers with some tasks.

- [gravity_debug](/capi/utils/gravity_debug.md)
- [gravity_json](/capi/utils/gravity_json.md)
- [gravity_utils](/capi/utils/gravity_utils.md)

## [`gravity_debug.h`](/capi/utils/gravity_debug.md)
Functions to help look into bytecode (serialized or not).

- [`opcode_constname`](/capi/utils/gravity_debug.md#opcode_constname)
- [`opcode_name`](/capi/utils/gravity_debug.md#opcode_name)
- [`gravity_disassemble`](/capi/utils/gravity_debug.md#gravity_disassemble)

## [`gravity_json.h`](/capi/utils/gravity_json.md)
A simple JSON interface used within Gravity.
- Types
  - [`json_opt_mask` (`enum`)](/capi/utils/gravity_json.md#json_opt_mask)
  - [`json_type` (`enum`)](/capi/utils/gravity_json.md#json_type)
  - [`json_settings` (`struct`)](/capi/utils/gravity_json.md#json_settings)
  - [`json_value` (`struct`)](/capi/utils/gravity_json.md#json_value)
  - [`json_t` (`struct`)](/capi/utils/gravity_json.md#json_t)

- Functions
  - Creation/Destruction/Parsing
    - [`json_new`](/capi/utils/gravity_json.md#json_new)
    - [`json_free`](/capi/utils/gravity_json.md#json_free)
    - [`json_parse`](/capi/utils/gravity_json.md#json_parse)
    - [`json_parse_ex`](/capi/utils/gravity_json.md#json_parse_ex)
    - [`json_value_free`](/capi/utils/gravity_json.md#json_value_free)
    - [`json_value_free_ex`](/capi/utils/gravity_json.md#json_value_free_ex)
  - Nesting
    - [`json_begin_array`](/capi/utils/gravity_json.md#json_begin_array)
    - [`json_begin_object`](/capi/utils/gravity_json.md#json_begin_object)
    - [`json_end_array`](/capi/utils/gravity_json.md#json_end_array)
    - [`json_end_object`](/capi/utils/gravity_json.md#json_end_object)
  - Entries
    - [`json_add_bool`](/capi/utils/gravity_json.md#json_add_bool)
    - [`json_add_cstring`](/capi/utils/gravity_json.md#json_add_cstring)
    - [`json_add_double`](/capi/utils/gravity_json.md#json_add_double)
    - [`json_add_int`](/capi/utils/gravity_json.md#json_add_int)
    - [`json_add_null`](/capi/utils/gravity_json.md#json_add_null)
    - [`json_add_string`](/capi/utils/gravity_json.md#json_add_string)
    - [`json_get_label`](/capi/utils/gravity_json.md#json_get_label)
    - [`json_set_label`](/capi/utils/gravity_json.md#json_set_label)
  - Buffers
    - [`json_buffer`](/capi/utils/gravity_json.md#json_buffer)
    - [`json_write_file`](/capi/utils/gravity_json.md#json_write_file)
  - options
    - [`json_clear_option`](/capi/utils/gravity_json.md#json_clear_option)
    - [`json_get_options`](/capi/utils/gravity_json.md#json_get_options)
    - [`json_option_isset`](/capi/utils/gravity_json.md#json_option_isset)
    - [`json_set_option`](/capi/utils/gravity_json.md#json_set_option)

## [`gravity_utils.h`](/capi/utils/gravity_utils.md)
This is a compendium for some utilities commonly used for interactions with or
for Gravity.  
Basic file/directory interactions are provided to easily expand I/O related
features or detection.  
Strings, their UTF-8 encoding and parsing strings to numbers (octal, decimal
and hexadecimals)  
Time-functions and an simple `ceil(n^2)` function is provided as well.

- Time
  - [`nanotime`](/capi/utils/gravity_utils.md#nanotime)
  - [`microtime`](/capi/utils/gravity_utils.md#microtime)
  - [`millitime`](/capi/utils/gravity_utils.md#millitime)
- File
  - [`file_size`](/capi/utils/gravity_utils.md#file_size)
  - [`file_exists`](/capi/utils/gravity_utils.md#file_exists)
  - [`file_delete`](/capi/utils/gravity_utils.md#file_delete)
  - [`file_read`](/capi/utils/gravity_utils.md#file_read)
  - [`file_write`](/capi/utils/gravity_utils.md#file_write)
  - [`file_buildpath`](/capi/utils/gravity_utils.md#file_buildpath)
  - [`file_name_frompath`](/capi/utils/gravity_utils.md#file_name_frompath)
- Directory
  - [`directory_create`](/capi/utils/gravity_utils.md#directory_create)
  - [`directory_init`](/capi/utils/gravity_utils.md#directory_init)
  - [`directory_read`](/capi/utils/gravity_utils.md#directory_read)
  - [`directory_read_extend`](/capi/utils/gravity_utils.md#directory_read_extend)
  - [`is_directory`](/capi/utils/gravity_utils.md#is_directory)
- Math and Numbers
  - [`number_from_hex`](/capi/utils/gravity_utils.md#number_from_hex)
  - [`number_from_oct`](/capi/utils/gravity_utils.md#number_from_oct)
  - [`number_from_bin`](/capi/utils/gravity_utils.md#number_from_bin)
  - [`power_of2_ceil`](/capi/utils/gravity_utils.md#power_of2_ceil)
- Strings
  - [`string_nocasencmp`](/capi/utils/gravity_utils.md#string_nocasencmp)
  - [`string_casencmp`](/capi/utils/gravity_utils.md#string_casencmp)
  - [`string_cmp`](/capi/utils/gravity_utils.md#string_cmp)
  - [`string_dup`](/capi/utils/gravity_utils.md#string_dup)
  - [`string_ndup`](/capi/utils/gravity_utils.md#string_ndup)
  - [`string_reverse`](/capi/utils/gravity_utils.md#string_reverse)
  - [`string_size`](/capi/utils/gravity_utils.md#string_size)
  - [`string_strnstr`](/capi/utils/gravity_utils.md#string_strnstr)
  - [`string_replace`](/capi/utils/gravity_utils.md#string_replace)
- UTF-8
  - [`utf8_charbytes`](/capi/utils/gravity_utils.md#utf8_charbytes)
  - [`utf8_nbytes`](/capi/utils/gravity_utils.md#utf8_nbytes)
  - [`utf8_encode`](/capi/utils/gravity_utils.md#utf8_encode)
  - [`utf8_len`](/capi/utils/gravity_utils.md#utf8_len)
  - [`utf8_reverse`](/capi/utils/gravity_utils.md#utf8_reverse)
