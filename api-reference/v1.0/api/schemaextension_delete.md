# <a name="delete-schemaextension"></a>schemaExtension を削除する

[スキーマ拡張機能](../resources/schemaExtension.md)の定義を削除します。

スキーマ拡張機能を作成したアプリ (所有者アプリ) だけが、そのスキーマ拡張機能が **InDevelopment** 状態の場合に限り、スキーマ拡張機能の定義を削除できます。スキーマ拡張機能の定義を削除しても、その定義に基づいてリソース インスタンスに追加されたカスタム データへのアクセスには影響しません。


## <a name="prerequisites"></a>前提条件
この API を実行するには、以下の**スコープ**が必要です。*Directory.AccessAsUser.All*

## <a name="http-request"></a>HTTP 要求
<!-- { "blockType": "ignored" } -->
```http
DELETE /schemaExtensions/{id}
```

## <a name="request-headers"></a>要求ヘッダー
| 名前      |説明|
|:----------|:----------|
| Authorization  | Bearer &lt;token&gt;。必須。 |
 

## <a name="request-body"></a>要求本文
このメソッドには、要求本文を指定しません。


## <a name="response"></a>応答
成功した場合、このメソッドは `204, No Content` 応答コードを返します。応答本文には何も返されません。

## <a name="example"></a>例
##### <a name="request"></a>要求
以下は、要求の例です。
<!-- {
  "blockType": "request",
  "name": "delete_schemaextension"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/schemaExtensions/{id}
```
##### <a name="response"></a>応答
以下は、応答の例です。 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a>関連項目

- [拡張機能を使用してカスタム データをリソースに追加する](../../../concepts/extensibility_overview.md)
- [スキーマ拡張機能を使用したグループへのカスタム データの追加](../../../concepts/extensibility_schema_groups.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete schemaExtension",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->