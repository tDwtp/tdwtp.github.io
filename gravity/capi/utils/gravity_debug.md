

## `opcode_constname`
```c
const char *opcode_constname (int n);
```
Return the name of a given constant.
<dl>
<dt>`n` *(`int`)*
<dd>The value a constant inside constant pool can have.
</dl>

See [`CPOOL_VALUE_*`](/shared/gravity_value.md#CPOOL) for a list of possible values for `n`.

## `opcode_name`
```c
const char *opcode_name (opcode_t op);
```
Returns the name of a given opcode.
<dl>
<dt>`op` *([opcode_t](/shared/graity_opcode.md#opcode_t))*
<dd>opcode to be translated
</dl>


See [opcode_t](/shared/graity_opcode.md#opcode_t) for more details

## `gravity_disassemble`
`const char *gravity_disassemble (gravity_vm *vm, gravity_function_t *f, const char *bcode, uint32_t blen, bool deserialize);`
<dl>
<dt>`vm` *([gravity_vm](/runtime/graity_vm.md#vm))*
<dd>Source of constants when dumping code.
<dt>`bcode` *(`const char*`)*
<dd>A serialized string of ascii-hexadecimal digits as used in the json format for compiled code. 
Otherwise an uint32_t array containing the plain bytecode.
<dt>`blen` *(`uint32_t`)*
<dd>char-count of `bcode` in serialized form or the instruction-count if `bcode` is an uint32_t array of instructions.
<dt>`deserialize` *(`bool`)*
<dd>`true` if bcode is a string of ascii-hexadecimals as used in the json format for compiled code.  
`false` if bytecode is already an uint32_t array containing the palin bytecode.
</dl>

### 
