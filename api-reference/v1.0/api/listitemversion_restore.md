# <a name="restore-a-previous-version-of-a-listitem"></a>旧バージョンのリスト アイテムを復元する

旧バージョンのリスト アイテムを現在のバージョンに復元します。 旧バージョンのコンテンツを持つ新しいバージョンを作成します。しかし、アイテムの既存のバージョンはすべて保持されます。

## <a name="permissions"></a>アクセス許可

この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。

|            アクセス許可の種類             |         アクセス許可 (特権の小さいものから大きいものへ)          |
| :------------------------------------- | :----------------------------------------------------------- |
| 委任 (職場または学校のアカウント)     | Sites.ReadWrite.All、Sites.Manage.All、Sites.FullControl.All |
| 委任 (個人用 Microsoft アカウント) | 該当なし                                                          |
| アプリケーション                            | Sites.ReadWrite.All、Sites.Manage.All、Sites.FullControl.All |

## <a name="http-request"></a>HTTP 要求

<!-- { "blockType": "ignored" } -->

```http
POST /sites/{site-id}/items/{item-id}/versions/{version-id}/restoreVersion
POST /sites/{site-id}/lists/{list-id}/items/{item-id}/versions/{version-id}/restoreVersion
```

### <a name="request-body"></a>要求本文

要求の本文は必要ありません。

## <a name="example"></a>例

この例では、`{item-id}` と `{version-id}` で識別されるリスト アイテムのバージョンを復元します。

<!-- { "blockType": "request", "name": "restore-item-version-listItem", "scopes": "files.readwrite sites.readwrite.all", "target": "action", "tags": "service.graph service.sharepoint" } -->

```http
POST /sites/{site-id}/lists/{list-id}/items/{item-id}/versions/{version-id}/restoreVersion
```

## <a name="response"></a>応答

成功すると、API 呼び出しは `204 No Content` を返します。

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```

<!-- {
  "type": "#page.annotation",
  "description": "Create a copy of an existing item.",
  "keywords": "copy existing item",
  "section": "documentation",
  "tocPath": "Items/Copy"
} -->
