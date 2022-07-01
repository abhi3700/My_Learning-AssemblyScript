# FAQs

Q. Does AssemblyScript involve an interpreter, or a "VM in a VM"?

A. No, AssemblyScript compiles to WebAssembly bytecode directly, statically, ahead-of-time.

---

Q. What are the differences between AssemblyScript and TypeScript?

A. TypeScript transpiles down to JavaScript, a dynamic just-in-time compiled language. AssemblyScript, on the other hand, compiles to a static WebAssembly binary. Their compiler implementations are quite different. However, the two languages are so very similar on the surface that they share many concepts. For example, TypeScript tooling can be used to author and refactor AssemblyScript code and, with some effort, the same code base can be transpiled to JavaScript with tsc and compiled to WebAssembly with asc, or code shared. The AssemblyScript compiler itself is portable.

---

Q. Will AssemblyScript support all of TypeScript eventually?

A. It likely won't. While TypeScript adds typings to JavaScript, it is a superset after all and can describe many of JavaScript's dynamic features, not all of which are feasible to support in ahead-of-time compilation. Yet, sufficiently strict TypeScript code can often be made compatible with the AssemblyScript compiler with little effort.

---

Q. What are good use cases for AssemblyScript?

A. Computation-heavy logic like image manipulation, hot game logic, specialized algorithms, emulators, compilers and the likes are great use cases for WebAssembly, and as such for AssemblyScript as well. In some situations it may also be preferable to ship bytecode instead of minified JS, or just the ability to utilize a TypeScript-like language may open up new opportunities, for example for embedded scripting or plugins.

---

Q. Can AssemblyScript be used outside of the browser?

A. Absolutely! AssemblyScript modules are self-contained and run anywhere where WebAssembly is supported. There is also the option to target WASI.

---

Q. Why the strange name?

A. AssemblyScript is to Assembly as JavaScript is to Java. Not quite.

---
