# Criar vendedor do tipo empresa

{% api-method method="post" host="https://api.zoop.ws" path="/v1/marketplaces/:marketplace\_id/sellers/businesses" %}
{% api-method-summary %}
Criar vendedor do tipo empresa
{% endapi-method-summary %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="marketplace\_id" type="string" required=true %}
ID de identificação do marketplace
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}

{% api-method-body-parameters %}
{% api-method-parameter name="id" type="string" required=false %}
{% endapi-method-parameter %}

{% api-method-parameter name="status" type="string" required=true %}
{% endapi-method-parameter %}

{% api-method-parameter name="resource" type="string" required=true %}
{% endapi-method-parameter %}

{% api-method-parameter name="type" type="string" required=true %}
{% endapi-method-parameter %}

{% api-method-parameter name="account_balance" type="string" required=true %}
{% endapi-method-parameter %}

{% api-method-parameter name="current_balance" type="string" required=true %}
{% endapi-method-parameter %}

{% api-method-parameter name="fiscal_responsability" type="string" required=true %}
{% endapi-method-parameter %}

{% api-method-parameter name="owner.first_name" type="string" required=true %}
{% endapi-method-parameter %}

{% api-method-parameter name="owner.last_name" type="string" required=true %}
{% endapi-method-parameter %}

{% api-method-parameter name="owner.email" type="string" required=true %}
{% endapi-method-parameter %}

{% api-method-parameter name="owner.phone_number" type="string" required=true %}
{% endapi-method-parameter %}

{% api-method-parameter name="owner.taxpayer_id" type="string" required=true %}
{% endapi-method-parameter %}

{% api-method-parameter name="owner.birthdate" type="string" required=true %}
{% endapi-method-parameter %}

{% api-method-parameter name="description" type="string" required=true %}
{% endapi-method-parameter %}

{% api-method-parameter name="business_name" type="string" required=true %}
{% endapi-method-parameter %}

{% api-method-parameter name="business_phone" type="string" required=true %}
{% endapi-method-parameter %}

{% api-method-parameter name="business_email" type="string" required=true %}
{% endapi-method-parameter %}

{% api-method-parameter name="business_website" type="string" required=true %}
{% endapi-method-parameter %}

{% api-method-parameter name="business_description" type="string" required=true %}
{% endapi-method-parameter %}

{% api-method-parameter name="business_facebook" type="string" required=true %}
{% endapi-method-parameter %}

{% api-method-parameter name="business_twitter" type="string" required=true %}
{% endapi-method-parameter %}

{% api-method-parameter name="ein" type="string" required=true %}
{% endapi-method-parameter %}

{% api-method-parameter name="statement_descriptor" type="string" required=true %}
{% endapi-method-parameter %}

{% api-method-parameter name="business_address" type="object" required=true %}
{% endapi-method-parameter %}

{% api-method-parameter name="business_address.line1" type="string" required=true %}
{% endapi-method-parameter %}

{% api-method-parameter name="business_address.line2" type="string" required=true %}
{% endapi-method-parameter %}

{% api-method-parameter name="business_address.line3" type="string" required=true %}
{% endapi-method-parameter %}

{% api-method-parameter name="business_address.neighborhood" type="string" required=true %}
{% endapi-method-parameter %}

{% api-method-parameter name="business_address.city" type="string" required=true %}
{% endapi-method-parameter %}

{% api-method-parameter name="business_address.state" type="string" required=true %}
{% endapi-method-parameter %}

{% api-method-parameter name="business_address.postal_code" type="string" required=true %}
{% endapi-method-parameter %}

{% api-method-parameter name="business_address.country_code" type="string" required=true %}
{% endapi-method-parameter %}

{% api-method-parameter name="business_opening_date" type="string" required=true %}
{% endapi-method-parameter %}

{% api-method-parameter name=""owner_address type="object" required=true %}
{% endapi-method-parameter %}







{% endapi-method-body-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
Cake successfully retrieved.
{% endapi-method-response-example-description %}

```javascript
{
    "name": "Cake's name",
    "recipe": "Cake's recipe name",
    "cake": "Binary cake"
}
```
{% endapi-method-response-example %}

{% api-method-response-example httpCode=404 %}
{% api-method-response-example-description %}
Could not find a cake matching this query.
{% endapi-method-response-example-description %}

```javascript
{
    "message": "Ain't no cake like that."
}
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}
