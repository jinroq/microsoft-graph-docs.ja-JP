# <a name="sortfield-resource-type"></a>SortField リソースの種類

並べ替え操作の条件を表します。

## <a name="properties"></a>プロパティ
| プロパティ     | タイプ   |説明|
|:---------------|:--------|:----------|
|昇順|ブール値|昇順の方法で並べ替えを行うかどうかを表します。|
|色|文字列|並べ替えがフォントまたはセルの色で行われるときに条件の対象となる色を表します。|
|dataOption|文字列|このフィールドの他の並べ替えオプションを表します。 指定できる値は、`Normal`、`TextAsNumber` です。|
|鍵|int|条件の対象とする列 (または行。並べ替えの方向によって異なります) を表します。最初の列 (または行) からのオフセットとして表します。|
|sortOn|文字列|この条件の並べ替えの種類を表します。 可能な値は、`Value`、`CellColor`、`FontColor`、`Icon` です。|
|アイコン|[WorkbookIcon](icon.md)|並べ替えがセルのアイコンで行われるときに条件の対象となるアイコンを表します。|

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "@odata.type": "microsoft.graph.workbookSortField"
}-->

```json
{
  "ascending": true,
  "color": "string",
  "dataOption": "string",
  "key": 1024,
  "sortOn": "string",
  "icon": { "@odata.type": "microsoft.graph.workbookIcon" }
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "SortField resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->