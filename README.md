# tes3mp-rs-example

This is an example project for tes3mp-rs, using my personal fork for tes3mp 0.8.1 [Here](https://github.com/HotaruBlaze/tes3mp-rs)

# How to get started
`git clone --recurse-submodules https://github.com/HotaruBlaze/tes3mp-rs-example.git`

# How to install the build project
1) Place the compiled file to `server/lib`
2) edit `tes3mp-server-default.cfg` and append the file to plugins, such as the following

### Note: You __cannot__ have a space after the comma.

```
[Plugins]
home = ./server
plugins = serverCore.lua,../lib/libtes3mp_plugin.so
```

If successful you should see something like the following the following in tes3mp's console output
```
[2023-06-14 18:58:21] [WARN]: Script function pointer not found: CreateTimerEx
[2023-06-14 18:58:21] [WARN]: Script function pointer not found: CallPublic
[2023-06-14 18:58:21] [WARN]: Script function pointer not found: MessageBox
[2023-06-14 18:58:21] [INFO]: [Script]: Called "OnServerInit"
[2023-06-14 18:58:21] [INFO]: [Script]: Reading banlist.json
[2023-06-14 18:58:21] [WARN]: [Script]: Hello from Phoenix's tes3mp-rs Fork :3
[2023-06-14 18:58:21] [INFO]: [Script]: Event triggered: on_server_init
[2023-06-14 18:58:21] [INFO]: Sharing server query info to master enabled.
[2023-06-14 18:58:21] [INFO]: [Script]: Reading requiredDataFiles.json
[Script]: - 1: "Morrowind.esm": [7B6AF5B9, 34282D67] 
[Script]: - 2: "Tribunal.esm": [F481F334, 211329EF] 
[Script]: - 3: "Bloodmoon.esm": [43DD2132, 9EB62F26] 
[2023-06-14 18:58:21] [INFO]: [Script]: Event triggered: on_request_data_file_list
[2023-06-14 18:58:21] [INFO]: [Script]: Called "OnServerPostInit"
[2023-06-14 18:58:21] [FATAL]: [Script]: Hello there!
[2023-06-14 18:58:21] [INFO]: [Script]: Event triggered: on_server_post_init
