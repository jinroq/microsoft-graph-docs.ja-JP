# <a name="opentypeextension-resource-type-open-extensions"></a>openTypeExtension リソース タイプ (オープン拡張機能)

オープン拡張機能 (旧称は Office 365 のデータ拡張機能) を使用すると、型指定されていないプロパティを Microsoft Graph のリソースに簡単に直接追加できます。オープン拡張機能は、**openTypeExtension** リソースで表されます。リソースに追加されるオープン拡張機能は **extensions** ナビゲーション プロパティに表示されます。このプロパティは、[extension](extension.md) 抽象型から派生します。各拡張機能には **extensionName** プロパティがあります。このプロパティは、すべての拡張機能とカスタム データで唯一定義済みの書き込み可能なプロパティです。拡張機能名が必ず一意であるようにする方法の 1 つは、_独自のドメイン_に依存する逆引きドメイン ネーム システム (DNS) 形式 (例: `Com.Contoso.ContactInfo`) を使用することです。拡張機能名に Microsoft ドメイン (`Com.Microsoft` または `Com.OnMicrosoft`) を使用しないでください。

オープン拡張機能は、次のリソースの対応するバージョンの一般提供 (GA: /v1.0 および /ベータ) またはプレビュー (/ベータ) でサポートされています。

| リソース | バージョン |
|---------------|-------|
| [管理単位](../../beta/resources/administrativeunit.md)  | プレビューのみ |
| [予定表イベント](event.md) | GA |
| グループ[予定表イベント](event.md) | GA |
| グループ会話スレッド[投稿](post.md) | GA |
| [デバイス](../../beta/resources/device.md) | プレビューのみ |
| [グループ](../../beta/resources/group.md) | プレビューのみ |
| [message](message.md) | GA |
| [組織](../../beta/resources/organization.md) | プレビューのみ |
| [個人用連絡先](contact.md) | GA |
| [ユーザー](../../beta/resources/user.md) | プレビューのみ |


### <a name="use-open-extensions-for-outlook-resources-or-extended-properties"></a>オープン拡張機能 (Outlook リソース用) と拡張プロパティのどちらを使用するか

オープン拡張機能は、カスタム データの格納およびカスタムデータへのアクセスを必要とするほとんどのシナリオに対して推奨されるソリューションです。ただし、[拡張プロパティとこの REST API](extended-properties-overview.md) は、[Microsoft Graph API のメタデータ](http://developer.microsoft.com/en-us/graph/docs/overview/call_api)を通じてまだ公開されていない Outlook MAPI プロパティのカスタム データにアクセスする必要がある場合に使用できます。メタデータが公開するプロパティは、https://graph.microsoft.com/v1.0/$metadata で確認できます。


## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.opentypeextension"
}-->

```json
{
  "extensionName": "string",
  "id": "string (identifier)"
}

```
## <a name="properties"></a>プロパティ
| プロパティ       | 型    |説明|
|:---------------|:--------|:----------|
|extensionName|String|オープン型のオープン拡張機能の一意のテキスト識別子。必須。|
|id|String| **extensionName** と拡張子タイプを連結する完全修飾識別子。読み取り専用。|

## <a name="relationships"></a>リレーションシップ
なし


## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[Post](../api/opentypeextension_post_opentypeextension.md) | [openTypeExtension](opentypeextension.md)、または openTypeExtension オブジェクトが含まれている [メッセージ](../resources/message.md)、[イベント](../resources/event.md)、あるいは [連絡先](../resources/contact.md)。 | 既存または新規のリソース インスタンス内に openTypeExtension オブジェクトを作成します。| 
|[Get](../api/opentypeextension_get.md) | [openTypeExtension](opentypeextension.md) |openTypeExtension オブジェクトのプロパティと関係を読み取ります。|
|[更新する](../api/opentypeextension_update.md) | [openTypeExtension](opentypeextension.md)    |openTypeExtension オブジェクトを更新します。 |
|[削除](../api/opentypeextension_delete.md) | なし |openTypeExtension オブジェクトを削除します。 |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "openTypeExtension resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->