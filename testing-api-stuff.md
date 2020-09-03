---
description: This is some Heartcore stuff
---

# Testing API stuff

{% api-method method="get" host="https://cdn.umbraco.io/media" path="" %}
{% api-method-summary %}
Get root media
{% endapi-method-summary %}

{% api-method-description %}
Get all media at the root of the tree.
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-headers %}
{% api-method-parameter name="Umb-Project-Alias" type="string" required=true %}
{project alias}
{% endapi-method-parameter %}

{% api-method-parameter name="Api-Version" type="string" required=true %}

{% endapi-method-parameter %}
{% endapi-method-headers %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}

{% endapi-method-response-example-description %}

```
{
    "_links": {
        "self": {
            "href": "https://cdn.umbraco.io/media"
        },
        "media": [
            {
                "href": "https://cdn.umbraco.io/media/b6f11172-373f-4473-af0f-0b0e5aefd21c"
            },
            {
                "href": "https://cdn.umbraco.io/media/1fd2ecaf-f371-4c00-9306-867fa4585e7a"
            },
            {
                "href": "https://cdn.umbraco.io/media/6d5bf746-cb82-45c5-bd15-dd3798209b87"
            }
        ]
    },
    "_embedded": {
        "media": [
            {
                "_creatorName": "Rasmus",
                "_url": "",
                "_writerName": "Rasmus",
                "_hasChildren": true,
                "_level": 1,
                "_createDate": "2019-06-17T13:46:41.47Z",
                "_id": "b6f11172-373f-4473-af0f-0b0e5aefd21c",
                "_updateDate": "2019-06-17T13:46:41.47Z",
                "_links": {
                    "self": {
                        "href": "https://cdn.umbraco.io/media/b6f11172-373f-4473-af0f-0b0e5aefd21c"
                    }
                },
                "mediaTypeAlias": "Folder",
                "name": "Design",
                "sortOrder": 1
            },
            {
                "_creatorName": "Rasmus",
                "_url": "",
                "_writerName": "Rasmus",
                "_hasChildren": true,
                "_level": 1,
                "_createDate": "2019-06-17T13:46:41.64Z",
                "_id": "1fd2ecaf-f371-4c00-9306-867fa4585e7a",
                "_updateDate": "2019-06-17T13:46:41.64Z",
                "_links": {
                    "self": {
                        "href": "https://cdn.umbraco.io/media/1fd2ecaf-f371-4c00-9306-867fa4585e7a"
                    }
                },
                "mediaTypeAlias": "Folder",
                "name": "People",
                "sortOrder": 1
            },
            {
                "_creatorName": "Rasmus",
                "_url": "",
                "_writerName": "Rasmus",
                "_hasChildren": true,
                "_level": 1,
                "_createDate": "2019-06-17T13:46:41.783Z",
                "_id": "6d5bf746-cb82-45c5-bd15-dd3798209b87",
                "_updateDate": "2019-06-17T13:46:41.783Z",
                "_links": {
                    "self": {
                        "href": "https://cdn.umbraco.io/media/6d5bf746-cb82-45c5-bd15-dd3798209b87"
                    }
                },
                "mediaTypeAlias": "Folder",
                "name": "Products",
                "sortOrder": 1
            }
        ]
    }
}
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

