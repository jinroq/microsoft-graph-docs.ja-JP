---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: DriveItem
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 9fa2f5cb9d40b0f8f12a5d1a6709eb03bf2975ba
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/08/2019
ms.locfileid: "30481490"
---
# <a name="driveitem-resource-type"></a>drive item リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**driveItem** リソースは、ドライブに格納されているファイル、フォルダーなどのアイテムを表します。OneDrive および SharePoint 内のすべてのファイル システム オブジェクトが、**driveItem** リソースとして返されます。

**driveItem** リソースのアドレス指定には、主に 2 つの方法があります。

* **** を使用した、`drive/items/{item-id}` 一意識別子による方法
* `/drive/root:/path/to/file` を使用した、ファイル システム パスによる方法

**DriveItem** リソースには、driveItem の ID および機能に関するデータを提供するプロパティとしてモデル化されたファセットがあります。例:

* フォルダーには、[**フォルダー ファセット **][folder] があります
* ファイルには、[**ファイル ファセット **][file] があります。
* 画像には[**画像ファセット **][image] とそのファイル ファセットがあります。
* カメラで撮影した画像 (写真) には[**写真ファセット **][photo] があります。写真ファセットは、アイテムを写真として識別し、撮影日時と撮影デバイスのプロパティを提供します。

**フォルダー** ファセットを持つアイテムは、アイテムのコンテナーとして機能するため、フォルダーに含まれる **driveItems** のコレクションを指す `children` 参照を持ちます。

## <a name="json-representation"></a>JSON 表記

以下は、**driveItem** リソースの JSON 表記です。

**driveItem** リソースは [**baseItem**][baseItem] から派生し、そのリソースからプロパティを継承します。

<!-- { "blockType": "resource", "@type": "microsoft.graph.driveItem", "@type.aka": "oneDrive.item",
       "baseType": "microsoft.graph.baseItem",
       "optionalProperties": ["cTag", "children", "folder", "file", "image", "audio", "video",
       "location", "deleted", "specialFolder", "photo", "thumbnails", "searchResult", "remoteItem",
       "shared", "content", "@microsoft.graph.conflictBehavior", "@microsoft.graph.downloadUrl", "@content.sourceUrl",
       "sharepointIds"],
       "keyProperty": "id", "openType": true } -->

```json
{
  "audio": { "@odata.type": "microsoft.graph.audio" },
  "cTag": "string (etag)",
  "deleted": { "@odata.type": "microsoft.graph.deleted"},
  "description": "string",
  "file": { "@odata.type": "microsoft.graph.file" },
  "fileSystemInfo": { "@odata.type": "microsoft.graph.fileSystemInfo" },
  "folder": { "@odata.type": "microsoft.graph.folder" },
  "image": { "@odata.type": "microsoft.graph.image" },
  "location": { "@odata.type": "microsoft.graph.geoCoordinates" },
  "package": { "@odata.type": "microsoft.graph.package" },
  "photo": { "@odata.type": "microsoft.graph.photo" },
  "publication": {"@odata.type": "microsoft.graph.publicationFacet"},
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
  "activities": [{"@odata.type": "microsoft.graph.itemActivity"}],
  "content": { "@odata.type": "Edm.Stream" },
  "children": [ { "@odata.type": "microsoft.graph.driveItem" }],
  "permissions": [ {"@odata.type": "microsoft.graph.permission"} ],
  "thumbnails": [ {"@odata.type": "microsoft.graph.thumbnailSet"}],
  "versions": [ {"@odata.type": "Collection(microsoft.graph.driveItemVersion)"}],

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

| プロパティ             | 種類               | 説明
|:---------------------|:-------------------|:---------------------------------
| audio                | [audio][]          | オーディオのメタデータ (アイテムがオーディオ ファイルである場合)。読み取り専用です。
| createdBy            | [identitySet][]    | そのアイテムを作成したユーザーの ID、デバイス、アプリケーション。読み取り専用です。
| createdDateTime      | DateTimeOffset     | アイテム作成の日時。読み取り専用です。
| cTag                 | String
             | アイテムのコンテンツの eTag。メタデータのみが変更された場合、この eTag は変更されません。**注:** アイテムがフォルダーである場合、このプロパティは返されません。読み取り専用です。
| deleted              | [deleted][]        | アイテムの削除状態に関する情報。読み取り専用です。
| description          | String             | ユーザーに表示されるアイテムの説明を提供します。読み取り/書き込み。OneDrive 個人用においてのみ
| eTag                 | String
             | アイテム全体 (メタデータおよびコンテンツ) の eTag。読み取り専用です。
| file                 | [file][]           | ファイルのメタデータ (アイテムがファイルである場合)。読み取り専用です。
| fileSystemInfo       | [fileSystemInfo][] | クライアント上のファイル システム情報。読み取り/書き込み。
| folder               | [フォルダー][]         | フォルダーのメタデータ (アイテムがフォルダーである場合)。読み取り専用です。
| id                   | String             | ドライブ内のアイテムの一意識別子。読み取り専用です。
| image                | [image][]          | 画像のメタデータ (アイテムが画像である場合)。読み取り専用です。
| lastModifiedBy       | [identitySet][]    | アイテムを最終更新したユーザーの ID、デバイス、アプリケーション。読み取り専用です。
| lastModifiedDateTime | DateTimeOffset     | アイテムが最後に変更された日時。読み取り専用です。
| location             | [geoCoordinates][] | 場所のメタデータ (アイテムに場所データが含まれている場合)。読み取り専用です。
| name                 | String
             | アイテムの名前 (ファイル名と拡張子)。読み取り/書き込み。
| package              | [package][]        | これがある場合、アイテムはフォルダーやファイルではなく、パッケージです。パッケージは、コンテキスト次第で、ファイルとして、あるいはフォルダーとして扱われます。読み取り専用です。
| parentReference      | [itemReference][]  | 親の情報 (アイテムに親がある場合)。読み取り/書き込み。
| 写真                | [photo][]          | 写真のメタデータ (アイテムが写真である場合)。読み取り専用です。
| publication          | [publicationFacet][] | アイテムが公開されているか、チェックアウトの状態かどうかの情報を、そのような操作をサポートする場所で提供します。 既定では、このプロパティは返されません。 読み取り専用です。 |
| remoteItem           | [remoteItem][]     | リモート アイテムのデータ (現在アクセス中のドライブ以外のドライブから共有されているアイテムの場合)。読み取り専用です。
| root                 | [root][]           | このプロパティが null ではない場合は、driveItem がドライブで最上位の driveItem であることを示します。
| searchResult         | [searchResult][]   | 検索のメタデータ (検索結果に由来するアイテムの場合)。読み取り専用です。
| 共有               | [shared][]         | アイテムが他のユーザーと共有されていることを示し、アイテムの共有状態に関する情報を提供します。読み取り専用です。
| sharepointIds        | [sharepointIds][]  | SharePoint REST 互換性に役立つ識別子を返します。読み取り専用です。
| size                 | Int64              | アイテムのサイズ (バイト単位)。読み取り専用です。
| specialFolder        | [specialFolder][]  | 現在のアイテムが特別なフォルダーとしても使用可能な場合は、このファセットが返されます。読み取り専用です。
| video                | [video][]          | ビデオのメタデータ (アイテムがビデオである場合)。読み取り専用です。
| webDavUrl            | String             | アイテムの WebDAV 互換性のある URL。
| webUrl               | 文字列             | ブラウザーでリソースを表示するための URL。読み取り専用です。

**注:** eTag プロパティと cTag プロパティは、コンテナー (フォルダー) 上での機能が異なります。cTag 値は、フォルダーのいずれかの子孫のコンテンツまたはメタデータが変更されると変更されます。eTag 値は、子孫から派生したプロパティ (**childCount** や **lastModifiedDateTime** など) 以外のフォルダーのプロパティが変更されたときにのみ、変更されます。

## <a name="relationships"></a>リレーションシップ

| リレーションシップ       | 種類                            | 説明
|:-------------------|:--------------------------------|:--------------------------
| アクティビティ         | [itemActivity][] コレクション     | このアイテムに対して行われた最近のアクティビティのリストです。
| 分析          | [itemanalytics][]リソース      | このアイテムに対して行われたビューアクティビティに関する分析。
| content            | Stream                          | コンテンツのストリーム (アイテムがファイルを表す場合)。
| children           | driveitem コレクション            | アイテムの直接の子のアイテム オブジェクトを格納するコレクション。子が含まれるのは、フォルダーを表すアイテムのみです。読み取り専用です。Null 許容型。
| listItem           | [listItem][]                    | SharePoint のドライブの場合は、関連付けられているドキュメントライブラリのリストアイテム。 読み取り専用。 Null 許容型。
| アクセス許可        | [permission][] コレクション       | アイテムのアクセス許可のセット。読み取り専用です。Null 許容型。
| thumbnails         | [thumbnailSet][] コレクション     | アイテムに関連付けられた [ThumbnailSet][] オブジェクトを格納するコレクション。詳細については、[サムネイルの取得][]についてのページを参照してください。読み取り専用です。Null 許容型。
| 最新           | [drive itemversion][]コレクション | アイテムの以前のバージョンのリスト。 詳細については、「[以前のバージョンを取得][]する」を参照してください。 読み取り専用です。 Null 許容型。

## <a name="instance-attributes"></a>インスタンスの属性

インスタンスの属性は、動作が特殊なプロパティです。これらのプロパティは一時的なものであり、a) サービスの動作を定義するか、b) 短期的なプロパティの値 (有効期限を持つアイテムのダウンロード URL など) を提供します。

| プロパティ名                     | 種類   | 説明
|:----------------------------------|:-------|:--------------------------------
| @microsoft.graph.conflictBehavior | string | 新しいアイテムを作成するアクションの競合を解決する動作。*fail*、*replace*、*rename* という値を使用できます。PUT の既定値は *replace* です。この注釈とともにアイテムが返されることはありません。書き込み専用です。
| @microsoft.graph.downloadUrl      | string | このファイルのコンテンツをダウンロードするために使用できる URL。この URL では認証は必要ありません。読み取り専用です。
| @microsoft.graph.sourceUrl        | string | PUT 要求を発行するときにこのインスタンスの注釈を使用すると、サービスに対し、URL のコンテンツをダウンロードし、それをファイルとして保存するように指示できます。書き込み専用です。

**注:**@microsoft.graph.downloadUrl の値は短時間限定の URL であるため、キャッシュすることはできません。
URL は短い期間 (1 時間) だけ使用でき、その後は無効になります。 ユーザーのファイルアクセス許可を削除しても、その URL はすぐに無効になることはありません。

## <a name="methods"></a>メソッド

| メソッド                                                   | REST パス
|:---------------------------------------------------------|:------------------
| [アイテムを取得する](../api/driveitem-get.md)                      | `GET /drive/items/{item-id}`
| [アクティビティを一覧表示する](../api/activities-list.md)             | `GET /drive/items/{item-id}/activities`
| [分析を取得する][]                                        | `GET /drive/items/{item-id}/analytics`
| [間隔でアクティビティを取得する][]                           | `GET /drive/items/{item-id}/getActivitiesByInterval`
| [子を一覧表示する](../api/driveitem-list-children.md)       | `GET /drive/items/{item-id}/children`
| [バージョンを一覧表示する](../api/driveitem-list-versions.md)       | `GET /drive/items/{item-id}/versions`
| [アイテムを作成する](../api/driveitem-post-children.md)         | `POST /drive/items/{item-id}/children`
| [アイテムを更新する](../api/driveitem-update.md)                | `PATCH /drive/items/{item-id}`
| [コンテンツをアップロードする](../api/driveitem-put-content.md)        | `PUT /drive/items/{item-id}/content`
| [コンテンツをダウンロードする](../api/driveitem-get-content.md)      | `GET /drive/items/{item-id}/content`
| [特定のファイル形式をダウンロードする][download-format]         | `GET /drive/items/{item-id}/content?format={format}`
| [アイテムを削除する](../api/driveitem-delete.md)                | `DELETE /drive/items/{item-id}`
| [アイテムを移動する](../api/driveitem-move.md)                    | `PATCH /drive/items/{item-id}`
| [アイテムをコピーする](../api/driveitem-copy.md)                    | `POST /drive/items/{item-id}/copy`
| [アイテムを検索する](../api/driveitem-search.md)               | `GET /drive/items/{item-id}/search(q='text')`
| [ドライブ内の変更内容を一覧表示する](../api/driveitem-delta.md)     | `GET /drive/root/delta`
| [サムネイルを一覧表示する](../api/driveitem-list-thumbnails.md)   | `GET /drive/items/{item-id}/thumbnails`
| [共有リンクを作成する](../api/driveitem-createlink.md)    | `POST /drive/items/{item-id}/createLink`
| [アクセス許可を追加する](../api/driveitem-invite.md)            | `POST /drive/items/{item-id}/invite`
| [アクセス許可を一覧表示する](../api/driveitem-list-permissions.md) | `GET /drive/items/{item-id}/permissions`
| [アクセス許可を削除する](../api/permission-delete.md)         | `DELETE /drive/items/{item-id}/permissions/{perm-id}`
| [WebSocket チャネルの取得][getWebSocket]                    | `GET /drive/root/subscriptions/socketIo`
| [アイテムのプレビュー][item-preview]                             | `POST /drive/items/{item-id}/preview`

[item-preview]: ../api/driveitem-preview.md
[分析を取得する]: ../api/itemanalytics-get.md
[間隔でアクティビティを取得する]: ../api/itemactivity-getbyinterval.md

## <a name="remarks"></a>備考

OneDrive for Business または SharePoint のドキュメント ライブラリでは、**driveItem** に[フォルダー][] ファセットがある場合、**cTag** プロパティは返されません。

[audio]: audio.md
[baseItem]: baseitem.md
[deleted]: deleted.md
[download-format]: ../api/driveitem-get-content-format.md
[driveItemVersion]: driveitemversion.md
[file]: file.md
[fileSystemInfo]: filesysteminfo.md
[folder]: folder.md
[以前のバージョンの取得]: ../api/driveitem-list-versions.md
[サムネイルの取得]: ../api/driveitem-list-thumbnails.md
[getWebSocket]: ../api/driveitem-subscriptions-socketio.md
[identitySet]: identityset.md
[image]: image.md
[itemActivity]: itemactivity.md
[itemanalytics]: itemanalytics.md
[itemReference]: itemreference.md
[geoCoordinates]: geocoordinates.md
[List activities]: ../api/activities-list.md
[listItem]: listitem.md
[package]: package.md
[permission]: permission.md
[photo]: photo.md
[remoteItem]: remoteitem.md
[root]: root.md
[searchResult]: searchresult.md
[shared]: shared.md
[sharepointIds]: sharepointids.md
[specialFolder]: specialfolder.md
[thumbnailSet]: thumbnailset.md
[video]: video.md
[user]: https://developer.microsoft.com/graph/docs/api-reference/v1.0/resources/users
[publicationFacet]: publicationfacet.md

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Item is the main data model in the OneDrive API. Everything is an item.",
  "keywords": "item,facet,resource",
  "section": "documentation",
  "tocPath": "Items",
  "tocBookmarks": {
    "Resources/Item": "#"
  },
  "suppressions": [
    "Error: /api-reference/beta/resources/driveitem.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
