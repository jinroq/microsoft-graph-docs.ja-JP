# <a name="update-schemaextension"></a>schemaExtension を更新する

指定された [schemaExtension](../resources/schemaextension.md) の定義に含まれるプロパティを更新します。

この更新は、拡張機能の **targetTypes** プロパティに含まれるすべてのリソースに適用されます。これらのリソースは、[サポートしているリソースの種類](../../../concepts/extensibility_overview.md#supported-resources)にあります。

スキーマ拡張機能を作成したアプリ (所有者アプリ) に限り、その拡張機能が **InDevelopment** か **Available** の状態である場合、拡張機能に対して付加的な更新を行うことができます。したがって、そのアプリは、定義からカスタム プロパティやターゲット リソースの種類を削除できません。ただし、このアプリで拡張機能の説明を変更することはできます。

## <a name="prerequisites"></a>前提条件
この API を実行するには、以下の**スコープ**が必要です。*Directory.AccessAsUser.All*

## <a name="http-request"></a>HTTP 要求
<!-- { "blockType": "ignored" } -->
```http
PATCH /schemaExtensions/{id}
```
### <a name="optional-request-headers"></a>オプションの要求ヘッダー
| 名前      |説明|
|:----------|:----------|
| Authorization  | Bearer &lt;token&gt;。必須。 |
| Content-Type   | application/json | 

## <a name="request-body"></a>要求本文
要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。

| プロパティ       | 型    |説明|
|:---------------|:--------|:----------|
|description|String|スキーマ拡張機能の説明。|
|properties|[extensionSchemaProperty](../resources/extensionschemaproperty.md) コレクション|スキーマ拡張機能の定義を構成するプロパティの名前と種類のコレクション。付加的な変更のみが許可されます。 |
|status|String|スキーマ拡張機能のライフサイクル状態。作成時の初期状態は **InDevelopment** です。状態は、**InDevelopment** から **Available**、**Available** から **Deprecated**、**Deprecated** から **Available** のいずれかに切り替わります。|
|targetTypes|String コレクション|スキーマ拡張機能に適用できる (拡張機能をサポートできる) 一連の Microsoft Graph の種類。付加的な変更のみが許可されます。|

## <a name="response"></a>応答
成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で、更新された [schemaExtension](../resources/schemaextension.md) オブジェクトを返します。
## <a name="example"></a>例
##### <a name="request"></a>要求
以下は、要求の例です。
<!-- {
  "blockType": "request",
  "name": "update_schemaextension"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/schemaExtensions/{id}
Content-type: application/json
Content-length: 201

{
  "properties": [
    {
      "name":"new-name-value",
      "type":"new-type-value"
    },
    {
      "name":"additional-name-value",
      "type":"additional-type-value"
    }
  ],
}
```
##### <a name="response"></a>応答
以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.schemaExtension"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 201

{
  "id": "id-value",
  "description": "description-value",
  "targetTypes": [
    "targetTypes-value"
  ],
  "properties": [
    {
      "name":"name-value",
      "type":"type-value"
    },
    {
      "name":"new-name-value",
      "type":"new-type-value"
    },
    {
      "name":"additional-name-value",
      "type":"additional-type-value"
    }  
  ],
  "status": "status-value",
  "owner": "owner-value"
}
```

## <a name="see-also"></a>関連項目

- [拡張機能を使用してカスタム データをリソースに追加する](../../../concepts/extensibility_overview.md)
- [スキーマ拡張機能を使用したグループへのカスタム データの追加](../../../concepts/extensibility_schema_groups.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update schemaextension",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->