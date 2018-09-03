---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: DriveItem
ms.openlocfilehash: 60f2d58331f349f9990f78f36f04df055ce90b9e
ms.sourcegitcommit: abf4b739257e3ffd9d045f783ec595d846172590
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/21/2018
ms.locfileid: "23269839"
---
# <a name="driveitem-resource-type"></a>DriveItem リソース型

**driveItem** リソースは、ドライブに格納されているファイル、フォルダーなどのアイテムを表します。OneDrive および SharePoint 内のすべてのファイル システム オブジェクトが、**driveItem** リソースとして返されます。

**driveItem** リソースのアドレス指定には、主に 2 つの方法があります。

* を使用した、**driveItem** 一意識別子による方法 `drive/items/{item-id}`
* を使用した、ファイル システム パスによる方法 `/drive/root:/path/to/file`

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
  "content": { "@odata.type": "Edm.Stream" },
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
  "children": [{ "@odata.type": "microsoft.graph.driveItem" }],
  "createdByUser": { "@odata.type": "microsoft.graph.user" },
  "lastModifiedByUser": { "@odata.type": "microsoft.graph.user" },
  "permissions": [ {"@odata.type": "microsoft.graph.permission"} ],
  "thumbnails": [ {"@odata.type": "microsoft.graph.thumbnailSet"}],
  "versions": [ {"@odata.type": "microsoft.graph.driveItemVersion"}],

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

| プロパティ             | タイプ               | 説明
|:---------------------|:-------------------|:---------------------------------
| オーディオ                | [オーディオ][]          | オーディオのメタデータ (アイテムがオーディオ ファイルである場合)。読み取り専用です。
| コンテンツ              | ストリーム             | コンテンツのストリーム (アイテムがファイルを表す場合)。
| createdBy            | [identitySet][]    | そのアイテムを作成したユーザーの ID、デバイス、アプリケーション。読み取り専用です。
| createdDateTime      | DateTimeOffset     | アイテム作成の日時。読み取り専用です。
| cTag                 | 文字列             | アイテムのコンテンツの eTag。メタデータのみが変更された場合、この eTag は変更されません。**注:** アイテムがフォルダーである場合、このプロパティは返されません。読み取り専用です。
| 削除済み              | [削除済み][]        | アイテムの削除状態に関する情報。読み取り専用です。
| 説明          | 文字列             | ユーザーに表示されるアイテムの説明を提供します。読み取り/書き込み。OneDrive 個人用においてのみ
| eTag                 | 文字列             | アイテム全体 (メタデータおよびコンテンツ) の eTag。読み取り専用です。
| ファイル                 | [ファイル][]           | ファイルのメタデータ (アイテムがファイルである場合)。読み取り専用です。
| fileSystemInfo       | [fileSystemInfo][] | クライアント上のファイル システム情報。読み取り/書き込み。
| フォルダー               | [フォルダー][]         | フォルダーのメタデータ (アイテムがフォルダーである場合)。読み取り専用です。
| ID                   | 文字列             | ドライブ内のアイテムの一意識別子。読み取り専用です。
| イメージ                | [イメージ][]          | 画像のメタデータ (アイテムが画像である場合)。読み取り専用です。
| lastModifiedBy       | [identitySet][]    | アイテムを最終更新したユーザーの ID、デバイス、アプリケーション。読み取り専用です。
| lastModifiedDateTime | DateTimeOffset     | アイテムが最後に変更された日時。読み取り専用です。
| 場所             | [geoCoordinates][] | 場所のメタデータ (アイテムに場所データが含まれている場合)。読み取り専用です。
| 名前                 | 文字列             | アイテムの名前 (ファイル名と拡張子)。読み取り/書き込み。
| パッケージ              | [パッケージ][]        | これがある場合、アイテムはフォルダーやファイルではなく、パッケージです。パッケージは、コンテキスト次第で、ファイルとして、あるいはフォルダーとして扱われます。読み取り専用です。
| parentReference      | [itemReference][]  | 親の情報 (アイテムに親がある場合)。読み取り/書き込み。
| 写真                | [写真][]          | 写真のメタデータ (アイテムが写真である場合)。読み取り専用です。
| パブリケーション          | [publicationFacet][] | アイテムが公開されているか、チェックアウトの状態かどうかの情報を、そのような操作をサポートする場所で提供します。 既定では、このプロパティは返されません。 読み取り専用です。 |
| remoteItem           | [remoteItem][]     | リモート アイテムのデータ (現在アクセス中のドライブ以外のドライブから共有されているアイテムの場合)。読み取り専用です。
| ルート                 | [ルート][]           | このプロパティが null ではない場合は、driveItem がドライブで最上位の driveItem であることを示します。
| searchResult         | [searchResult][]   | 検索のメタデータ (検索結果に由来するアイテムの場合)。読み取り専用です。
| 共有済み               | [共有済み][]         | アイテムが他のユーザーと共有されていることを示し、アイテムの共有状態に関する情報を提供します。読み取り専用です。
| sharepointIds        | [sharepointIds][]  | SharePoint REST 互換性に役立つ識別子を返します。読み取り専用です。
| サイズ                 | Int64              | アイテムのサイズ (バイト単位)。読み取り専用です。
| specialFolder        | [specialFolder][]  | 現在のアイテムが特別なフォルダーとしても使用可能な場合は、このファセットが返されます。読み取り専用です。
| ビデオ                | [ビデオ][]          | ビデオのメタデータ (アイテムがビデオである場合)。読み取り専用です。
| webDavUrl            | 文字列             | アイテムの WebDAV 互換性のある URL。
| webUrl               | 文字列             | ブラウザーでリソースを表示するための URL。読み取り専用です。

**注:** eTag プロパティと cTag プロパティは、コンテナー (フォルダー) 上での機能が異なります。cTag 値は、フォルダーのいずれかの子孫のコンテンツまたはメタデータが変更されると変更されます。eTag 値は、子孫から派生したプロパティ (**childCount** や **lastModifiedDateTime** など) 以外のフォルダーのプロパティが変更されたときにのみ、変更されます。

## <a name="relationships"></a>リレーションシップ

| リレーションシップ       | 型                        | 説明
|:-------------------|:----------------------------|:--------------------------
| 子           | driveitem コレクション        | アイテムの直接の子のアイテム オブジェクトを格納するコレクション。子が含まれるのは、フォルダーを表すアイテムのみです。読み取り専用です。Null 許容型。
| createdByUser      | [ユーザー][]                    | アイテムを作成したユーザーの ID です。 読み取り専用です。
| lastModifiedByUser | [ユーザー][]                    | アイテムを最後に変更したユーザーの ID です。 読み取り専用。
| listItem           | [listItem][]                | SharePoint のドライブ用の、関連付けられたドキュメント ライブラリのリスト アイテムです。 読み取り専用。 Null 許容型。
| アクセス許可        | [permission][] コレクション   | アイテムのアクセス許可のセット。読み取り専用です。Null 許容型。
| サムネイル         | [thumbnailSet][] コレクション | アイテムに関連付けられた [ThumbnailSet][] オブジェクトを格納するコレクション。詳細については、[サムネイルの取得][]についてのページをご覧ください。読み取り専用です。Null 許容型。
| バージョン           | [driveItemVersion][] コレクション | 項目の以前のバージョンの一覧です。 詳細については、「[以前のバージョンを取得する][]」を参照してください。 読み取り専用。 Null 許容型。
| ブック           | [ブック][]                | ファイルが Excel のスプレッドシートである場合、スプレッドシートのコンテンツを扱うためにブック API にアクセスします。 Null 許容型。

## <a name="instance-attributes"></a>インスタンスの属性

インスタンスの属性は、動作が特殊なプロパティです。これらのプロパティは一時的なものであり、a) サービスの動作を定義するか、b) 短期的なプロパティの値 (有効期限を持つアイテムのダウンロード URL など) を提供します。

| プロパティ名                     | 型   | 説明
|:----------------------------------|:-------|:--------------------------------
| @microsoft.graph.conflictBehavior | 文字列 | 新しいアイテムを作成するアクションの競合を解決する動作。*fail*、*replace*、*rename* という値を使用できます。PUT の既定値は *replace* です。この注釈とともにアイテムが返されることはありません。書き込み専用です。
| @microsoft.graph.downloadUrl      | 文字列 | このファイルのコンテンツをダウンロードするために使用できる URL。この URL では認証は必要ありません。読み取り専用です。
| @microsoft.graph.sourceUrl        | 文字列 | PUT 要求を発行するときにこのインスタンスの注釈を使用すると、サービスに対し、URL のコンテンツをダウンロードし、それをファイルとして保存するように指示できます。書き込み専用です。

**注:**@microsoft.graph.downloadUrl の値は短時間限定の URL であるため、キャッシュすることはできません。URL は短い期間 (1 時間) だけ使用でき、その後は無効になります。

## <a name="methods"></a>メソッド

| メソッド                                                   | REST パス
|:---------------------------------------------------------|:------------------
| [アイテムを取得する](../api/driveitem_get.md)                      | `GET /drive/items/{item-id}`
| [子を一覧表示する](../api/driveitem_list_children.md)       | `GET /drive/items/{item-id}/children`
| [バージョンの一覧表示](../api/driveitem_list_versions.md)       | `GET /drive/items/{item-id}/versions`
| [アイテムを作成する](../api/driveitem_post_children.md)         | `POST /drive/items/{item-id}/children`
| [アイテムを更新する](../api/driveitem_update.md)                | `PATCH /drive/items/{item-id}`
| [コンテンツをアップロードする](../api/driveitem_put_content.md)        | `PUT /drive/items/{item-id}/content`
| [コンテンツをダウンロードする](../api/driveitem_get_content.md)      | `GET /drive/items/{item-id}/content`
| [特定のファイル形式をダウンロードする][download-format]         | `GET /drive/items/{item-id}/content?format={format}`
| [アイテムを削除する](../api/driveitem_delete.md)                | `DELETE /drive/items/{item-id}`
| [アイテムを移動する](../api/driveitem_move.md)                    | `PATCH /drive/items/{item-id}`
| [アイテムをコピーする](../api/driveitem_copy.md)                    | `POST /drive/items/{item-id}/copy`
| [アイテムを検索する](../api/driveitem_search.md)               | `GET /drive/items/{item-id}/search(q='text')`
| [ドライブ内の変更内容を一覧表示する](../api/driveitem_delta.md)     | `GET /drive/root/delta`
| [サムネイルを一覧表示する](../api/driveitem_list_thumbnails.md)   | `GET /drive/items/{item-id}/thumbnails`
| [共有リンクを作成する](../api/driveitem_createlink.md)    | `POST /drive/items/{item-id}/createLink`
| [アクセス許可を追加する](../api/driveitem_invite.md)            | `POST /drive/items/{item-id}/invite`
| [アクセス許可を一覧表示する](../api/driveitem_list_permissions.md) | `GET /drive/items/{item-id}/permissions`
| [アクセス許可を削除する](../api/permission_delete.md)         | `DELETE /drive/items/{item-id}/permissions/{perm-id}`


## <a name="remarks"></a>備考

OneDrive for Business または SharePoint のドキュメント ライブラリでは、**driveItem** に[フォルダー][] ファセットがある場合、**cTag** プロパティは返されません。

[オーディオ]: audio.md
[baseItem]: baseItem.md
[削除済み]: deleted.md
[download-format]: ../api/driveitem_get_content_format.md
[driveItemVersion]: driveItemVersion.md
[ファイル]: file.md
[fileSystemInfo]: fileSystemInfo.md
[フォルダー]: folder.md
[以前のバージョンを取得する]: ../api/driveitem_list_versions.md
[サムネイルの取得]: ../api/driveitem_list_thumbnails.md
[identitySet]: identitySet.md
[イメージ]: image.md
[itemReference]: itemReference.md
[geoCoordinates]: geoCoordinates.md
[listItem]: listItem.md
[パッケージ]: package.md
[アクセス許可]: permission.md
[写真]: photo.md
[remoteItem]: remoteItem.md
[ルート]: root.md
[searchResult]: searchResult.md
[共有]: shared.md
[sharepointIds]: sharepointIds.md
[specialFolder]: specialFolder.md
[thumbnailSet]: thumbnailSet.md
[ビデオ]: video.md
[ブック]: workbook.md
[ユーザー]: https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/users
[publicationFacet]: publicationfacet.md

<!-- {
  "type": "#page.annotation",
  "description": "Item is the main data model in the OneDrive API. Everything is an item.",
  "keywords": "item,facet,resource",
  "section": "documentation",
  "tocPath": "Items",
  "tocBookmarks": { "Resources/Item": "#" }
} -->
