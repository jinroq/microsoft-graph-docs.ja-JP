# <a name="directoryobject-resource-type"></a>directoryObject リソースの種類

Azure Active Directory オブジェクトを表します。**directoryObject** 型は、他の多くのディレクトリ エンティティ型の基本型です。

## <a name="methods"></a>メソッド

| メソッド       | 戻り値の型  |説明|
|:---------------|:--------|:----------|
|[directoryObject を取得する](../api/directoryobject_get.md) | [directoryObject](directoryobject.md) |ディレクトリ オブジェクトのプロパティを読み取ります。|
|[directoryObject を削除する](../api/directoryobject_delete.md) | なし |ディレクトリ オブジェクトを削除します。 |
|[checkMemberGroups](../api/directoryobject_checkmembergroups.md)|String collection|グループの一覧内のメンバーシップを確認します。チェックは推移的です。|
|[getMemberGroups](../api/directoryobject_getmembergroups.md)|String collection|ユーザー オブジェクト、グループ オブジェクト、またはディレクトリ オブジェクトがメンバーであるすべてのグループを返します。チェックは推移的です。|
|[getMemberObjects](../api/directoryobject_getmemberobjects.md)|String コレクション| ユーザー オブジェクト、グループ オブジェクト、またはディレクトリ オブジェクトがメンバーであるすべてのグループとディレクトリ ロールを返します。チェックは推移的です。 |
|[getByIds](../api/directoryobject_getbyids.md) | [directoryObject](directoryobject.md) コレクション | 指定された一連の ID に基づいて、一連のディレクトリ オブジェクトを取得します。 |

## <a name="properties"></a>プロパティ

| プロパティ   | 型 |説明|
|:---------------|:--------|:----------|
|id|String|オブジェクトの一意識別子である Guid。例: 12345678-9abc-def0-1234-56789abcde。キー。null 許容ではありません。読み取り専用です。|

## <a name="relationships"></a>リレーションシップ

なし


## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.directoryObject"
}-->

```json
{
  "id": "string (identifier)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "directoryObject resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
