---
description: File Structure for Copy Bot jSON
---

# Optimized Settings for Copy Bot jSON File

**Things to Remember:  You can set individual quote amount for each wallet you want to copy.** \
\
\
**Example A**: If you have multiple wallets you want to copy\
\
\[&#x20;

&#x20;{ "wallet": "AAAAAAAXXXXXXXXXXXXXXXXXXX", \
&#x20;"buyAmount": 0.05, \
&#x20;"buySlippage": 300, \
&#x20;"sellSlippage": 70 \
&#x20;} ,\
&#x20;{ "wallet": "BBBBBBBBBBXXXXXXXXXXXXXXXX", \
&#x20;"buyAmount": 0.05, \
&#x20;"buySlippage": 300, \
&#x20;"sellSlippage": 70 \
&#x20;} ,\
&#x20;{ "wallet": "CCCCCCCCCCXXXXXXXXXXXXXXXXX", \
&#x20;"buyAmount": 0.05, \
&#x20;"buySlippage": 300, \
&#x20;"sellSlippage": 70 \
&#x20;}&#x20;

]\
\
\
**Example B:** If you only want to copy one Wallet\
\
\[

&#x20;{ "wallet": "XXXXXXXXXXXXXXXXXXXXXXXXXXX", \
&#x20;"buyAmount": 0.05, \
&#x20;"buySlippage": 300, \
&#x20;"sellSlippage": 70 \
&#x20;}&#x20;

]
