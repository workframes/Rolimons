# Recent Ads

## Fetching Recent Ads

{% swagger baseUrl="www.rolimons.com/tradeadsapi/getrecentads" method="get" path="" summary="Returns recently posted ads" %}
{% swagger-description %}

{% endswagger-description %}

{% swagger-response status="200" description="Successfully fetched data" %}
```json
{
   "success":true,
   "trade_ad_count":133,
   "trade_ads":[
      [
         AdId,
         Posted Time In Epoch,
         UserId,
         Username,
         {
            "items":[
               Offfering Items
            ]
         },
         {
            "items": [
               Requested Items
            ]
            "tags":[
               Requested Tags
            ]
         }
      ],
      [
         25984066,
         1662314052,
         703463166,
         "McTuTeJb228",
         {
            "items":[
               19027209,
               9731852643,
               3016210752
            ]
         },
         {
            "items": [
               151784526
            ]
            "tags":[
               5,
               6
            ]
         }
      ]
   ]
}
```
{% endswagger-response %}

{% swagger-response status="429: Too Many Requests" description="Rate Limited" %}

{% endswagger-response %}
{% endswagger %}

## Using The Data

{% tabs %}
{% tab title="Tags" %}


| 1  | Demand     |
| -- | ---------- |
| 2  | Rares      |
| 3  | Robux      |
| 4  | Any        |
| 5  | Upgrade    |
| 6  | Downgrade  |
| 7  | Rap        |
| 8  | Wishlist   |
| 9  | Projecteds |
| 10 | Adds       |
{% endtab %}
{% endtabs %}
