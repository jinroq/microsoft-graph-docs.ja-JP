# <a name="messageruleactions-resource-type"></a>messageRuleActions リソースの種類


ルールに使用可能なアクションのセットを表します。

## <a name="properties"></a>プロパティ
| プロパティ     | タイプ   |説明|
|:---------------|:--------|:----------|
| assignCategories | String コレクション | メッセージに割り当てられるカテゴリの一覧です。 |
| copyToFolder | 文字列 | メッセージのコピー先のフォルダーの ID です。 |
| 削除 | ブール値 | 削除済みアイテム フォルダーにメッセージを移動する必要があるかどうかを示します。 |
| forwardAsAttachmentTo | [recipient](recipient.md) コレクション | 添付ファイルとしてメッセージを転送する受信者の電子メール アドレスです。 |
| forwardTo | [recipient](recipient.md) コレクション | メッセージを転送する受信者の電子メール アドレスです。 |
| markAsRead | ブール値 | メッセージを開封済みにする必要があるかどうかを示します。 |
| markImportance | 重要性 | メッセージの重要性: `low`、`normal`、`high` を設定します。 |
| moveToFolder |  文字列| メッセージ移動先のフォルダーの ID です。 |
| permanentDelete | ブール値 | メッセージを完全に削除し、削除済みアイテム フォルダーにメッセージを保存しないようにするかどうかを示します。 |
| redirectTo | [recipient](recipient.md) コレクション | メッセージのリダイレクト先の電子メール アドレスです。 |
| stopProcessingRules | ブール値 | 後続のルールを評価する必要があるかどうかを示します。 |

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [
   ],
  "@odata.type": "microsoft.graph.messageRuleActions"
}-->

```json
{
  "assignCategories": ["String"],
  "copyToFolder": "String",
  "delete": "Boolean",
  "forwardAsAttachmentTo": [{"@odata.type": "microsoft.graph.recipient"}],
  "forwardTo": [{"@odata.type": "microsoft.graph.recipient"}],
  "markAsRead": "Boolean",
  "markImportance": "String",
  "moveToFolder": "String",
  "permanentDelete": "Boolean",
  "redirectTo": [{"@odata.type": "microsoft.graph.recipient"}],
  "stopProcessingRules": "Boolean"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "messageRuleActions resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->