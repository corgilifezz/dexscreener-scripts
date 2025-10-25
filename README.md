# dexscreener-scripts

Scripts for testing out dexscreener on windows

```sh
PS C:\Users\User> curl.exe 'https://api.dexscreener.com/token-profiles/latest/v1' | jq '.[0]'
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
100 30333    0 30333    0     0  55405      0 --:--:-- --:--:-- --:--:-- 55656
{
  "url": "https://dexscreener.com/bsc/0x212e05f7df8fafed3ce2cce6093f16fb0a224444",
  "chainId": "bsc",
  "tokenAddress": "0x212E05F7dF8faFed3cE2Cce6093f16fB0a224444",
  "icon": "https://cdn.dexscreener.com/cms/images/ed2462115f8a0d16509289a6f9d68baff00a7ca33e8eb460dabe929bd4788c8d?width=64&height=64&fit=crop&quality=95&format=auto",
  "header": "https://cdn.dexscreener.com/cms/images/87cf1a347cc3bc62d9a2e0a9de8849cc5ec398481b7ef77963c8a6550855ab41?width=600&height=200&fit=crop&quality=95&format=auto",
  "openGraph": "https://cdn.dexscreener.com/token-images/og/bsc/0x212e05f7df8fafed3ce2cce6093f16fb0a224444?timestamp=1761395400000",
  "description": "AI Robotics develops specialised, production-grade bots for modern financial markets. Each bot is engineered for a specific role ??? reliable exchange execution and portfolio operations, precision sniper bots for opportunistic trading, frontrun modules for latency-sensitive strategies, and integrated risk managers for stop-loss and position control. Our platform pairs low-latency execution with strict safety layers and clear audit trails, making it simple to deploy, monitor and adapt algorithms in live markets. Visual assets and detailed documentation explain each bot???s purpose and configuration, so clients can quickly choose the right tools for their strategies.",
  "links": [
    {
      "label": "Website",
      "url": "https://roboticsbnb.xyz/"
    },
    {
      "type": "twitter",
      "url": "https://x.com/airobotics_bsc?s=21"
    }
  ],
  "cto": false
}
```
