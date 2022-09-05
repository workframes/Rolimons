# User Details

## Fetching User Details

{% hint style="warning" %}

{% endhint %}

{% swagger baseUrl="https://www.rolimons.com/playerapi/player" method="get" path="/UserID" summary="Returns recently posted ads" %}
{% swagger-description %}

{% endswagger-description %}

{% swagger-parameter in="path" name="UserID" type="Number" required="true" %}

{% endswagger-parameter %}

{% swagger-response status="200" description="Successfully fetched data" %}
```json
{
   "name":"Rolimon",
   "value":324812,
   "rap":322989,
   "rank":null,
   "premium":true,
   "privacy_enabled":false,
   "terminated":false,
   "stats_updated":1662341676,
   "last_online":1662249022,
   "last_location":"Offline",
   "rolibadges":{
      "booster":1649531936,
      "roligang":1597630304,
      "verified":1567444532,
      "value_100k":1567444532,
      "own_10_items":1622046939,
      "own_lucky_cat_uaid":1594003428,
      "create_10_trade_ads":1579732196
   }
}
```
{% endswagger-response %}

{% swagger-response status="429: Too Many Requests" description="Rate Limited" %}
Recommended to send 10 requests every minute 
{% endswagger-response %}
{% endswagger %}

## Using The Data

{% tabs %}
{% tab title="Badges" %}


| Badge Name | Acquired Time in Epoch |
| ---------- | ---------------------- |
{% endtab %}
{% endtabs %}
