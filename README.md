# Development environment in Docker Container for Nordic nrf-sdk

Pre-Requisites:
- git installed
- vscode installed, with plugins "Remote Containers", "Cortex-Debug", "Serial Monitor", "C/C++"
- Docker Desktop installed
- Segger JLinkServer

How to use:
1. "git clone https://github.com/stemschmidt/nordic-project-template.git"
2. "cd nordic-project-template"
3. "code ." or open nordic-project-template in VSCode
4. in VSCode, select "reopen folder in container"
5. after docker container has started, go to "TERMINAL" tab:
6. "west init -l application"
7. "west update"
8. "source zephyr/zephyr-env.sh" (set environment variables, has to be done everytime the container is started)
9. "cd application"
10. "west build -b <YOUR_BOARD>" and wait for the build to finish...

11. on the host, launch the JLinkGDBServer (e.g "JLinkGDBServerCLExe -if swd -device <YOUR_DEVICE> -vd")
12. Select "Run and Debug" icon in activity bar in VSCode --> Download binary and start debugging by launching "JLink"

NOTE:
There is an issue with the order in which the plugins are loaded. A warning appears asking you to reload the window.
After reloading the window you will have to launch bash again: '$ bash'
