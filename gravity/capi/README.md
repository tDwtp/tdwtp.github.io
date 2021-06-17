# Gravity C API Reference

This is a reference documentation of the C API. For a tutorial on how to extend
or embed Gravity, visit the [Guide](/gravity/guide/).

## Commonly used headders

* [`shared/gravity_delegate.h`](shared/gravity_delegate.md)
* [`shared/gravity_value.h`](shared/gravity_value.md)
* [`utils/gravity_json.h`](utils/gravity_json.md)
* [`utils/gravity_utils.h`](utils/gravity_utils.md)
* [`shared/gravity_array.h`](shared/gravity_array.md)
* [`runtime/gravity_core.h`](runtime/gravity_core.md)
* [`runtime/gravity_vm.h`](runtime/gravity_vm.md)
* [`runtime/gravity_vmmacros.h`](runtime/gravity_vmmacros.md)



## List of files and directories

* [`compiler`](compiler.md)
  * [`compiler/debug_macros.h`]( compiler/debug_macros.md)
  * [`compiler/gravity_ast.h`]( compiler/gravity_ast.md)
  * [`compiler/gravity_codegen.h`]( compiler/gravity_codegen.md)
  * [`compiler/gravity_compiler.h`]( compiler/gravity_compiler.md)
  * [`compiler/gravity_ircode.h`]( compiler/gravity_ircode.md)
  * [`compiler/gravity_lexer.h`]( compiler/gravity_lexer.md)
  * [`compiler/gravity_optimizer.h`]( compiler/gravity_optimizer.md)
  * [`compiler/gravity_parser.h`]( compiler/gravity_parser.md)
  * [`compiler/gravity_semacheck1.h`]( compiler/gravity_semacheck1.md)
  * [`compiler/gravity_semacheck2.h`]( compiler/gravity_semacheck2.md)
  * [`compiler/gravity_token.h`]( compiler/gravity_token.md)
  * [`compiler/gravity_visitor.h`]( compiler/gravity_visitor.md)
* [`optionals`](optionals.md)
  * [`optionals/gravity_opt_env.h`](optionals/gravity_opt_env.md)
  * [`optionals/gravity_opt_file.h`](optionals/gravity_opt_file.md)
  * [`optionals/gravity_opt_json.h`](optionals/gravity_opt_json.md)
  * [`optionals/gravity_opt_math.h`](optionals/gravity_opt_math.md)
  * [`optionals/gravity_optionals.h`](optionals/gravity_optionals.md)
* [`runtime`](runtime.md)
  * [`runtime/gravity_core.h`](runtime/gravity_core.md)
  * [`runtime/gravity_vm.h`](runtime/gravity_vm.md)
  * [`runtime/gravity_vmmacros.h`](runtime/gravity_vmmacros.md)
* [`shared`](shared.md)
  * [`shared/gravity_array.h`](shared/gravity_array.md)
  * [`shared/gravity_config.h`](shared/gravity_config.md)
  * [`shared/gravity_delegate.h`](shared/gravity_delegate.md)
  * [`shared/gravity_hash.h`](shared/gravity_hash.md)
  * [`shared/gravity_macros.h`](shared/gravity_macros.md)
  * [`shared/gravity_memory.h`](shared/gravity_memory.md)
  * [`shared/gravity_opcodes.h`](shared/gravity_opcodes.md)
  * [`shared/gravity_value.h`](shared/gravity_value.md)
* [`utils`]( utils.md)
  * [`utils/gravity_debug.h`](utils/gravity_debug.md)
  * [`utils/gravity_json.h`](utils/gravity_json.md)
  * [`utils/gravity_utils.h`](utils/gravity_utils.md)