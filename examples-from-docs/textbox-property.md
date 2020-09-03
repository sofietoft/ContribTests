# Textbox Property

`Alias: Umbraco.Textbox`

`Returns: String`

Textbox is an HTML input control for text. It can be configured to have a fixed character limit. The default maximum amount of characters is 500 unless it's specifically changed to a lower amount.

## Data Type Definition Example

### Without a character limit

![](../.gitbook/assets/textbox-setup-v8.png)

## Content Example

### Without a character limit

![](../.gitbook/assets/textbox-content-v8.png)

### With a character limit

![](../.gitbook/assets/textbox-content-limit-v8.png)

## MVC View Example

{% tabs %}
{% tab title="v.8" %}
```csharp
@{
    if (Model.HasValue("pageTitle")){
        <p>@(Model.Value("pageTitle"))</p>
    }
}
```
{% endtab %}

{% tab title="v.7" %}
```csharp
@{
    if (Model.Content.HasValue("pageTitle")){
        <p>@(Model.Content.GetPropertyValue<string>("pageTitle"))</p>
    }
}
```
{% endtab %}
{% endtabs %}

