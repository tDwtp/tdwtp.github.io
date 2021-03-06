# Gravity C API Reference

This is a reference documentation of the C API. For a tutorial on how to extend
or embed Gravity, visit the [Guide](/guide/).

## Commonly used headers

* [`runtime/gravity_vm.h`](/capi/runtime/gravity_vm.md)
* [`runtime/gravity_vmmacros.h`](/capi/runtime/gravity_vmmacros.md)
* [`shared/gravity_value.h`](/capi/shared/gravity_value.md)
* [`runtime/gravity_core.h`](/capi/runtime/gravity_core.md)
* [`shared/gravity_array.h`](/capi/shared/gravity_array.md)
* [`utils/gravity_json.h`](/capi/utils/gravity_json.md)
* [`utils/gravity_utils.h`](/capi/utils/gravity_utils.md)
* [`shared/gravity_delegate.h`](/capi/shared/gravity_delegate.md)



## List of files and directories

* [`compiler`](/capi/compiler.md)
  * [`debug_macros.h`](/capi/compiler/debug_macros.md)
  * [`gravity_ast.h`](/capi/compiler/gravity_ast.md)
  * [`gravity_codegen.h`](/capi/compiler/gravity_codegen.md)
  * [`gravity_compiler.h`](/capi/compiler/gravity_compiler.md)
  * [`gravity_ircode.h`](/capi/compiler/gravity_ircode.md)
  * [`gravity_lexer.h`](/capi/compiler/gravity_lexer.md)
  * [`gravity_optimizer.h`](/capi/compiler/gravity_optimizer.md)
  * [`gravity_parser.h`](/capi/compiler/gravity_parser.md)
  * [`gravity_semacheck1.h`](/capi/compiler/gravity_semacheck1.md)
  * [`gravity_semacheck2.h`](/capi/compiler/gravity_semacheck2.md)
  * [`gravity_token.h`](/capi/compiler/gravity_token.md)
  * [`gravity_visitor.h`](/capi/compiler/gravity_visitor.md)
* [`optionals`](/capi/optionals.md)
  * [`gravity_opt_env.h`](/capi/optionals/gravity_opt_env.md)
  * [`gravity_opt_file.h`](/capi/optionals/gravity_opt_file.md)
  * [`gravity_opt_json.h`](/capi/optionals/gravity_opt_json.md)
  * [`gravity_opt_math.h`](/capi/optionals/gravity_opt_math.md)
  * [`gravity_optionals.h`](/capi/optionals/gravity_optionals.md)
* [`runtime`](/capi/runtime.md)
  * [`gravity_core.h`](/capi/runtime/gravity_core.md)
  * [`gravity_vm.h`](/capi/runtime/gravity_vm.md)
  * [`gravity_vmmacros.h`](/capi/runtime/gravity_vmmacros.md)
* [`shared`](/capi/shared.md)
  * [`gravity_array.h`](/capi/shared/gravity_array.md)
  * [`gravity_config.h`](/capi/shared/gravity_config.md)
  * [`gravity_delegate.h`](/capi/shared/gravity_delegate.md)
  * [`gravity_hash.h`](/capi/shared/gravity_hash.md)
  * [`gravity_macros.h`](/capi/shared/gravity_macros.md)
  * [`gravity_memory.h`](/capi/shared/gravity_memory.md)
  * [`gravity_opcodes.h`](/capi/shared/gravity_opcodes.md)
  * [`gravity_value.h`](/capi/shared/gravity_value.md)
* [`utils`](/capi/utils.md)
  * [`gravity_debug.h`](/capi/utils/gravity_debug.md)
  * [`gravity_json.h`](/capi/utils/gravity_json.md)
  * [`gravity_utils.h`](/capi/utils/gravity_utils.md)