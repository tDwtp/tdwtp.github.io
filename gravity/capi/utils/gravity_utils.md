# `gravity_utils.h`


## Types

### `nanotime_t`
A type capabale of holding the time in nanoseconds.

## Functions

### `nanotime`
```c
nanotime_t nanotime (void);
```
### `microtime`
```c
double microtime (nanotime_t tstart, nanotime_t tend);
```
### `millitime`
```c
double millitime (nanotime_t tstart, nanotime_t tend);
```

### `file_size`
```c
int64_t file_size (const char *path);
```
### `file_exists`
```c
bool file_exists (const char *path);
```
### `file_delete`
```c
bool file_delete (const char *path);
```
### `file_read`
```c
char *file_read (const char *path, size_t *len);
```
### `file_write`
```c
bool file_write (const char *path, const char *buffer, size_t len);
```
### `file_buildpath`
```c
char *file_buildpath (const char *filename, const char *dirpath);
```
### `file_name_frompath`
```c
char *file_name_frompath (const char *path);
```

### `is_directory`
```c
bool is_directory (const char *path);
```
### `directory_create`
```c
bool directory_create (const char *path);
```
### `directory_init`
```c
DIRREF directory_init (const char *path);
```
### `directory_read`
```c
char *directory_read (DIRREF ref, char *win32buffer);
```
### `directory_read_extend`
```c
char *directory_read_extend (DIRREF ref, char *win32buffer);
```

### `string_nocasencmp`
```c
int string_nocasencmp (const char *s1, const char *s2, size_t n);
```
### `string_casencmp`
```c
int string_casencmp (const char *s1, const char *s2, size_t n);
```
### `string_cmp`
```c
int string_cmp (const char *s1, const char *s2);
```
### `string_dup`
```c
char *string_dup (const char *s1);
```
### `string_ndup`
```c
char *string_ndup (const char *s1, size_t n);
```
### `string_reverse`
```c
void string_reverse (char *p);
```
### `string_size`
```c
uint32_t string_size (const char *p);
```
### `string_strnstr`
```c
char *string_strnstr (const char *s, const char *find, size_t slen);
```
### `string_replace`
```c
char *string_replace (const char *str, const char *from, const char *to, size_t *rlen);
```

### `utf8_charbytes`
```c
uint32_t utf8_charbytes (const char *s, uint32_t i);
```
### `utf8_nbytes`
```c
uint32_t utf8_nbytes (uint32_t n);
```
### `utf8_encode`
```c
uint32_t utf8_encode (char *buffer, uint32_t value);
```
### `utf8_len`
```c
uint32_t utf8_len (const char *s, uint32_t nbytes);
```
### `utf8_reverse`
```c
bool utf8_reverse (char *p);
```

### `power_of2_ceil`
```c
uint32_t power_of2_ceil (uint32_t n);
```
### `number_from_hex`
```c
int64_t number_from_hex (const char *s, uint32_t len);
```
### `number_from_oct`
```c
int64_t number_from_oct (const char *s, uint32_t len);
```
### `number_from_bin`
```c
int64_t number_from_bin (const char *s, uint32_t len);
```
