# <a name="update-a-group-setting"></a>グループ設定を更新する

特定のグループ設定オブジェクトのプロパティを更新します。

## <a name="prerequisites"></a>前提条件

この API を実行するには、以下のいずれかの**スコープ**が必要です。*Directory.ReadWrite.All* または *Directory.AccessAsUser.All*

> 注:テナント管理者のみが、作成、更新、削除の操作を実行する権限を持ちます。

## <a name="http-request"></a>HTTP 要求
<!-- { "blockType": "ignored" } -->

テナント全体またはグループ固有の設定を更新します。

```http
PATCH /groupSettings/{id}
PATCH /groups/{id}/settings/{id}
```
## <a name="optional-request-headers"></a>オプションの要求ヘッダー
| 名前 | 説明 |
|:-----------|:-----------|
| Authorization  | ベアラー {トークン}。必須。 |
| Content-Type  | application/json  |

## <a name="request-body"></a>要求本文
要求本文で、更新する関連フィールドの値を指定します。 

| プロパティ | 型 | 説明 |
|:---------------|:--------|:----------|
| values | settingValue | 更新された値のセットです。注:コレクション セット全体を指定する必要があります。単一の値のセットを更新することはできません。 |

## <a name="response"></a>応答

成功した場合、このメソッドは `204 OK` 応答コードと、応答本文で、更新された [groupSetting](../resources/groupsetting.md) オブジェクトを返します。

## <a name="example"></a>例
##### <a name="request"></a>要求
<!-- {
  "blockType": "request",
  "name": "update_groupsetting"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/groupSettings/{id}
Content-type: application/json
Content-length: 173

{
  "displayName": "displayName-value",
  "templateId": "templateId-value",
  "values": [
    {
      "name": "name-value",
      "value": "value-value"
    }
  ]
}
```
##### <a name="response"></a>応答

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.groupSetting"
} -->
```http
HTTP/1.1 204 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update groupSetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->