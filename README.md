# dexscreener-scripts

Scripts for testing out dexscreener on windows

```sh
$ curl.exe 'https://api.dexscreener.com/token-profiles/latest/v1' | jq '.[0]'
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

To get boosted ones that match on ethereum

```sh
$ curl.exe 'https://api.dexscreener.com/token-boosts/latest/v1' | jq '.[] | select(.chainId | contains(\"ethereum\"))'
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
100 25892    0 25892    0     0  94855      0 --:--:-- --:--:-- --:--:-- 95896
{
  "url": "https://dexscreener.com/ethereum/0xe4224e3fac2926eb18a20fa168d1b8c51e854526",
  "chainId": "ethereum",
  "tokenAddress": "0xE4224E3fAC2926Eb18A20Fa168D1B8C51E854526",
  "description": "??????????? GOMA INU (???????????????) The Hidden Sister of Doge\n\nWhile the world adored Kabosu, few knew of her quiet companion Goma, the gentle Shiba who shared her heart and home in Chiba, Japan.",
  "icon": "dda79694b064a1a53f7d9086574a4b8a4af45639c2d542f8dd342c155a8a47e8",
  "header": "https://cdn.dexscreener.com/cms/images/f15d14858c39cb191d3a55d4e9ffa3cd037a0f1400fc4980587c2733bfe15c37?width=900&height=300&fit=crop&quality=95&format=auto",
  "openGraph": "https://cdn.dexscreener.com/token-images/og/ethereum/0xe4224e3fac2926eb18a20fa168d1b8c51e854526?timestamp=1761396000000",
  "links": [
    {
      "url": "https://gomainu.xyz/"
    },
    {
      "type": "twitter",
      "url": "https://x.com/GomaInuEth"
    },
    {
      "type": "telegram",
      "url": "https://t.me/ShibaInuGOMA"
    }
  ],
  "totalAmount": 100,
  "amount": 100
}
```
