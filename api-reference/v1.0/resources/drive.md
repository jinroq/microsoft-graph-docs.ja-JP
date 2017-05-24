# <a name="drive-resource-type"></a>ドライブ リソースの種類

ドライブ リソースは、ユーザーの OneDrive または SharePoint のドキュメント ライブラリを表す、最上位のオブジェクトです。

OneDrive のユーザーは、少なくとも 1 つのドライブ (そのユーザーの既定のドライブ) を常に使用できます。OneDrive のライセンスが付与されていないユーザーには、使用可能な既定のドライブがないことがあります。

## <a name="json-representation"></a>JSON 表記

以下は、**ドライブ** リソースの JSON 表記です。

**drive** リソースは [**baseItem**](baseitem.md) から派生し、そのリソースからプロパティを継承します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [ "items", "root", "special", "owner", "description" ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.drive"
}-->

```json
{
  "id": "string (identifier)",
  "driveType": "string",
  "owner": {"@odata.type": "microsoft.graph.identitySet"},
  "quota": {"@odata.type": "microsoft.graph.quota"},
  "sharepointIds": { "@odata.type": "microsoft.graph.sharepointIds" },

  /* relationships */
  "root": {"@odata.type": "microsoft.graph.driveItem" },
  "items": [ {"@odata.type": "microsoft.graph.driveItem" }],
  "special": [ {"@odata.type": "microsoft.graph.driveItem" }],

  /* inherited from baseItem */
  "createdBy": { "@odata.type": "microsoft.graph.identitySet" },
  "createdDateTime": "datetime",
  "description": "string",
  "lastModifiedBy": { "@odata.type": "microsoft.graph.identitySet" },
  "lastModifiedDateTime": "datetime",
  "name": "string",
  "webUrl": "url"
}
```

## <a name="properties"></a>プロパティ

| プロパティ             | 型                          | 説明                                                                                                                                                                                                                      |
| :------------------- | :---------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| id                   | 文字列                        | ドライブの一意識別子。読み取り専用です。                                                                                                                                                                                   |
| createdBy            | [identitySet][]               | アイテムを作成したユーザーの ID、デバイス、アプリケーション。読み取り専用です。                                                                                                                                                  |
| createdDateTime      | dateTimeOffset                | アイテム作成の日時。読み取り専用です。                                                                                                                                                                                       |
| driveType            | String                        | このリソースで表されるドライブの種類についての説明。OneDrive 個人用のドライブは `personal` を返します。OneDrive for Business は `business` を返します。SharePoint ドキュメント ライブラリは `documentLibrary` を返します。読み取り専用。 |
| lastModifiedBy       | [identitySet][]               | アイテムを最終更新したユーザーの ID、デバイス、アプリケーション。読み取り専用です。                                                                                                                                           |
| lastModifiedDateTime | dateTimeOffset                | アイテムが最後に変更された日時。読み取り専用。                                                                                                                                                                             |
| name                 | string                        | アイテムの名前。読み取り/書き込み。                                                                                                                                                                                                |
| 所有者                | [identitySet](identityset.md) | 省略可能。ドライブを所有しているユーザー アカウント。読み取り専用です。                                                                                                                                                                       |
| クォータ                | [quota](quota.md)             | 省略可能。ドライブの記憶領域クォータに関する情報。読み取り専用です。                                                                                                                                                          |
| sharepointIds        | [sharepointIds][]             | SharePoint REST 互換性に役立つ識別子を返します。読み取り専用です。                                                                                                                                                         |
| webUrl               | string (URL)                  | ブラウザーでリソースを表示する URL。読み取り専用です。                                                                                                                                                                        |

[identitySet]: identityset.md
[sharepointIds]: sharepointids.md

## <a name="relationships"></a>リレーションシップ

| リレーションシップ | 型                                 | 説明                                                              |
| :----------- | :----------------------------------- | :----------------------------------------------------------------------- |
| items        | [driveitem](driveitem.md) コレクション | ドライブに含まれているすべてのアイテム。読み取り専用。Null 許容型。                   |
| root         | [driveitem](driveitem.md)            | ドライブのルート フォルダー。読み取り専用。                                 |
| special      | [driveitem](driveitem.md) コレクション | OneDrive で使用可能な共通フォルダーのコレクション。読み取り専用。Null 許容型。 |


## <a name="methods"></a>メソッド

次に、ドライブ リソースで使用可能なメソッドを示します。

| メソッド                                                | REST パス                        |
| :---------------------------------------------------- | :------------------------------- |
| [ユーザーの既定のドライブの取得](../api/drive_get.md)       | `GET /me/drive`                  |
| [別のユーザーのドライブの取得](../api/drive_get.md)       | `GET /users/{user-id}/drive`     |
| [ドライブのルート フォルダーの取得](../api/item_get.md)     | `GET /drives/{drive-id}/root`    |
| [ドライブ内のアイテムの一覧](../api/item_list_children.md) | `GET /me/drive/root/children`    |
| [ドライブ内の変更内容の一覧](../api/item_delta.md)       | `GET /me/drive/root/delta`       |
| [ドライブ内のアイテムの検索](../api/item_search.md)      | `GET /me/drive/search(q='text')` |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "drive resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "OneDrive/Drive"
}-->
