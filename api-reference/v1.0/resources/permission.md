# <a name="permission-resource-type"></a>Permission リソースタイプ

**Permission** リソースは、[DriveItem](driveitem.md) リソースに与えるアクセス許可についての情報を提供します。

アクセス許可にはさまざまなフォームがあります。**アクセス許可** リソースは、これらの異なるフォームをリソースのファセットを通じて表します。

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です

<!-- {
  "blockType": "resource",
  "optionalProperties": [ "link", "grantedTo", "invitation", "inheritedFrom", "shareId" ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.permission"
}-->
```json
{
  "id": "string (identifier)",
  "grantedTo": {"@odata.type": "microsoft.graph.identitySet"},
  "inheritedFrom": {"@odata.type": "microsoft.graph.itemReference"},
  "invitation": {"@odata.type": "microsoft.graph.sharingInvitation"},
  "link": {"@odata.type": "microsoft.graph.sharingLink"},
  "roles": ["string"],
  "shareId": "string"
}
```

## <a name="properties"></a>プロパティ

| プロパティ      | 型                                      | 説明                                                                                                                           |
|:--------------|:------------------------------------------|:--------------------------------------------------------------------------------------------------------------------------------------|
| id            | String                                    | 項目の全アクセス許可の中の、アクセス許可の一意の識別子です。読み取り専用。                                                 |
| grantedTo     | [IdentitySet](identityset.md)             | ユーザー タイプのアクセス許可、ユーザーとこのアクセス許可のアプリケーションの詳細。読み取り専用。                                    |
| invitation    | [SharingInvitation](sharinginvitation.md) | このアクセス許可に任意に関連付けられた共有招待状の詳細情報です。読み取り専用。                                                          |
| inheritedFrom | [ItemReference](itemreference.md)         | 現在のアクセス許可が先祖から継承されている場合、その先祖への参照を提供します。読み取り専用。                       |
| link          | [SharingLink](sharinglink.md)             | 現在のアクセス許可がリンク タイプのアクセス許可である場合は、そのリンクの詳細を提供します。読み取り専用。                                     |
| role          | Collection of String                      | `read` など、アクセス許可の種類。ロールの完全なリストは以下を参照してください。読み取り専用。                                                 |
| shareId       | String                                    | このアクセス許可に固有のトークンです。読み取り専用。 |

[アクセス権](../resources/permission.md)リソースは、_ファセット_を使用してリソースによって表されるアクセス許可の種類に関する情報を提供します。

[**リンク**](sharinglink.md) ファセットのあるアクセス許可は、項目上に作成された共有するリンクを表します。共有リンクは、リンクを持つすべてのユーザーのアイテムへのアクセス許可を提供する固有のトークンを含みます。

[**招待**](sharinginvitation.md) ファセットを持つアクセス許可は、指定のユーザーやグループをファイルへのアクセスへ招待することで追加されたアクセス許可を表します。

## <a name="roles-enumeration"></a>ロール列挙

| ロール  | 詳細                                                                        |
|:------|:-------------------------------------------------------------------------------|
| `read`  | 項目のメタデータと内容を読み取る機能を提供します。            |
| `write` | 項目のメタデータと内容の読み取りと改変の機能を提供します。 |

## <a name="methods"></a>メソッド

| Method                                              | REST パス                            |
|:----------------------------------------------------|:---------------------------------------|
| [アクセス許可を一覧表示する](../api/item_list_permissions.md) | `GET /drive/items/{item-id}/permissions`  |
| [アクセス許可を取得する](../api/permission_get.md)          | `GET /drive/items/{item-id}/permissions/{id}` |
| [追加](../api/item_invite.md)                        | `POST /drive/items/{item-id}/invite` |
| [更新する](../api/permission_update.md)               | `PATH /drive/items/{item-id}/permissions/{id}` |
| [削除](../api/permission_delete.md)               | `DELETE /drive/items/{item-id}/permissions/{id}` |


## <a name="remarks"></a>備考

OneDrive for Business と SharePoint ドキュメント ライブラリは、**inheritedFrom** プロパティを返しません。

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "permission resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
