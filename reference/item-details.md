# Item Details

## Fetching Item Details

{% swagger baseUrl="www.rolimons.com/itemapi/itemdetails" method="get" path="" summary="Returns Details about every limited" %}
{% swagger-description %}

{% endswagger-description %}

{% swagger-response status="200" description="Successfully fetched data" %}
```json
{
   "success":true,
   "item_count":2222,
   "items":{
      "Item ID":[
         Name,
         Acronym,
         Rap,
         Value,
         Default Value,
         Demand,
         Trend,
         Projected,
         Hyped,
         Rare,
      ],
      "1028606":[
         "Red Baseball Cap",
         "",
         1014,
         -1,
         1014,
         -1,
         -1,
         -1,
         -1,
         -1
      ]
   }
}
```
{% endswagger-response %}

{% swagger-response status="429: Too Many Requests" description="Rate Limited" %}
You are only able to send 1 request per minute. Spamming will do nothing as its cached.
{% endswagger-response %}
{% endswagger %}

## Using The Data

{% tabs %}
{% tab title="Demand" %}


| -1 | None     |
| -- | -------- |
| 0  | Terrible |
| 1  | Low      |
| 2  | Normal   |
| 3  | High     |
| 4  | Amazing  |
{% endtab %}

{% tab title="Trend" %}


| -1 | None        |
| -- | ----------- |
| 0  | Lowering    |
| 1  | Unstable    |
| 2  | Stable      |
| 3  | Raising     |
| 4  | Fluctuating |
{% endtab %}

{% tab title="Projected" %}


| -1 | False |
| -- | ----- |
| 1  | True  |
{% endtab %}

{% tab title="Hyped" %}


| -1 | False |
| -- | ----- |
| 1  | True  |
{% endtab %}

{% tab title="Rare" %}


| -1 | False |
| -- | ----- |
| 1  | True  |
{% endtab %}
{% endtabs %}
