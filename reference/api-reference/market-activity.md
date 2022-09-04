# Market Activity

## Fetching Market Activity

{% hint style="success" %}
10 \* (New Rap - Old Rap) + Old Rap = Price Purchased
{% endhint %}

{% swagger baseUrl="https://www.rolimons.com/api/activity" method="get" path="" summary="Returns recent market activity" %}
{% swagger-description %}

{% endswagger-description %}

{% swagger-response status="200" description="Successfully fetched data" %}
```json
{
   "success":true,
   "activities":[
      [
         Purchased Time In Epoch,
         Unkown Value,
         Item Id,
         Old Rap,
         New Rap,
         UAID
      ],
      [
         1662314641,
         1,
         10159622004,
         584,
         589,
         3144219
      ]
   ],
   "activities_count": 41
}
```
{% endswagger-response %}

{% swagger-response status="429: Too Many Requests" description="Rate Limited" %}

{% endswagger-response %}
{% endswagger %}
