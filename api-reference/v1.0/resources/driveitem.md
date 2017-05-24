# <a name="driveitem-resource-type"></a>DriveItem リソースの種類

**driveItem** リソースは、ドライブに格納されているファイル、フォルダーなどのアイテムを表します。OneDrive および SharePoint 内のすべてのファイル システム オブジェクトが、**driveItem** リソースとして返されます。

**driveItem** リソースのアドレス指定には、主に 2 つの方法があります。

* `drive/items/{item-id}` を使用した、**driveItem** 一意識別子による方法
* `/drive/root:/path/to/file` を使用した、ファイル システム パスによる方法

**DriveItem** リソースには、driveItem の ID および機能に関するデータを提供するプロパティとしてモデル化されたファセットがあります。次に例を示します。

* フォルダーには、[**フォルダー ファセット**](folder.md) があります
* ファイルには、[**ファイル ファセット**](file.md)があります。
* 画像にはファイル ファセットだけでなく、[**画像ファセット**](image.md)もあります。
* カメラで撮影した画像 (写真) には[**写真ファセット**](photo.md)があります。写真ファセットは、アイテムを写真として識別し、撮影日時と撮影デバイスのプロパティを提供します。

**フォルダー** ファセットを持つアイテムは、アイテムのコンテナーとして機能するため、フォルダーに含まれる **driveItems** のコレクションを指す `children` 参照を持ちます。

## <a name="json-representation"></a>JSON 表記

以下は、**driveItem** リソースの JSON 表記です。

**driveItem** リソースは [**baseItem**](baseitem.md) から派生し、そのリソースからプロパティを継承します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [ "children", "createdByUser", "lastModifiedByUser", "permissions", "thumbnails"],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.driveItem"
}-->

```json
{
  "audio": { "@odata.type": "microsoft.graph.audio" },
  "cTag": "string",
  "deleted": { "@odata.type": "microsoft.graph.deleted" },
  "description": "string",
  "file": { "@odata.type": "microsoft.graph.file" },
  "fileSystemInfo": { "@odata.type": "microsoft.graph.fileSystemInfo" },
  "folder": { "@odata.type": "microsoft.graph.folder" },
  "image": { "@odata.type": "microsoft.graph.image" },
  "location": { "@odata.type": "microsoft.graph.geoCoordinates" },
  "package": { "@odata.type": "microsoft.graph.package" },
  "photo": { "@odata.type": "microsoft.graph.photo" },
  "remoteItem": { "@odata.type": "microsoft.graph.remoteItem" },
  "root": { "@odata.type": "microsoft.graph.root" },
  "searchResult": { "@odata.type": "microsoft.graph.searchResult" },
  "shared": { "@odata.type": "microsoft.graph.shared" },
  "sharepointIds": { "@odata.type": "microsoft.graph.sharepointIds" },
  "size": 1024,
  "specialFolder": { "@odata.type": "microsoft.graph.specialFolder" },
  "video": { "@odata.type": "microsoft.graph.video" },
  "webDavUrl": "string",

  /* relationships */
  "content": { "@odata.type": "Edm.Stream" },
  "createdByUser": { "@odata.type": "microsoft.graph.user" },
  "lastModifiedByUser": { "@odata.type": "microsoft.graph.user" },
  "children": [ { "@odata.type": "microsoft.graph.driveItem" }],
  "thumbnails": [ {"@odata.type": "microsoft.graph.thumbnailSet"}],
  "permissions": [ {"@odata.type": "microsoft.graph.permission"} ],

  /* inherited from baseItem */
  "id": "string (identifier)",
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "createdDateTime": "String (timestamp)",
  "eTag": "string",
  "lastModifiedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "lastModifiedDateTime": "String (timestamp)",
  "name": "string",
  "parentReference": {"@odata.type": "microsoft.graph.itemReference"},
  "webUrl": "string",

  /* instance annotations */
  "@microsoft.graph.conflictBehavior": "string",
  "@microsoft.graph.downloadUrl": "url",
  "@microsoft.graph.sourceUrl": "url"
}

```

## <a name="properties"></a>プロパティ

| プロパティ             | 型                                | 説明                                                                                                                                                               |
| :------------------- | :---------------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| audio                | [audio](audio.md)                   | オーディオのメタデータ (アイテムがオーディオ ファイルである場合)。読み取り専用です。                                                                                                                  |
| createdBy            | [identitySet](identityset.md)       | そのアイテムを作成したユーザーの ID、デバイス、アプリケーション。読み取り専用です。                                                                                          |
| createdDateTime      | DateTimeOffset                      | アイテム作成の日時。読み取り専用です。                                                                                                                                |
| cTag                 | String                              | アイテムのコンテンツの eTag。メタデータのみが変更された場合、この eTag は変更されません。**注:** アイテムがフォルダーである場合、このプロパティは返されません。読み取り専用です。 |
| deleted              | [deleted](deleted.md)               | アイテムの削除状態に関する情報。読み取り専用です。                                                                                                               |
| 説明          | String                              | ユーザーに表示されるアイテムの説明を提供します。読み取り/書き込み。OneDrive 個人用においてのみ                                                                                    |
| eTag                 | String                              | アイテム全体 (メタデータおよびコンテンツ) の eTag。読み取り専用です。                                                                                                                 |
| file                 | [file](file.md)                     | ファイルのメタデータ (アイテムがファイルである場合)。読み取り専用です。                                                                                                                          |
| fileSystemInfo       | [fileSystemInfo](filesysteminfo.md) | クライアント上のファイル システム情報。読み取り/書き込み。                                                                                                                            |
| folder               | [folder](folder.md)                 | フォルダーのメタデータ (アイテムがフォルダーである場合)。読み取り専用です。                                                                                                                      |
| id                   | String                              | ドライブ内のアイテムの一意識別子。読み取り専用です。                                                                                                            |
| image                | [image](image.md)                   | 画像のメタデータ (アイテムが画像である場合)。読み取り専用です。                                                                                                                       |
| lastModifiedBy       | [identitySet](identityset.md)       | アイテムを最終更新したユーザーの ID、デバイス、アプリケーション。読み取り専用です。                                                                                    |
| lastModifiedDateTime | DateTimeOffset                      | アイテムが最後に変更された日時。読み取り専用です。                                                                                                                      |
| location             | [geoCoordinates](geoCoordinates.md) | 場所のメタデータ (アイテムに場所データが含まれている場合)。読み取り専用です。                                                                                                              |
| name                 | String                              | アイテムの名前 (ファイル名と拡張子)。読み取り/書き込み。                                                                                                                |
| package              | [package](package.md)               | これがある場合、アイテムはフォルダーやファイルではなく、パッケージです。パッケージは、コンテキスト次第で、ファイルとして、あるいはフォルダーとして扱われます。読み取り専用です。         |
| parentReference      | [itemReference](itemreference.md)   | 親の情報 (アイテムに親がある場合)。読み取り/書き込み。                                                                                                                 |
| 写真                | [photo](photo.md)                   | 写真のメタデータ (アイテムが写真である場合)。読み取り専用です。                                                                                                                        |
| remoteItem           | [remoteItem](remoteitem.md)         | リモート アイテムのデータ (現在アクセス中のドライブ以外のドライブから共有されているアイテムの場合)。読み取り専用です。                                                                        |
| root                 | [root](root.md)                     | このプロパティが null ではない場合は、driveItem がドライブで最上位の driveItem であることを示します。                                                                     |
| searchResult         | [searchResult](searchresult.md)     | 検索のメタデータ (検索結果に由来するアイテムの場合)。読み取り専用です。                                                                                                          |
| 共有               | [shared](shared.md)                 | アイテムが他のユーザーと共有されていることを示し、アイテムの共有状態に関する情報を提供します。読み取り専用です。                                               |
| sharepointIds        | [sharepointIds](sharepointids.md)   | SharePoint REST 互換性に役立つ識別子を返します。読み取り専用です。                                                                                                  |
| size                 | Int64                               | アイテムのサイズ (バイト単位)。読み取り専用です。                                                                                                                                     |
| specialFolder        | [specialFolder](specialfolder.md)   | 現在のアイテムが特別なフォルダーとしても使用可能な場合は、このファセットが返されます。読み取り専用です。                                                                             |
| video                | [video](video.md)                   | ビデオのメタデータ (アイテムがビデオである場合)。読み取り専用です。                                                                                                                        |
| webDavUrl            | String                              | アイテムの WebDAV 互換性のある URL。                                                                                                                                       |
| webUrl               | String                              | ブラウザーでリソースを表示するための URL。読み取り専用です。                                                                                                                 |

**注:**eTag プロパティと cTag プロパティは、コンテナー (フォルダー) 上での機能が異なります。cTag 値は、フォルダーのいずれかの子孫のコンテンツまたはメタデータが変更されると変更されます。eTag 値は、子孫から派生したプロパティ (**childCount** や **lastModifiedDateTime** など) 以外のフォルダーのプロパティが変更されたときにのみ、変更されます。

## <a name="relationships"></a>リレーションシップ

| リレーションシップ       | 型                                       | 説明                                                                                                                                                                       |
| :----------------- | :----------------------------------------- | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| content            | Stream                                     | コンテンツのストリーム (アイテムがファイルを表す場合)。                                                                                                                                |
| children           | [driveitem](driveitem.md) コレクション       | アイテムの直接の子のアイテム オブジェクトを格納するコレクション。子が含まれるのは、フォルダーを表すアイテムのみです。読み取り専用です。Null 許容型。                                        |
| createdByUser      | [user](user.md)                            | そのアイテムを作成したユーザーの ID、デバイス、アプリケーション。読み取り専用です。                                                                                                  |
| lastModifiedByUser | [user](user.md)                            | アイテムを最終更新したユーザーの ID、デバイス、アプリケーション。読み取り専用です。                                                                                            |
| アクセス許可        | [permission](permission.md) コレクション     | アイテムのアクセス許可のセット。読み取り専用です。Null 許容型。                                                                                                                         |
| thumbnails         | [thumbnailSet](thumbnailset.md) コレクション | アイテムに関連付けられた [ThumbnailSet](thumbnailSet.md) オブジェクトを格納するコレクション。詳細については、[サムネイルの取得](../api/thumbnailset_get.md)についてのページをご覧ください。読み取り専用です。Null 許容型。 |


## <a name="instance-attributes"></a>インスタンスの属性

インスタンスの属性は、動作が特殊なプロパティです。これらのプロパティは一時的なものであり、a) サービスの動作を定義するか、b) 短期的なプロパティの値 (有効期限を持つアイテムのダウンロード URL など) を提供します。

| プロパティ名                     | 種類   | 説明                                                                                                                                                         |
|:----------------------------------|:-------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| @microsoft.graph.conflictBehavior | string | 新しいアイテムを作成するアクションの競合を解決する動作。*fail*、*replace*、*rename* という値を使用できます。PUT の既定値は *replace* です。この注釈とともにアイテムが返されることはありません。書き込み専用です。                               |
| @microsoft.graph.downloadUrl      | string | このファイルのコンテンツをダウンロードするために使用できる URL。この URL では認証は必要ありません。読み取り専用です。                                                    |
| @microsoft.graph.sourceUrl        | string | PUT 要求を発行するときにこのインスタンスの注釈を使用すると、サービスに対し、URL のコンテンツをダウンロードし、それをファイルとして保存するように指示できます。書き込み専用です。 |

**注:**@microsoft.graph.downloadUrl の値は短時間限定の URL であるため、キャッシュすることはできません。URL は短い期間 (1 時間) だけ使用でき、その後は無効になります。


## <a name="methods"></a>メソッド

| Method                                                 | REST パス
|:-------------------------------------------------------|:--------------------
| [アイテムを取得する](../api/item_get.md)                         | `GET /drive/items/{item-id}`
| [子を一覧表示する](../api/item_list_children.md)          | `GET /drive/items/{item-id}/children`
| [アイテムを作成する](../api/item_post_children.md)            | `POST /drive/items/{item-id}/children`
| [アイテムを更新する](../api/item_update.md)                   | `PATCH /drive/items/{item-id}`
| [コンテンツをアップロードする](../api/item_uploadcontent.md)         | `PUT /drive/items/{item-id}/content`
| [コンテンツをダウンロードする](../api/item_downloadcontent.md)     | `GET /drive/items/{item-id}/content`
| [アイテムを削除する](../api/item_delete.md)                   | `DELETE /drive/items/{item-id}`
| [アイテムを移動する](../api/item_move.md)                       | `PATCH /drive/items/{item-id}`
| [アイテムをコピーする](../api/item_copy.md)                       | `POST /drive/items/{item-id}/copy`
| [アイテムを検索する](../api/item_search.md)                  | `GET /drive/items/{item-id}/search(q='text')`
| [ドライブ内の変更内容を一覧表示する](../api/item_delta.md)        | `GET /drive/root/delta`
| [サムネイルを一覧表示する](../api/item_list_thumbnails.md)      | `GET /drive/items/{item-id}/thumbnails`  |
| [共有リンクを作成する](../api/item_createlink.md)       | `POST /drive/items/{item-id}/createLink` |
| [アクセス許可を追加する](../api/item_invite.md)               | `POST /drive/items/{item-id}/invite`     |
| [アクセス許可を一覧表示する](../api/item_list_permissions.md)    | `GET /drive/items/{item-id}/permissions` |
| [アクセス許可を削除する](../api/permission_delete.md)       | `DELETE /drive/items/{item-id}/permissions/{perm-id}` |


## <a name="remarks"></a>備考

OneDrive for Business または SharePoint のドキュメント ライブラリでは、**driveItem** に [フォルダー](folder.md) ファセットがある場合、**cTag** プロパティは返されません。

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "item resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
