# <a name="workbooksessioninfo-resource-type"></a>workbookSessionInfo リソース型

ブック セッションについての情報を提供します。


## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です

<!-- {
  "blockType": "resource",
  "optionalProperties": [  ],
  "@odata.type": "microsoft.graph.workbookSessionInfo"
}-->

```json
{
  "id": "string",
  "persistChanges": true
}
```

## <a name="properties"></a>プロパティ

| プロパティ | 型  | 説明                               |
|:---------|:------|:------------------------------------------|
| id  | string | ブック セッションの ID。 |
| persistChanges | string |  `true`: 永続セッションの場合。 `false`: 非永続セッション (表示モード) の場合。 |

