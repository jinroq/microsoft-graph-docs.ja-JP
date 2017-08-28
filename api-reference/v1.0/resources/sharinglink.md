# <a name="sharinglink-resource-type"></a>SharingLink リソースタイプ

**SharingLink** リソースは、リンク関連のデータ項目を 1 つの構造にグループ化します。

[**Permission**](permission.md) リソースが非 null の **sharingLink** ファセットを持つ場合、アクセス許可は (ユーザーやグループに与えられているアクセス許可ではなく) 共有リンクを表します。

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [ "application", "scope" ],
  "@odata.type": "microsoft.graph.sharingLink"
}-->

```json
{
  "application": {"@odata.type": "microsoft.graph.identity"},
  "type": "view | edit",
  "scope": "anonymous | organization",
  "webUrl": "url"
}
```

## <a name="properties"></a>プロパティ

| プロパティ    | 型                    | 説明                                                                                                                                                                                             |
|:------------|:------------------------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| application | [identity](identity.md) | リンクが関連付けられているアプリケーションです。                                                                                                                                                                    |
| type        | String                  | 作成されたリンクの種類。                                                                                                                                                                           |
| scope       | String                  | このアクセス許可によって表されるリンクの範囲です。値 `anonymous` は、すべてのユーザーがリンクを使用できることを示し、`organization` は同じテナントにサインインしたユーザーのみがリンクを使用できることを示します。 |
| webUrl      | String                  | OneDrive の web サイト上で、項目をブラウザーに開く URL です。                                                                                                                                       |

## <a name="type-enumeration"></a>Type 列挙

この表は、**type** プロパティの可能な値を定義します。

| 値   | ロール    | 説明                                                                     |
|:--------|:--------|:--------------------------------------------------------------------------------|
| `view`  | `read`  | 読み取り専用のアクセスを許可する、閲覧専用の共有リンクです。                            |
| `edit`  | `write` | 読み取り / 書き込みのアクセスを許可する、編集共有リンクです。                               |

## <a name="scope-enumeration"></a>スコープ列挙

| 値          | 説明                                                                                                                 |
|:---------------|:----------------------------------------------------------------------------------------------------------------------------|
| `anonymous`    | 共有リンクは誰でも使用可能です。                                                                            |
| `organization` | 共有リンクは、同じ組織 (テナント) 内のすべてのユーザーが使用可能です。OneDrive Personal では使用できません。 |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "sharingLink resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
