# User Details

## Fetching User Details

{% hint style="warning" %}
This endpoint is **NOT** recommended to be used to fetch players inventories, if so please use Roblox's inventory API for that.&#x20;
{% endhint %}

{% swagger baseUrl="https://www.rolimons.com/api/playerassets" method="get" path="/UserID" summary="Returns recently posted ads" %}
{% swagger-description %}

{% endswagger-description %}

{% swagger-parameter in="path" name="UserID" type="Number" required="true" %}

{% endswagger-parameter %}

{% swagger-response status="200" description="Successfully fetched data" %}
```json
{
   "success":true,
   "playerTerminated":false,
   "playerPrivacyEnabled":false,
   "playerVerified":true,
   "playerId":135190312,
   "chartNominalScanTime":1662249600,
   "playerAssets":{
      "9255011":[
         22555818460
      ],
      "745788688":[
         10436409764
      ],
      "1744060292":[
         22167452815
      ]
   },
   "isOnline":true,
   "lastOnline":1662298114,
   "lastLocation":"Online",
   "lastPlaceId":null,
   "locationGameIsTracked":false,
   "locationGameIconUrl":null,
   "premium":true,
   "badges":{
      "booster":1652205943,
      "verified":1577050507,
      "own_1_rare":1646863170,
      "value_100k":1617674796,
      "own_10_items":1646472014,
      "own_1_dominus":1658909715,
      "own_1_kotn_item":1617649694,
      "create_10_trade_ads":1604896347,
      "create_100_trade_ads":1646510247,
      "own_1_immortal_sword":1646863170
   }
}
```
{% endswagger-response %}

{% swagger-response status="429: Too Many Requests" description="Rate Limited" %}

{% endswagger-response %}
{% endswagger %}

## Using The Data

{% tabs %}
{% tab title="Player Assets" %}


| ItemId | UAID |
| ------ | ---- |
{% endtab %}

{% tab title="Untitled" %}


| Badge Name | Acquired Time in Epoch |
| ---------- | ---------------------- |
{% endtab %}
{% endtabs %}
