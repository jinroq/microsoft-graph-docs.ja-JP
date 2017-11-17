<span data-ttu-id="a44be-p102">クライアントは、オープン型のプロパティを定義できます。この例では、プロパティとその値を [externalReference](plannerexternalreference.md) オブジェクトにする必要があるため、クライアントは **HTTP/HTTPS** プロトコルに基づいて **有効な URL** を指定する必要があります。OData に基づき、オープン型のプロパティ名には、`.`、`:`、`%` の文字を含めることができないため、エンコードする必要があります。以下に例を示します。参照を削除するには、プロパティの値を `null` に設定します。</span><span class="sxs-lookup"><span data-stu-id="a44be-p102">Properties of an Open Type can be defined by the client. In this case, the client must provide **valid URLs** based on the **HTTP/HTTPS** protocols as properties and their values must be the [externalReference](plannerexternalreference.md) objects. Based on OData, property names in Open Types cannot contain the following characters: `.`, `:`, `%`  so they need to be encoded. Example is shown below. To remove a reference, set the value of the property to `null`.</span></span>
クライアントは、オープン型のプロパティを定義できます。この例では、プロパティとその値を [externalReference](plannerexternalreference.md) オブジェクトにする必要があるため、クライアントは **HTTP/HTTPS** プロトコルに基づいて **有効な URL** を指定する必要があります。OData に基づき、オープン型のプロパティ名には、`.`、`:`、`%` の文字を含めることができないため、エンコードする必要があります。以下に例を示します。参照を削除するには、プロパティの値を `null` に設定します。

## <span data-ttu-id="a44be-112">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a44be-112">JSON representation</span></span>
<a id="json-representation" class="xliff"></a>

<span data-ttu-id="a44be-113">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="a44be-113">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerExternalReferences"
}-->


```json
{
  "String-value":
  {
    "alias": "String-value",
    "lastModifiedBy": "String-value",
    "lastModifiedDateTime": "String(timestamp)",
    "previewPriority": "String-value",
    "type": "String-value"
  }
}
```

<span data-ttu-id="a44be-114">// 例</span><span class="sxs-lookup"><span data-stu-id="a44be-114">// Example</span></span>

```json
{
  "https%3A//contoso%2Esharepoint%2Ecom/teams/agile/documents/AnnualReport%2Epptx":
  {
    "@odata.type": "microsoft.graph.externalReference", // required in PATCH requests to edit the references on a task
    "alias": "Agile Team Annual Report",
    "lastModifiedBy": {
      "user": {
        "id": "ebf3b108-5234-4e22-b93d-656d7dae5874"
      }
    },
    "lastModifiedDateTime": "2015-09-21T17:45:12.039Z",
    "previewPriority": "0009005756397228702",
    "type": "PowerPoint"
  }
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerExternalReferences resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->