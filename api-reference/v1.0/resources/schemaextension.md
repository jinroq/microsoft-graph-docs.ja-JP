# <a name="schemaextension-resource-type-schema-extensions"></a>schemaExtension リソースの種類 (スキーマ拡張機能)

スキーマの拡張機能を使用すると、拡張するスキーマを定義し、厳密に型指定されたカスタム データをリソースの種類に追加できます。カスタム データは拡張したリソースの複合型として表示されます。 

スキーマ拡張機能は次のリソースの種類でサポートされています。

 - [contact](contact.md)
 - [device](device.md)
 - ユーザーまたは Office 365 グループ カレンダーの [event](event.md)
 - Office 365 グループの [post](post.md)
 - [group](group.md)
 - [message](message.md) 
 - [organization](organization.md)
 - [user](user.md)

カスタム データのグループへの追加方法については、[スキーマ拡張機能の例](../../../concepts/extensibility_schema_groups.md)を参照してください。

## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[Create](../api/schemaextension_post_schemaextensions.md) | schemaExtension |スキーマ拡張機能の定義を作成します。|
|[List](../api/schemaextension_list.md) | schemaExtension |使用可能な schemaExtension の定義とそのプロパティを一覧表示します。|
|[Get](../api/schemaextension_get.md) | schemaExtension |特定の schemaExtension 定義のプロパティを読み取ります。|
|[Update](../api/schemaextension_update.md) | schemaExtension   |schemaExtension 定義を更新します。 |
|[Delete](../api/schemaextension_delete.md) | なし |schemaExtension 定義を削除します。 |

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|description|String|スキーマ拡張機能の説明。|
|id|String|スキーマ拡張機能の定義の一意の識別子。 <br>値の割り当ては、以下の 2 方法のいずれかで行うことができます。 <ul><li>確認されたドメインの内の 1 つの名前とスキーマ拡張機能の名前を連結して、\{_&#65279;domainName_\}\_\{_&#65279;schemaName_\} という形式の一意の文字列を形成します。たとえば、`contoso_mySchema` です。 </li><li>スキーマ名を指定し、Microsoft Graph がそのスキーマ名を使用して **id** 割り当てを完了するには、次の形式を使用します。ext\{_&#65279;8-random-alphanumeric-chars_\}\_\{_&#65279;schema-name_\}。たとえば、`extkvbmkofy_mySchema` です。</li></ul>作成後、このプロパティは変更できません。 |
|owner|String|スキーマ拡張機能を作成したアプリケーションの AppID。読み取り専用です。|
|properties|[extensionSchemaProperty](extensionschemaproperty.md) コレクション|スキーマ拡張機能の定義を構成するプロパティ名と種類のコレクション。|
|status|String|スキーマ拡張機能のライフサイクル状態。考えられる状態は、**InDevelopment**、**Available**、および **Deprecated** です。作成時に自動で **InDevelopment** に設定されます。考えられる状態遷移と動作の詳細については、「[スキーマ拡張機能](../../../concepts/extensibility_overview.md#schema-extensions)」をご覧ください。|
|targetTypes|String collection|スキーマ拡張機能に適用できる (拡張機能をサポートできる) 一連の Microsoft Graph の種類。**contact**、**device**、**event**、**group**、**message**、**organization**、**post**、**user** のいずれかから選択します。|

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.schemaExtension"
}-->

```json
{
  "description": "String",
  "id": "String (identifier)",
  "owner": "String",
  "properties": [{"@odata.type": "microsoft.graph.extensionSchemaProperty"}],
  "status": "String",
  "targetTypes": ["String"]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "schemaExtension resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->