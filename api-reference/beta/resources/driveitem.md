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
# <a name="driveitem-resource-type"></a><span data-ttu-id="cfbd0-102">drive item リソースの種類</span><span class="sxs-lookup"><span data-stu-id="cfbd0-102">driveItem resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cfbd0-p101">**driveItem** リソースは、ドライブに格納されているファイル、フォルダーなどのアイテムを表します。OneDrive および SharePoint 内のすべてのファイル システム オブジェクトが、**driveItem** リソースとして返されます。</span><span class="sxs-lookup"><span data-stu-id="cfbd0-p101">The **driveItem** resource represents a file, folder, or other item stored in a drive. All file system objects in OneDrive and SharePoint are returned as **driveItem** resources.</span></span>

<span data-ttu-id="cfbd0-105">**driveItem** リソースのアドレス指定には、主に 2 つの方法があります。</span><span class="sxs-lookup"><span data-stu-id="cfbd0-105">There are two primary ways of addressing a **driveItem** resource:</span></span>

* <span data-ttu-id="cfbd0-106">\*\*\*\* を使用した、`drive/items/{item-id}` 一意識別子による方法</span><span class="sxs-lookup"><span data-stu-id="cfbd0-106">By the **driveItem** unique identifier using `drive/items/{item-id}`</span></span>
* <span data-ttu-id="cfbd0-107">`/drive/root:/path/to/file` を使用した、ファイル システム パスによる方法</span><span class="sxs-lookup"><span data-stu-id="cfbd0-107">By file system path using `/drive/root:/path/to/file`</span></span>

<span data-ttu-id="cfbd0-p102">**DriveItem** リソースには、driveItem の ID および機能に関するデータを提供するプロパティとしてモデル化されたファセットがあります。例:</span><span class="sxs-lookup"><span data-stu-id="cfbd0-p102">**DriveItem** resources have facets modeled as properties that provide data about the driveItem's identities and capabilities. For example:</span></span>

* <span data-ttu-id="cfbd0-110">フォルダーには、[\*\*フォルダー ファセット \*\*][folder] があります</span><span class="sxs-lookup"><span data-stu-id="cfbd0-110">Folders have a [**folder facet**][folder]</span></span>
* <span data-ttu-id="cfbd0-111">ファイルには、[\*\*ファイル ファセット \*\*][file] があります。</span><span class="sxs-lookup"><span data-stu-id="cfbd0-111">Files have a [**file facet**][file].</span></span>
* <span data-ttu-id="cfbd0-112">画像には[\*\*画像ファセット \*\*][image] とそのファイル ファセットがあります。</span><span class="sxs-lookup"><span data-stu-id="cfbd0-112">Images have an [**image facet**][image] in addition to their file facet.</span></span>
* <span data-ttu-id="cfbd0-113">カメラで撮影した画像 (写真) には[\*\*写真ファセット \*\*][photo] があります。写真ファセットは、アイテムを写真として識別し、撮影日時と撮影デバイスのプロパティを提供します。</span><span class="sxs-lookup"><span data-stu-id="cfbd0-113">Images taken with a camera (photos) have a [**photo facet**][photo] that identifies the item as a photo and provides the properties of when the photo was taken and with what device.</span></span>

<span data-ttu-id="cfbd0-114">**フォルダー** ファセットを持つアイテムは、アイテムのコンテナーとして機能するため、フォルダーに含まれる **driveItems** のコレクションを指す `children` 参照を持ちます。</span><span class="sxs-lookup"><span data-stu-id="cfbd0-114">Items with the **folder** facet act as containers of items and therefore have a `children` reference pointing to a collection of **driveItems** under the folder.</span></span>

## <a name="json-representation"></a><span data-ttu-id="cfbd0-115">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="cfbd0-115">JSON representation</span></span>

<span data-ttu-id="cfbd0-116">以下は、**driveItem** リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="cfbd0-116">Here is a JSON representation of a **driveItem** resource.</span></span>

<span data-ttu-id="cfbd0-117">**driveItem** リソースは [**baseItem**][baseItem] から派生し、そのリソースからプロパティを継承します。</span><span class="sxs-lookup"><span data-stu-id="cfbd0-117">The **driveItem** resource is derived from [**baseItem**][baseItem] and inherits properties from that resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="cfbd0-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cfbd0-118">Properties</span></span>

| <span data-ttu-id="cfbd0-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cfbd0-119">Property</span></span>             | <span data-ttu-id="cfbd0-120">種類</span><span class="sxs-lookup"><span data-stu-id="cfbd0-120">Type</span></span>               | <span data-ttu-id="cfbd0-121">説明</span><span class="sxs-lookup"><span data-stu-id="cfbd0-121">Description</span></span>
|:---------------------|:-------------------|:---------------------------------
| <span data-ttu-id="cfbd0-122">audio</span><span class="sxs-lookup"><span data-stu-id="cfbd0-122">audio</span></span>                | <span data-ttu-id="cfbd0-123">[audio][]</span><span class="sxs-lookup"><span data-stu-id="cfbd0-123">[audio][]</span></span>          | <span data-ttu-id="cfbd0-p103">オーディオのメタデータ (アイテムがオーディオ ファイルである場合)。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="cfbd0-p103">Audio metadata, if the item is an audio file. Read-only.</span></span>
| <span data-ttu-id="cfbd0-126">createdBy</span><span class="sxs-lookup"><span data-stu-id="cfbd0-126">createdBy</span></span>            | <span data-ttu-id="cfbd0-127">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="cfbd0-127">[identitySet][]</span></span>    | <span data-ttu-id="cfbd0-p104">そのアイテムを作成したユーザーの ID、デバイス、アプリケーション。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="cfbd0-p104">Identity of the user, device, and application which created the item. Read-only.</span></span>
| <span data-ttu-id="cfbd0-130">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="cfbd0-130">createdDateTime</span></span>      | <span data-ttu-id="cfbd0-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cfbd0-131">DateTimeOffset</span></span>     | <span data-ttu-id="cfbd0-p105">アイテム作成の日時。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="cfbd0-p105">Date and time of item creation. Read-only.</span></span>
| <span data-ttu-id="cfbd0-134">cTag</span><span class="sxs-lookup"><span data-stu-id="cfbd0-134">cTag</span></span>                 | <span data-ttu-id="cfbd0-135">String
</span><span class="sxs-lookup"><span data-stu-id="cfbd0-135">String</span></span>             | <span data-ttu-id="cfbd0-p106">アイテムのコンテンツの eTag。メタデータのみが変更された場合、この eTag は変更されません。**注:** アイテムがフォルダーである場合、このプロパティは返されません。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="cfbd0-p106">An eTag for the content of the item. This eTag is not changed if only the metadata is changed. **Note** This property is not returned if the item is a folder. Read-only.</span></span>
| <span data-ttu-id="cfbd0-140">deleted</span><span class="sxs-lookup"><span data-stu-id="cfbd0-140">deleted</span></span>              | <span data-ttu-id="cfbd0-141">[deleted][]</span><span class="sxs-lookup"><span data-stu-id="cfbd0-141">[deleted][]</span></span>        | <span data-ttu-id="cfbd0-p107">アイテムの削除状態に関する情報。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="cfbd0-p107">Information about the deleted state of the item. Read-only.</span></span>
| <span data-ttu-id="cfbd0-144">description</span><span class="sxs-lookup"><span data-stu-id="cfbd0-144">description</span></span>          | <span data-ttu-id="cfbd0-145">String</span><span class="sxs-lookup"><span data-stu-id="cfbd0-145">String</span></span>             | <span data-ttu-id="cfbd0-p108">ユーザーに表示されるアイテムの説明を提供します。読み取り/書き込み。OneDrive 個人用においてのみ</span><span class="sxs-lookup"><span data-stu-id="cfbd0-p108">Provides a user-visible description of the item. Read-write. Only on OneDrive Personal</span></span>
| <span data-ttu-id="cfbd0-149">eTag</span><span class="sxs-lookup"><span data-stu-id="cfbd0-149">eTag</span></span>                 | <span data-ttu-id="cfbd0-150">String
</span><span class="sxs-lookup"><span data-stu-id="cfbd0-150">String</span></span>             | <span data-ttu-id="cfbd0-p109">アイテム全体 (メタデータおよびコンテンツ) の eTag。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="cfbd0-p109">eTag for the entire item (metadata + content). Read-only.</span></span>
| <span data-ttu-id="cfbd0-153">file</span><span class="sxs-lookup"><span data-stu-id="cfbd0-153">file</span></span>                 | <span data-ttu-id="cfbd0-154">[file][]</span><span class="sxs-lookup"><span data-stu-id="cfbd0-154">[file][]</span></span>           | <span data-ttu-id="cfbd0-p110">ファイルのメタデータ (アイテムがファイルである場合)。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="cfbd0-p110">File metadata, if the item is a file. Read-only.</span></span>
| <span data-ttu-id="cfbd0-157">fileSystemInfo</span><span class="sxs-lookup"><span data-stu-id="cfbd0-157">fileSystemInfo</span></span>       | <span data-ttu-id="cfbd0-158">[fileSystemInfo][]</span><span class="sxs-lookup"><span data-stu-id="cfbd0-158">[fileSystemInfo][]</span></span> | <span data-ttu-id="cfbd0-p111">クライアント上のファイル システム情報。読み取り/書き込み。</span><span class="sxs-lookup"><span data-stu-id="cfbd0-p111">File system information on client. Read-write.</span></span>
| <span data-ttu-id="cfbd0-161">folder</span><span class="sxs-lookup"><span data-stu-id="cfbd0-161">folder</span></span>               | <span data-ttu-id="cfbd0-162">[フォルダー][]</span><span class="sxs-lookup"><span data-stu-id="cfbd0-162">[folder][]</span></span>         | <span data-ttu-id="cfbd0-p112">フォルダーのメタデータ (アイテムがフォルダーである場合)。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="cfbd0-p112">Folder metadata, if the item is a folder. Read-only.</span></span>
| <span data-ttu-id="cfbd0-165">id</span><span class="sxs-lookup"><span data-stu-id="cfbd0-165">id</span></span>                   | <span data-ttu-id="cfbd0-166">String</span><span class="sxs-lookup"><span data-stu-id="cfbd0-166">String</span></span>             | <span data-ttu-id="cfbd0-p113">ドライブ内のアイテムの一意識別子。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="cfbd0-p113">The unique identifier of the item within the Drive. Read-only.</span></span>
| <span data-ttu-id="cfbd0-169">image</span><span class="sxs-lookup"><span data-stu-id="cfbd0-169">image</span></span>                | <span data-ttu-id="cfbd0-170">[image][]</span><span class="sxs-lookup"><span data-stu-id="cfbd0-170">[image][]</span></span>          | <span data-ttu-id="cfbd0-p114">画像のメタデータ (アイテムが画像である場合)。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="cfbd0-p114">Image metadata, if the item is an image. Read-only.</span></span>
| <span data-ttu-id="cfbd0-173">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="cfbd0-173">lastModifiedBy</span></span>       | <span data-ttu-id="cfbd0-174">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="cfbd0-174">[identitySet][]</span></span>    | <span data-ttu-id="cfbd0-p115">アイテムを最終更新したユーザーの ID、デバイス、アプリケーション。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="cfbd0-p115">Identity of the user, device, and application which last modified the item. Read-only.</span></span>
| <span data-ttu-id="cfbd0-177">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="cfbd0-177">lastModifiedDateTime</span></span> | <span data-ttu-id="cfbd0-178">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cfbd0-178">DateTimeOffset</span></span>     | <span data-ttu-id="cfbd0-p116">アイテムが最後に変更された日時。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="cfbd0-p116">Date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="cfbd0-181">location</span><span class="sxs-lookup"><span data-stu-id="cfbd0-181">location</span></span>             | <span data-ttu-id="cfbd0-182">[geoCoordinates][]</span><span class="sxs-lookup"><span data-stu-id="cfbd0-182">[geoCoordinates][]</span></span> | <span data-ttu-id="cfbd0-p117">場所のメタデータ (アイテムに場所データが含まれている場合)。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="cfbd0-p117">Location metadata, if the item has location data. Read-only.</span></span>
| <span data-ttu-id="cfbd0-185">name</span><span class="sxs-lookup"><span data-stu-id="cfbd0-185">name</span></span>                 | <span data-ttu-id="cfbd0-186">String
</span><span class="sxs-lookup"><span data-stu-id="cfbd0-186">String</span></span>             | <span data-ttu-id="cfbd0-p118">アイテムの名前 (ファイル名と拡張子)。読み取り/書き込み。</span><span class="sxs-lookup"><span data-stu-id="cfbd0-p118">The name of the item (filename and extension). Read-write.</span></span>
| <span data-ttu-id="cfbd0-189">package</span><span class="sxs-lookup"><span data-stu-id="cfbd0-189">package</span></span>              | <span data-ttu-id="cfbd0-190">[package][]</span><span class="sxs-lookup"><span data-stu-id="cfbd0-190">[package][]</span></span>        | <span data-ttu-id="cfbd0-p119">これがある場合、アイテムはフォルダーやファイルではなく、パッケージです。パッケージは、コンテキスト次第で、ファイルとして、あるいはフォルダーとして扱われます。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="cfbd0-p119">If present, indicates that this item is a package instead of a folder or file. Packages are treated like files in some contexts and folders in others. Read-only.</span></span>
| <span data-ttu-id="cfbd0-194">parentReference</span><span class="sxs-lookup"><span data-stu-id="cfbd0-194">parentReference</span></span>      | <span data-ttu-id="cfbd0-195">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="cfbd0-195">[itemReference][]</span></span>  | <span data-ttu-id="cfbd0-p120">親の情報 (アイテムに親がある場合)。読み取り/書き込み。</span><span class="sxs-lookup"><span data-stu-id="cfbd0-p120">Parent information, if the item has a parent. Read-write.</span></span>
| <span data-ttu-id="cfbd0-198">写真</span><span class="sxs-lookup"><span data-stu-id="cfbd0-198">photo</span></span>                | <span data-ttu-id="cfbd0-199">[photo][]</span><span class="sxs-lookup"><span data-stu-id="cfbd0-199">[photo][]</span></span>          | <span data-ttu-id="cfbd0-p121">写真のメタデータ (アイテムが写真である場合)。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="cfbd0-p121">Photo metadata, if the item is a photo. Read-only.</span></span>
| <span data-ttu-id="cfbd0-202">publication</span><span class="sxs-lookup"><span data-stu-id="cfbd0-202">publication</span></span>          | <span data-ttu-id="cfbd0-203">[publicationFacet][]</span><span class="sxs-lookup"><span data-stu-id="cfbd0-203">[publicationFacet][]</span></span> | <span data-ttu-id="cfbd0-204">アイテムが公開されているか、チェックアウトの状態かどうかの情報を、そのような操作をサポートする場所で提供します。</span><span class="sxs-lookup"><span data-stu-id="cfbd0-204">Provides information about the published or checked-out state of an item, in locations that support such actions.</span></span> <span data-ttu-id="cfbd0-205">既定では、このプロパティは返されません。</span><span class="sxs-lookup"><span data-stu-id="cfbd0-205">This property is not returned by default.</span></span> <span data-ttu-id="cfbd0-206">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="cfbd0-206">Read-only.</span></span> |
| <span data-ttu-id="cfbd0-207">remoteItem</span><span class="sxs-lookup"><span data-stu-id="cfbd0-207">remoteItem</span></span>           | <span data-ttu-id="cfbd0-208">[remoteItem][]</span><span class="sxs-lookup"><span data-stu-id="cfbd0-208">[remoteItem][]</span></span>     | <span data-ttu-id="cfbd0-p123">リモート アイテムのデータ (現在アクセス中のドライブ以外のドライブから共有されているアイテムの場合)。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="cfbd0-p123">Remote item data, if the item is shared from a drive other than the one being accessed. Read-only.</span></span>
| <span data-ttu-id="cfbd0-211">root</span><span class="sxs-lookup"><span data-stu-id="cfbd0-211">root</span></span>                 | <span data-ttu-id="cfbd0-212">[root][]</span><span class="sxs-lookup"><span data-stu-id="cfbd0-212">[root][]</span></span>           | <span data-ttu-id="cfbd0-213">このプロパティが null ではない場合は、driveItem がドライブで最上位の driveItem であることを示します。</span><span class="sxs-lookup"><span data-stu-id="cfbd0-213">If this property is non-null, it indicates that the driveItem is the top-most driveItem in the drive.</span></span>
| <span data-ttu-id="cfbd0-214">searchResult</span><span class="sxs-lookup"><span data-stu-id="cfbd0-214">searchResult</span></span>         | <span data-ttu-id="cfbd0-215">[searchResult][]</span><span class="sxs-lookup"><span data-stu-id="cfbd0-215">[searchResult][]</span></span>   | <span data-ttu-id="cfbd0-p124">検索のメタデータ (検索結果に由来するアイテムの場合)。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="cfbd0-p124">Search metadata, if the item is from a search result. Read-only.</span></span>
| <span data-ttu-id="cfbd0-218">共有</span><span class="sxs-lookup"><span data-stu-id="cfbd0-218">shared</span></span>               | <span data-ttu-id="cfbd0-219">[shared][]</span><span class="sxs-lookup"><span data-stu-id="cfbd0-219">[shared][]</span></span>         | <span data-ttu-id="cfbd0-p125">アイテムが他のユーザーと共有されていることを示し、アイテムの共有状態に関する情報を提供します。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="cfbd0-p125">Indicates that the item has been shared with others and provides information about the shared state of the item. Read-only.</span></span>
| <span data-ttu-id="cfbd0-222">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="cfbd0-222">sharepointIds</span></span>        | <span data-ttu-id="cfbd0-223">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="cfbd0-223">[sharepointIds][]</span></span>  | <span data-ttu-id="cfbd0-p126">SharePoint REST 互換性に役立つ識別子を返します。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="cfbd0-p126">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>
| <span data-ttu-id="cfbd0-226">size</span><span class="sxs-lookup"><span data-stu-id="cfbd0-226">size</span></span>                 | <span data-ttu-id="cfbd0-227">Int64</span><span class="sxs-lookup"><span data-stu-id="cfbd0-227">Int64</span></span>              | <span data-ttu-id="cfbd0-p127">アイテムのサイズ (バイト単位)。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="cfbd0-p127">Size of the item in bytes. Read-only.</span></span>
| <span data-ttu-id="cfbd0-230">specialFolder</span><span class="sxs-lookup"><span data-stu-id="cfbd0-230">specialFolder</span></span>        | <span data-ttu-id="cfbd0-231">[specialFolder][]</span><span class="sxs-lookup"><span data-stu-id="cfbd0-231">[specialFolder][]</span></span>  | <span data-ttu-id="cfbd0-p128">現在のアイテムが特別なフォルダーとしても使用可能な場合は、このファセットが返されます。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="cfbd0-p128">If the current item is also available as a special folder, this facet is returned. Read-only.</span></span>
| <span data-ttu-id="cfbd0-234">video</span><span class="sxs-lookup"><span data-stu-id="cfbd0-234">video</span></span>                | <span data-ttu-id="cfbd0-235">[video][]</span><span class="sxs-lookup"><span data-stu-id="cfbd0-235">[video][]</span></span>          | <span data-ttu-id="cfbd0-p129">ビデオのメタデータ (アイテムがビデオである場合)。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="cfbd0-p129">Video metadata, if the item is a video. Read-only.</span></span>
| <span data-ttu-id="cfbd0-238">webDavUrl</span><span class="sxs-lookup"><span data-stu-id="cfbd0-238">webDavUrl</span></span>            | <span data-ttu-id="cfbd0-239">String</span><span class="sxs-lookup"><span data-stu-id="cfbd0-239">String</span></span>             | <span data-ttu-id="cfbd0-240">アイテムの WebDAV 互換性のある URL。</span><span class="sxs-lookup"><span data-stu-id="cfbd0-240">WebDAV compatible URL for the item.</span></span>
| <span data-ttu-id="cfbd0-241">webUrl</span><span class="sxs-lookup"><span data-stu-id="cfbd0-241">webUrl</span></span>               | <span data-ttu-id="cfbd0-242">文字列</span><span class="sxs-lookup"><span data-stu-id="cfbd0-242">String</span></span>             | <span data-ttu-id="cfbd0-p130">ブラウザーでリソースを表示するための URL。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="cfbd0-p130">URL that displays the resource in the browser. Read-only.</span></span>

<span data-ttu-id="cfbd0-p131">**注:** eTag プロパティと cTag プロパティは、コンテナー (フォルダー) 上での機能が異なります。cTag 値は、フォルダーのいずれかの子孫のコンテンツまたはメタデータが変更されると変更されます。eTag 値は、子孫から派生したプロパティ (**childCount** や **lastModifiedDateTime** など) 以外のフォルダーのプロパティが変更されたときにのみ、変更されます。</span><span class="sxs-lookup"><span data-stu-id="cfbd0-p131">**Note:** The eTag and cTag properties work differently on containers (folders). The cTag value is modified when content or metadata of any descendant of the folder is changed. The eTag value is only modified when the folder's properties are changed, except for properties that are derived from descendants (like **childCount** or **lastModifiedDateTime**).</span></span>

## <a name="relationships"></a><span data-ttu-id="cfbd0-248">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="cfbd0-248">Relationships</span></span>

| <span data-ttu-id="cfbd0-249">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="cfbd0-249">Relationship</span></span>       | <span data-ttu-id="cfbd0-250">種類</span><span class="sxs-lookup"><span data-stu-id="cfbd0-250">Type</span></span>                            | <span data-ttu-id="cfbd0-251">説明</span><span class="sxs-lookup"><span data-stu-id="cfbd0-251">Description</span></span>
|:-------------------|:--------------------------------|:--------------------------
| <span data-ttu-id="cfbd0-252">アクティビティ</span><span class="sxs-lookup"><span data-stu-id="cfbd0-252">activities</span></span>         | <span data-ttu-id="cfbd0-253">[itemActivity][] コレクション</span><span class="sxs-lookup"><span data-stu-id="cfbd0-253">[itemActivity][] collection</span></span>     | <span data-ttu-id="cfbd0-254">このアイテムに対して行われた最近のアクティビティのリストです。</span><span class="sxs-lookup"><span data-stu-id="cfbd0-254">The list of recent activities that took place on this item.</span></span>
| <span data-ttu-id="cfbd0-255">分析</span><span class="sxs-lookup"><span data-stu-id="cfbd0-255">analytics</span></span>          | <span data-ttu-id="cfbd0-256">[itemanalytics][]リソース</span><span class="sxs-lookup"><span data-stu-id="cfbd0-256">[itemAnalytics][] resource</span></span>      | <span data-ttu-id="cfbd0-257">このアイテムに対して行われたビューアクティビティに関する分析。</span><span class="sxs-lookup"><span data-stu-id="cfbd0-257">Analytics about the view activities that took place on this item.</span></span>
| <span data-ttu-id="cfbd0-258">content</span><span class="sxs-lookup"><span data-stu-id="cfbd0-258">content</span></span>            | <span data-ttu-id="cfbd0-259">Stream</span><span class="sxs-lookup"><span data-stu-id="cfbd0-259">Stream</span></span>                          | <span data-ttu-id="cfbd0-260">コンテンツのストリーム (アイテムがファイルを表す場合)。</span><span class="sxs-lookup"><span data-stu-id="cfbd0-260">The content stream, if the item represents a file.</span></span>
| <span data-ttu-id="cfbd0-261">children</span><span class="sxs-lookup"><span data-stu-id="cfbd0-261">children</span></span>           | <span data-ttu-id="cfbd0-262">driveitem コレクション</span><span class="sxs-lookup"><span data-stu-id="cfbd0-262">driveitem collection</span></span>            | <span data-ttu-id="cfbd0-p132">アイテムの直接の子のアイテム オブジェクトを格納するコレクション。子が含まれるのは、フォルダーを表すアイテムのみです。読み取り専用です。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="cfbd0-p132">Collection containing Item objects for the immediate children of Item. Only items representing folders have children. Read-only. Nullable.</span></span>
| <span data-ttu-id="cfbd0-267">listItem</span><span class="sxs-lookup"><span data-stu-id="cfbd0-267">listItem</span></span>           | <span data-ttu-id="cfbd0-268">[listItem][]</span><span class="sxs-lookup"><span data-stu-id="cfbd0-268">[listItem][]</span></span>                    | <span data-ttu-id="cfbd0-269">SharePoint のドライブの場合は、関連付けられているドキュメントライブラリのリストアイテム。</span><span class="sxs-lookup"><span data-stu-id="cfbd0-269">For drives in SharePoint, the associated document library list item.</span></span> <span data-ttu-id="cfbd0-270">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="cfbd0-270">Read-only.</span></span> <span data-ttu-id="cfbd0-271">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="cfbd0-271">Nullable.</span></span>
| <span data-ttu-id="cfbd0-272">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="cfbd0-272">permissions</span></span>        | <span data-ttu-id="cfbd0-273">[permission][] コレクション</span><span class="sxs-lookup"><span data-stu-id="cfbd0-273">[permission][] collection</span></span>       | <span data-ttu-id="cfbd0-p134">アイテムのアクセス許可のセット。読み取り専用です。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="cfbd0-p134">The set of permissions for the item. Read-only. Nullable.</span></span>
| <span data-ttu-id="cfbd0-277">thumbnails</span><span class="sxs-lookup"><span data-stu-id="cfbd0-277">thumbnails</span></span>         | <span data-ttu-id="cfbd0-278">[thumbnailSet][] コレクション</span><span class="sxs-lookup"><span data-stu-id="cfbd0-278">[thumbnailSet][] collection</span></span>     | <span data-ttu-id="cfbd0-p135">アイテムに関連付けられた [ThumbnailSet][] オブジェクトを格納するコレクション。詳細については、[サムネイルの取得][]についてのページを参照してください。読み取り専用です。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="cfbd0-p135">Collection containing [ThumbnailSet][] objects associated with the item. For more info, see [getting thumbnails][]. Read-only. Nullable.</span></span>
| <span data-ttu-id="cfbd0-283">最新</span><span class="sxs-lookup"><span data-stu-id="cfbd0-283">versions</span></span>           | <span data-ttu-id="cfbd0-284">[drive itemversion][]コレクション</span><span class="sxs-lookup"><span data-stu-id="cfbd0-284">[driveItemVersion][] collection</span></span> | <span data-ttu-id="cfbd0-285">アイテムの以前のバージョンのリスト。</span><span class="sxs-lookup"><span data-stu-id="cfbd0-285">The list of previous versions of the item.</span></span> <span data-ttu-id="cfbd0-286">詳細については、「[以前のバージョンを取得][]する」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="cfbd0-286">For more info, see [getting previous versions][].</span></span> <span data-ttu-id="cfbd0-287">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="cfbd0-287">Read-only.</span></span> <span data-ttu-id="cfbd0-288">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="cfbd0-288">Nullable.</span></span>

## <a name="instance-attributes"></a><span data-ttu-id="cfbd0-289">インスタンスの属性</span><span class="sxs-lookup"><span data-stu-id="cfbd0-289">Instance Attributes</span></span>

<span data-ttu-id="cfbd0-p137">インスタンスの属性は、動作が特殊なプロパティです。これらのプロパティは一時的なものであり、a) サービスの動作を定義するか、b) 短期的なプロパティの値 (有効期限を持つアイテムのダウンロード URL など) を提供します。</span><span class="sxs-lookup"><span data-stu-id="cfbd0-p137">Instance attributes are properties with special behaviors. These properties are temporary and either a) define behavior the service should perform or b) provide short-term property values, like a download URL for an item that expires.</span></span>

| <span data-ttu-id="cfbd0-292">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="cfbd0-292">Property name</span></span>                     | <span data-ttu-id="cfbd0-293">種類</span><span class="sxs-lookup"><span data-stu-id="cfbd0-293">Type</span></span>   | <span data-ttu-id="cfbd0-294">説明</span><span class="sxs-lookup"><span data-stu-id="cfbd0-294">Description</span></span>
|:----------------------------------|:-------|:--------------------------------
| <span data-ttu-id="cfbd0-295">@microsoft.graph.conflictBehavior</span><span class="sxs-lookup"><span data-stu-id="cfbd0-295">@microsoft.graph.conflictBehavior</span></span> | <span data-ttu-id="cfbd0-296">string</span><span class="sxs-lookup"><span data-stu-id="cfbd0-296">string</span></span> | <span data-ttu-id="cfbd0-p138">新しいアイテムを作成するアクションの競合を解決する動作。*fail*、*replace*、*rename* という値を使用できます。PUT の既定値は *replace* です。この注釈とともにアイテムが返されることはありません。書き込み専用です。</span><span class="sxs-lookup"><span data-stu-id="cfbd0-p138">The conflict resolution behavior for actions that create a new item. You can use the values *fail*, *replace*, or *rename*. The default for PUT is *replace*. An item will never be returned with this annotation. Write-only.</span></span>
| <span data-ttu-id="cfbd0-302">@microsoft.graph.downloadUrl</span><span class="sxs-lookup"><span data-stu-id="cfbd0-302">@microsoft.graph.downloadUrl</span></span>      | <span data-ttu-id="cfbd0-303">string</span><span class="sxs-lookup"><span data-stu-id="cfbd0-303">string</span></span> | <span data-ttu-id="cfbd0-p139">このファイルのコンテンツをダウンロードするために使用できる URL。この URL では認証は必要ありません。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="cfbd0-p139">A URL that can be used to download this file's content. Authentication is not required with this URL. Read-only.</span></span>
| <span data-ttu-id="cfbd0-307">@microsoft.graph.sourceUrl</span><span class="sxs-lookup"><span data-stu-id="cfbd0-307">@microsoft.graph.sourceUrl</span></span>        | <span data-ttu-id="cfbd0-308">string</span><span class="sxs-lookup"><span data-stu-id="cfbd0-308">string</span></span> | <span data-ttu-id="cfbd0-p140">PUT 要求を発行するときにこのインスタンスの注釈を使用すると、サービスに対し、URL のコンテンツをダウンロードし、それをファイルとして保存するように指示できます。書き込み専用です。</span><span class="sxs-lookup"><span data-stu-id="cfbd0-p140">When issuing a PUT request, this instance annotation can be used to instruct the service to download the contents of the URL, and store it as the file. Write-only.</span></span>

<span data-ttu-id="cfbd0-311">**注:**@microsoft.graph.downloadUrl の値は短時間限定の URL であるため、キャッシュすることはできません。</span><span class="sxs-lookup"><span data-stu-id="cfbd0-311">**Note:** The @microsoft.graph.downloadUrl value is a short-lived URL and can't be cached.</span></span>
<span data-ttu-id="cfbd0-312">URL は短い期間 (1 時間) だけ使用でき、その後は無効になります。</span><span class="sxs-lookup"><span data-stu-id="cfbd0-312">The URL will only be available for a short period of time (1 hour) before it is invalidated.</span></span> <span data-ttu-id="cfbd0-313">ユーザーのファイルアクセス許可を削除しても、その URL はすぐに無効になることはありません。</span><span class="sxs-lookup"><span data-stu-id="cfbd0-313">Removing file permissions for a user may not immediately invalidate the URL.</span></span>

## <a name="methods"></a><span data-ttu-id="cfbd0-314">メソッド</span><span class="sxs-lookup"><span data-stu-id="cfbd0-314">Methods</span></span>

| <span data-ttu-id="cfbd0-315">メソッド</span><span class="sxs-lookup"><span data-stu-id="cfbd0-315">Method</span></span>                                                   | <span data-ttu-id="cfbd0-316">REST パス</span><span class="sxs-lookup"><span data-stu-id="cfbd0-316">REST Path</span></span>
|:---------------------------------------------------------|:------------------
| [<span data-ttu-id="cfbd0-317">アイテムを取得する</span><span class="sxs-lookup"><span data-stu-id="cfbd0-317">Get item</span></span>](../api/driveitem-get.md)                      | `GET /drive/items/{item-id}`
| [<span data-ttu-id="cfbd0-318">アクティビティを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="cfbd0-318">List activities</span></span>](../api/activities-list.md)             | `GET /drive/items/{item-id}/activities`
| <span data-ttu-id="cfbd0-319">[分析を取得する][]</span><span class="sxs-lookup"><span data-stu-id="cfbd0-319">[Get analytics][]</span></span>                                        | `GET /drive/items/{item-id}/analytics`
| <span data-ttu-id="cfbd0-320">[間隔でアクティビティを取得する][]</span><span class="sxs-lookup"><span data-stu-id="cfbd0-320">[Get activities by interval][]</span></span>                           | `GET /drive/items/{item-id}/getActivitiesByInterval`
| [<span data-ttu-id="cfbd0-321">子を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="cfbd0-321">List children</span></span>](../api/driveitem-list-children.md)       | `GET /drive/items/{item-id}/children`
| [<span data-ttu-id="cfbd0-322">バージョンを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="cfbd0-322">List versions</span></span>](../api/driveitem-list-versions.md)       | `GET /drive/items/{item-id}/versions`
| [<span data-ttu-id="cfbd0-323">アイテムを作成する</span><span class="sxs-lookup"><span data-stu-id="cfbd0-323">Create item</span></span>](../api/driveitem-post-children.md)         | `POST /drive/items/{item-id}/children`
| [<span data-ttu-id="cfbd0-324">アイテムを更新する</span><span class="sxs-lookup"><span data-stu-id="cfbd0-324">Update item</span></span>](../api/driveitem-update.md)                | `PATCH /drive/items/{item-id}`
| [<span data-ttu-id="cfbd0-325">コンテンツをアップロードする</span><span class="sxs-lookup"><span data-stu-id="cfbd0-325">Upload content</span></span>](../api/driveitem-put-content.md)        | `PUT /drive/items/{item-id}/content`
| [<span data-ttu-id="cfbd0-326">コンテンツをダウンロードする</span><span class="sxs-lookup"><span data-stu-id="cfbd0-326">Download content</span></span>](../api/driveitem-get-content.md)      | `GET /drive/items/{item-id}/content`
| <span data-ttu-id="cfbd0-327">[特定のファイル形式をダウンロードする][download-format]</span><span class="sxs-lookup"><span data-stu-id="cfbd0-327">[Download specific file format][download-format]</span></span>         | `GET /drive/items/{item-id}/content?format={format}`
| [<span data-ttu-id="cfbd0-328">アイテムを削除する</span><span class="sxs-lookup"><span data-stu-id="cfbd0-328">Delete item</span></span>](../api/driveitem-delete.md)                | `DELETE /drive/items/{item-id}`
| [<span data-ttu-id="cfbd0-329">アイテムを移動する</span><span class="sxs-lookup"><span data-stu-id="cfbd0-329">Move item</span></span>](../api/driveitem-move.md)                    | `PATCH /drive/items/{item-id}`
| [<span data-ttu-id="cfbd0-330">アイテムをコピーする</span><span class="sxs-lookup"><span data-stu-id="cfbd0-330">Copy item</span></span>](../api/driveitem-copy.md)                    | `POST /drive/items/{item-id}/copy`
| [<span data-ttu-id="cfbd0-331">アイテムを検索する</span><span class="sxs-lookup"><span data-stu-id="cfbd0-331">Search items</span></span>](../api/driveitem-search.md)               | `GET /drive/items/{item-id}/search(q='text')`
| [<span data-ttu-id="cfbd0-332">ドライブ内の変更内容を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="cfbd0-332">List changes in a drive</span></span>](../api/driveitem-delta.md)     | `GET /drive/root/delta`
| [<span data-ttu-id="cfbd0-333">サムネイルを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="cfbd0-333">List thumbnails</span></span>](../api/driveitem-list-thumbnails.md)   | `GET /drive/items/{item-id}/thumbnails`
| [<span data-ttu-id="cfbd0-334">共有リンクを作成する</span><span class="sxs-lookup"><span data-stu-id="cfbd0-334">Create sharing link</span></span>](../api/driveitem-createlink.md)    | `POST /drive/items/{item-id}/createLink`
| [<span data-ttu-id="cfbd0-335">アクセス許可を追加する</span><span class="sxs-lookup"><span data-stu-id="cfbd0-335">Add permissions</span></span>](../api/driveitem-invite.md)            | `POST /drive/items/{item-id}/invite`
| [<span data-ttu-id="cfbd0-336">アクセス許可を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="cfbd0-336">List permissions</span></span>](../api/driveitem-list-permissions.md) | `GET /drive/items/{item-id}/permissions`
| [<span data-ttu-id="cfbd0-337">アクセス許可を削除する</span><span class="sxs-lookup"><span data-stu-id="cfbd0-337">Delete permission</span></span>](../api/permission-delete.md)         | `DELETE /drive/items/{item-id}/permissions/{perm-id}`
| <span data-ttu-id="cfbd0-338">[WebSocket チャネルの取得][getWebSocket]</span><span class="sxs-lookup"><span data-stu-id="cfbd0-338">[Get WebSocket channel][getWebSocket]</span></span>                    | `GET /drive/root/subscriptions/socketIo`
| <span data-ttu-id="cfbd0-339">[アイテムのプレビュー][item-preview]</span><span class="sxs-lookup"><span data-stu-id="cfbd0-339">[Preview item][item-preview]</span></span>                             | `POST /drive/items/{item-id}/preview`

[item-preview]: ../api/driveitem-preview.md
[分析を取得する]: ../api/itemanalytics-get.md
[Get analytics]: ../api/itemanalytics-get.md
[間隔でアクティビティを取得する]: ../api/itemactivity-getbyinterval.md
[Get activities by interval]: ../api/itemactivity-getbyinterval.md

## <a name="remarks"></a><span data-ttu-id="cfbd0-342">備考</span><span class="sxs-lookup"><span data-stu-id="cfbd0-342">Remarks</span></span>

<span data-ttu-id="cfbd0-343">OneDrive for Business または SharePoint のドキュメント ライブラリでは、**driveItem** に[フォルダー][] ファセットがある場合、**cTag** プロパティは返されません。</span><span class="sxs-lookup"><span data-stu-id="cfbd0-343">In OneDrive for Business or SharePoint document libraries, the **cTag** property is not returned, if the **driveItem** has a [folder][] facet.</span></span>

[audio]: audio.md
[baseItem]: baseitem.md
[deleted]: deleted.md
[download-format]: ../api/driveitem-get-content-format.md
[driveItemVersion]: driveitemversion.md
[file]: file.md
[fileSystemInfo]: filesysteminfo.md
[folder]: folder.md
[以前のバージョンの取得]: ../api/driveitem-list-versions.md
[getting previous versions]: ../api/driveitem-list-versions.md
[サムネイルの取得]: ../api/driveitem-list-thumbnails.md
[getting thumbnails]: ../api/driveitem-list-thumbnails.md
[getWebSocket]: ../api/driveitem-subscriptions-socketio.md
[identitySet]: identityset.md
[image]: image.md
[itemActivity]: itemactivity.md
[itemanalytics]: itemanalytics.md
[itemAnalytics]: itemanalytics.md
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
