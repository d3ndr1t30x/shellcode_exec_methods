# Shellcode Execution Methods

## Commonly Used Methods

1. **Direct Shellcode Execution**
   - Injecting and executing shellcode directly in a target process.

2. **Process Hollowing**
   - Creating a new process in a suspended state, replacing its code with shellcode, and resuming it.

3. **DLL Injection**
   - Injecting a DLL containing shellcode into a target process.

4. **Remote Thread Injection**
   - Creating a remote thread in a target process that executes shellcode.

5. **Reflective DLL Injection**
   - Loading and executing a DLL directly from memory.

6. **Heap Spraying**
   - Allocating a large amount of memory in a process and filling it with shellcode to increase the chances of execution.

7. **Code Cavities**
   - Finding and exploiting unused code sections in an existing binary to inject shellcode.

8. **Stack Pivoting**
   - Redirecting the stack pointer to controlled data that includes shellcode.

## Less Commonly Used Methods

1. **Atom Bombing**
   - Using the Windows atom table to store shellcode and execute it.

2. **Thread Hijacking**
   - Hijacking an existing thread to execute shellcode.

3. **Callback Functions**
   - Using Windows callback functions (e.g., Windows Hook, APC) to execute shellcode.

4. **VBA Macro Injection**
   - Embedding shellcode in a VBA macro in Office documents.

5. **Hardware Breakpoints**
   - Setting a hardware breakpoint to trigger execution of shellcode.

6. **Registry-based Persistence**
   - Storing shellcode in the Windows registry and executing it via a registry-based mechanism.

7. **Userland API Hooking**
   - Hooking userland APIs and redirecting execution flow to shellcode.

8. **COM Hijacking**
   - Hijacking Component Object Model (COM) objects to execute shellcode.

9. **Windows Management Instrumentation (WMI)**
   - Using WMI scripts or events to execute shellcode.

10. **Transacted Hollowing**
    - Using Windows transactions to hollow out and replace code in a transacted file.

11. **PowerShell**
    - Using PowerShell scripts to download and execute shellcode.

12. **Abusing Signed Binaries**
    - Using legitimate signed binaries (Living off the Land Binaries) to load and execute shellcode.
