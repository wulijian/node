https://juejin.im/post/5cc5141ce51d456e3e7a3be2
在vscode中debug

vscode配置
{
   "name": "node debug",
    "type": "cppdbg",
    "request": "launch",
    // "preLaunchTask": "make",
    "program": "${workspaceRoot}/out/Debug/node",
    "args": [
      "--inspect-brk",
        "/path/to/debug/index.js"
    ],
    "stopAtEntry": false,
    "cwd": "${workspaceFolder}",
    "environment": [],
    "externalConsole": false,
    "MIMode": "lldb"
}

externalConsole 如果为true，会打开外部终端，无法进入debug模式
