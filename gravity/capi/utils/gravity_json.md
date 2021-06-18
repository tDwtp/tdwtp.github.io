# `gravity_json.h`


## Types

### `json_opt_mask`
`enum`

### `json_type`
`enum`

### `json_settings`
`struct`

### `json_value`
`struct`

### `json_t`
`struct`

## Functions

### `json_new`
```c
json_t      *json_new (void);
```
### `json_free`
```c
void        json_free (json_t *json);
```

### `json_begin_object`
```c
void        json_begin_object (json_t *json, const char *key);
```
### `json_end_object`
```c
void        json_end_object (json_t *json);
```
### `json_begin_array`
```c
void        json_begin_array (json_t *json, const char *key);
```
### `json_end_array`
```c
void        json_end_array (json_t *json);
```
### `json_add_cstring`
```c
void        json_add_cstring (json_t *json, const char *key, const char *value);
```
### `json_add_string`
```c
void        json_add_string (json_t *json, const char *key, const char *value, size_t len);
```
### `json_add_int`
```c
void        json_add_int (json_t *json, const char *key, int64_t value);
```
### `json_add_double`
```c
void        json_add_double (json_t *json, const char *key, double value);
```
### `json_add_bool`
```c
void        json_add_bool (json_t *json, const char *key, bool value);
```
### `json_add_null`
```c
void        json_add_null (json_t *json, const char *key);
```
### `json_set_label`
```c
void        json_set_label (json_t *json, const char *key);
```
### `char`
```c
const char  *json_get_label (json_t *json, const char *key);
```

### `json_buffer`
```c
char        *json_buffer (json_t *json, size_t *len);
```
### `json_write_file`
```c
bool        json_write_file (json_t *json, const char *path);
```

### `json_get_options`
```c
uint32_t    json_get_options (json_t *json);
```
### `json_set_option`
```c
void        json_set_option (json_t *json, json_opt_mask option_value);
```
### `json_clear_option`
```c
void        json_clear_option (json_t *json, json_opt_mask option_value);
```
### `json_option_isset`
```c
bool        json_option_isset (json_t *json, json_opt_mask option_value);
```


### `json_parse`
```c
json_value * json_parse (const json_char * json, size_t length);
```

### `json_parse_ex`
```c
json_value * json_parse_ex (json_settings * settings, const json_char * json, size_t length, char * error);
```
#define json_error_max 128

### `json_value_free`
```c
void json_value_free (json_value *);
```


/* Not usually necessary, unless you used a custom mem_alloc and now want to
 * use a custom mem_free.
 */
### `json_value_free_ex`
```c
void json_value_free_ex (json_settings * settings, json_value *);
```