# BTCPay Server Plugin for Galoy

Learn more in [plugin documentation](https://docs.btcpayserver.org/Development/Plugins/).

# To Build and Run
1. Build your plugin
```
dotnet build BTCPayServer.Plugins.Galoy
```
2. Open btcpayserver in a new vscode instance (need a new instance for debugging later on)
```
code btcpayserver
```
3. Add settings
```
touch BTCPayServer/appsettings.dev.json
```
File
```
{
  "DEBUG_PLUGINS": "/full/path/to/btcpayserver-plugin-galoy/BTCPayServer.Plugins.Galoy/bin/Debug/net6.0/BTCPayServer.Plugins.Galoy.dll"
}
```
4. Build btcpayserver
```
dotnet build btcpayserver
```
5. Add ref to your plugin (if you have not already done this)
```
dotnet sln add ../BTCPayServer.Plugins.Galoy -s Plugins
```
6. Debug
- Click the debug button in vscode
- Click "Play" button (.NET Core launch (web))
7. Enable plugin in web. This will open the web browser. Add the Galoy plugin
