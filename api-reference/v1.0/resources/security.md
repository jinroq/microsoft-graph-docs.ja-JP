# <a name="security-resource-type"></a>セキュリティ リソースの種類

セキュリティ リソースは、セキュリティ オブジェクト モデルのエントリ ポイントです。 シングルトンのセキュリティ リソースを返します。 使用可能なプロパティが含まれていません。

## <a name="methods"></a>メソッド

| メソッド       | 戻り値の型 | 説明 |
|:-------------|:------------|:------------|
| [警告の一覧表示](../api/alert_list.md) | [アラート](alert.md) のコレクション | 警告オブジェクトのコレクションを取得。 |
| [アラートを取得](../api/alert_get.md) | [アラート](alert.md) のコレクション | アラートオブジェクトを取得。 |
| [通知を更新](../api/alert_update.md) | [アラート](alert.md) のコレクション | アラートオブジェクトを取得。 |

## <a name="properties"></a>プロパティ
なし

## <a name="relationships"></a>関係
| リレーションシップ | 型        | 説明 |
|:-------------|:------------|:------------|
|アラート|[アラート](alert.md) のコレクション| 読み取り専用。Null 許容型。|


## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.security"
}-->

```json
{
}
```

## <a name="example"></a>例

**プランナー** のリソースは、グラフのルートに使用できます。

<!--{
  "blockType": "request"
}-->
```http
GET https://graph.microsoft.com/v1.0/security
```

<!--{
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.security"
}-->
```json
HTTP/1.1 200 OK
Content-type: application/json

{
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "security resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->