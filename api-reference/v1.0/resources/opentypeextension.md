# <a name="opentypeextension-resource-type-open-extensions"></a>openTypeExtension リソース タイプ (オープン拡張機能)

オープン拡張機能 (旧称は Office 365 のデータ拡張機能) を使用すると、型指定されていないプロパティを Microsoft Graph のリソースに簡単に直接追加できます。

オープン拡張機能は、**openTypeExtension** リソースで表されます。 リソースに追加されるオープン拡張機能は **extensions** ナビゲーション プロパティに表示されます。このプロパティは、[extension](extension.md) 抽象型から派生します。 各拡張機能には **extensionName** プロパティがあります。このプロパティは、すべての拡張機能とカスタム データで唯一定義済みの書き込み可能なプロパティです。

拡張機能名が必ず一意であるようにする方法の 1 つは、_独自のドメイン_に依存する逆引きドメイン ネーム システム (DNS) 形式 (例: `Com.Contoso.ContactInfo`) を使用することです。 拡張機能名に Microsoft ドメイン (`Com.Microsoft` または `Com.OnMicrosoft`) を使用しないでください。

オープン拡張機能の例:[オープン拡張機能を使用してカスタム データをユーザーに追加する](../../../concepts/extensibility_open_users.md)

オープン拡張機能は、次のリソースの対応するバージョンの一般提供 (GA: /v1.0 および /ベータ) またはプレビュー (/ベータ) でサポートされています。

|リソース |バージョン |
|:---------------|:-------|
| [管理単位](../../beta/resources/administrativeunit.md)  | プレビューのみ |
| [予定表イベント](event.md) | GA |
| グループ[予定表イベント](event.md) | GA |
| グループ会話スレッド[投稿](post.md) | GA |
| [device](device.md) | GA |
| [グループ](group.md) | GA |
| [メッセージ](message.md) | GA |
| [組織](organization.md) | GA |
| [個人用連絡先](contact.md) | GA |
| [ユーザー](user.md) | GA |

## <a name="outlook-specific-considerations"></a>Outlook に固有の考慮事項

Outlook のリソース上に存在する各オープン拡張 (イベント、メッセージ、または個人用の連絡先) は、[MAPI の名前付きプロパティ](https://msdn.microsoft.com/en-us/library/cc765864(v=office.15).aspx) に格納されます。 Outlook でオープン拡張を作成する際には、MAPI の名前付きプロパティを、ユーザーのメールボックス内の有限のリソースとみなします。 ユーザーの名前付きプロパティのクォータが不足すると、そのユーザーに対しそれ以上の名前付きプロパティを作成できません。 その場合、機能する名前付きプロパティに依存するクライアントで予期しない動作が発生することがあります。

Outlook のリソースでオープン拡張を作製する場合には、次のガイドラインを適用します。

- 必要な最小数の拡張機能を作成します。 ほとんどのアプリケーションでは、複数の拡張機能が必要です。 拡張機能には定義されたプロパティや構造がないため、単一の拡張機能に複数の値を格納することができます。
- (ユーザー入力などに基づく) 変数の方法で拡張機能の名前付けをしないでください。 ユーザーのメールボックスで以前に使用されたことがない新しい名前でオープン拡張が作成されるたびに、新しい MAPI 名前付きプロパティが作成されます。 拡張子を削除しても、名前付きプロパティは削除されません。

### <a name="use-open-extensions-for-outlook-resources-or-extended-properties"></a>オープン拡張 (Outlook リソース用) または拡張プロパティを使用

オープン拡張は、カスタム データの格納およびカスタムデータへのアクセスを必要とするほとんどのシナリオで推奨されるソリューションです。 ただし、[Microsoft Graph API メタデータ](http://developer.microsoft.com/en-us/graph/docs/overview/call_api) を通じてすでに公開されていない Outlook MAPI プロパティのカスタム データにアクセスする必要がある場合は、[拡張プロパティとその REST API](extended-properties-overview.md) を使用できます。 メタデータがどのプロパティを公開するかは [https://graph.microsoft.com/v1.0/$metadata](https://graph.microsoft.com/v1.0/$metadata) で確認できます。

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!--{
  "blockType": "resource",
  "openType": true,
  "optionalProperties": [],
  "baseType": "microsoft.graph.extension",
  "@odata.type": "microsoft.graph.openTypeExtension"
}-->

```json
{
  "extensionName": "string",
  "id": "string (identifier)"
}

```

## <a name="properties"></a>プロパティ

|プロパティ | タイプ | 説明 |
|:---------------|:--------|:----------|
|extensionName|文字列|オープン型のオープン拡張機能の一意のテキスト識別子。必須。|
|id|文字列| **extensionName** と拡張子タイプを連結する完全修飾識別子。読み取り専用。|

## <a name="relationships"></a>リレーションシップ

なし

## <a name="methods"></a>メソッド

|メソッド | 戻り値の型 | 説明 |
|:---------------|:--------|:----------|
|[投稿](../api/opentypeextension_post_opentypeextension.md) | (既存リソースのインスタンス内の) [openTypeExtension](opentypeextension.md)、または、openTypeExtension オブジェクトを含む新しい[contact](../resources/contact.md)、[event](../resources/event.md)、[message](../resources/message.md)。 | 既存または新規のリソース インスタンス内に openTypeExtension オブジェクトを作成します。|
|[取得](../api/opentypeextension_get.md) | [openTypeExtension](opentypeextension.md) |openTypeExtension オブジェクトのプロパティと関係を読み取ります。|
|[更新する](../api/opentypeextension_update.md) | [openTypeExtension](opentypeextension.md) |openTypeExtension オブジェクトを更新します。 |
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
