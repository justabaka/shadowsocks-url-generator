## Shadowsocks URL Generator
Simple script to generate shadowsocks base64 encoded URL from config file

### Usage
Simply copy and paste the following in a terminal:
```bash
python <(curl -s https://raw.githubusercontent.com/amayatsky/shadowsocks-url-generator/master/ss-genuri.py) \
-c /etc/shadowsocks-libev/config.json
```
Change /etc/shadowsocks-libev/config.json path if needed.
### Example
Input:
```javascript
{
    "server":"github.com",
    "server_port":8388,
    "password":"fake_pwd",
    "method":"chacha20-ietf-poly1305"
}
```
Output:
```bash
Server: github.com
Method: chacha20-ietf-poly1305
Password: HIDDEN
Port: 8388
URL: ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpmYWtlX3B3ZEBnaXRodWIuY29tOjgzODg=#github.com
```
### Disclaimer
Requires Python to work
### Contribution
Feel free to send me your PRs! :)
