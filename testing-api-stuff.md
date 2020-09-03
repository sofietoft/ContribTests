---
description: This is some Heartcore stuff
---

# Testing API stuff

{% api-method method="get" host="https://cdn.umbraco.io/media" path="/" %}
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

{% api-method method="put" host="https://api.umbraco.io" path="/content/{id}/publish" %}
{% api-method-summary %}
Publich content
{% endapi-method-summary %}

{% api-method-description %}
Publish a specific content item with all language variation specific language.
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-query-parameters %}
{% api-method-parameter name="culture" type="string" required=true %}
Use language/variation alias, eg. "en-US"
{% endapi-method-parameter %}
{% endapi-method-query-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}

{% endapi-method-response-example-description %}

```
{
    "_currentVersionState": {
        "$invariant": "PUBLISHED"
    },
    "name": {
        "$invariant": "Another one"
    },
    "_updateDate": {
        "$invariant": "2019-10-10T11:19:04.3988745+00:00"
    },
    "_hasChildren": false,
    "_level": 3,
    "_createDate": "2019-10-07T11:53:09.653Z",
    "_id": "041067a0-74f5-4d03-92af-40c3c0aa13e7",
    "_links": {
        "self": {
            "href": "https://api.umbraco.io/content/041067a0-74f5-4d03-92af-40c3c0aa13e7"
        },
        "root": {
            "href": "https://api.umbraco.io/content"
        },
        "children": {
            "href": "https://api.umbraco.io/content/041067a0-74f5-4d03-92af-40c3c0aa13e7/children"
        },
        "publish": {
            "href": "https://api.umbraco.io/content/041067a0-74f5-4d03-92af-40c3c0aa13e7/publish"
        },
        "unpublish": {
            "href": "https://api.umbraco.io/content/041067a0-74f5-4d03-92af-40c3c0aa13e7/unpublish"
        },
        "contenttype": {
            "href": "https://api.umbraco.io/content/type/blogpost"
        }
    },
    "contentTypeAlias": "blogpost",
    "parentId": "8007e923-e62a-4ac1-a33f-caf3052582f4",
    "sortOrder": 0,
    "seoMetaDescription": {
        "$invariant": ""
    },
    "keywords": {
        "$invariant": []
    },
    "umbNaviHide": {
        "$invariant": "0"
    },
    "pageTitle": {
        "$invariant": "Another one"
    },
    "categories": {
        "$invariant": [
            "cg16",
            "codegarden",
            "umbraco"
        ]
    },
    "excerpt": {
        "$invariant": "Donec sollicitudin molestie malesuada. Vivamus suscipit tortor eget felis porttitor volutpat. Sed porttitor lectus nibh."
    },
    "bodyText": {
        "$invariant": "<p>Donec sollicitudin molestie malesuada. Proin eget tortor risus. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus magna justo, lacinia eget consectetur sed, convallis at tellus. Vivamus magna justo, lacinia eget consectetur sed, convallis at tellus. Curabitur arcu erat, accumsan id imperdiet et, porttitor at sem. Nulla porttitor accumsan tincidunt. Vivamus magna justo, lacinia eget consectetur sed, convallis at tellus. Nulla porttitor accumsan tincidunt. Donec rutrum congue leo eget malesuada.</p>\n<p>Vestibulum ante ipsum primis in faucibus orci luctus et ultrices posuere cubilia Curae; Donec velit neque, auctor sit amet aliquam vel, ullamcorper sit amet ligula. Pellentesque in ipsum id orci porta dapibus. Donec rutrum congue leo eget malesuada. Nulla porttitor accumsan tincidunt. Vestibulum ante ipsum primis in faucibus orci luctus et ultrices posuere cubilia Curae; Donec velit neque, auctor sit amet aliquam vel, ullamcorper sit amet ligula. Curabitur non nulla sit amet nisl tempus convallis quis ac lectus. Proin eget tortor risus. Pellentesque in ipsum id orci porta dapibus. Proin eget tortor risus. Sed porttitor lectus nibh.</p>\n<p>Pellentesque in ipsum id orci porta dapibus. Curabitur aliquet quam id dui posuere blandit. Praesent sapien massa, convallis a pellentesque nec, egestas non nisi. Praesent sapien massa, convallis a pellentesque nec, egestas non nisi. Curabitur non nulla sit amet nisl tempus convallis quis ac lectus. Praesent sapien massa, convallis a pellentesque nec, egestas non nisi. Donec rutrum congue leo eget malesuada. Donec rutrum congue leo eget malesuada. Sed porttitor lectus nibh. Nulla quis lorem ut libero malesuada feugiat.</p>"
    }
}
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

{% api-method method="delete" host="https://api.umbraco.io" path="/content/{id}" %}
{% api-method-summary %}
Delete content
{% endapi-method-summary %}

{% api-method-description %}
Delete a specific content item with all its language variations.
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}

{% endapi-method-response-example-description %}

```
{
    "_currentVersionState": {
        "$invariant": "PUBLISHED"
    },
    "name": {
        "$invariant": "Another one"
    },
    "_updateDate": {
        "$invariant": "2019-10-07T11:53:09.653Z"
    },
    "_hasChildren": false,
    "_level": 3,
    "_createDate": "2019-10-07T11:53:09.653Z",
    "_id": "041067a0-74f5-4d03-92af-40c3c0aa13e7",
    "_deleteDate": "2019-10-10T11:19:53.6828938Z",
    "_links": {
        "self": {
            "href": "https://api.umbraco.io/content/041067a0-74f5-4d03-92af-40c3c0aa13e7"
        },
        "root": {
            "href": "https://api.umbraco.io/content"
        },
        "children": {
            "href": "https://api.umbraco.io/content/041067a0-74f5-4d03-92af-40c3c0aa13e7/children"
        },
        "publish": {
            "href": "https://api.umbraco.io/content/041067a0-74f5-4d03-92af-40c3c0aa13e7/publish"
        },
        "unpublish": {
            "href": "https://api.umbraco.io/content/041067a0-74f5-4d03-92af-40c3c0aa13e7/unpublish"
        },
        "contenttype": {
            "href": "https://api.umbraco.io/content/type/blogpost"
        }
    },
    "contentTypeAlias": "blogpost",
    "parentId": "8007e923-e62a-4ac1-a33f-caf3052582f4",
    "sortOrder": 0,
    "seoMetaDescription": {
        "$invariant": ""
    },
    "keywords": {
        "$invariant": []
    },
    "umbNaviHide": {
        "$invariant": "0"
    },
    "pageTitle": {
        "$invariant": "Another one"
    },
    "categories": {
        "$invariant": [
            "cg16",
            "codegarden",
            "umbraco"
        ]
    },
    "excerpt": {
        "$invariant": "Donec sollicitudin molestie malesuada. Vivamus suscipit tortor eget felis porttitor volutpat. Sed porttitor lectus nibh."
    },
    "bodyText": {
        "$invariant": "<p>Donec sollicitudin molestie malesuada. Proin eget tortor risus. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus magna justo, lacinia eget consectetur sed, convallis at tellus. Vivamus magna justo, lacinia eget consectetur sed, convallis at tellus. Curabitur arcu erat, accumsan id imperdiet et, porttitor at sem. Nulla porttitor accumsan tincidunt. Vivamus magna justo, lacinia eget consectetur sed, convallis at tellus. Nulla porttitor accumsan tincidunt. Donec rutrum congue leo eget malesuada.</p>\n<p>Vestibulum ante ipsum primis in faucibus orci luctus et ultrices posuere cubilia Curae; Donec velit neque, auctor sit amet aliquam vel, ullamcorper sit amet ligula. Pellentesque in ipsum id orci porta dapibus. Donec rutrum congue leo eget malesuada. Nulla porttitor accumsan tincidunt. Vestibulum ante ipsum primis in faucibus orci luctus et ultrices posuere cubilia Curae; Donec velit neque, auctor sit amet aliquam vel, ullamcorper sit amet ligula. Curabitur non nulla sit amet nisl tempus convallis quis ac lectus. Proin eget tortor risus. Pellentesque in ipsum id orci porta dapibus. Proin eget tortor risus. Sed porttitor lectus nibh.</p>\n<p>Pellentesque in ipsum id orci porta dapibus. Curabitur aliquet quam id dui posuere blandit. Praesent sapien massa, convallis a pellentesque nec, egestas non nisi. Praesent sapien massa, convallis a pellentesque nec, egestas non nisi. Curabitur non nulla sit amet nisl tempus convallis quis ac lectus. Praesent sapien massa, convallis a pellentesque nec, egestas non nisi. Donec rutrum congue leo eget malesuada. Donec rutrum congue leo eget malesuada. Sed porttitor lectus nibh. Nulla quis lorem ut libero malesuada feugiat.</p>"
    }
}
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

