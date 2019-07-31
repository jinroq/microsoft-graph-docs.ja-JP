---
author: JeremyKelley
description: driveItem リソースは、ドライブに格納されているファイル、フォルダーなどのアイテムを表します。
ms.date: 09/10/2017
title: DriveItem
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 93c73fa61c871afce4ce4c7ed00e3c1ef554ca79
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972972"
---
# <a name="driveitem-resource-type"></a><span data-ttu-id="ddeb0-103">driveItem リソース型</span><span class="sxs-lookup"><span data-stu-id="ddeb0-103">driveItem resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ddeb0-p101">**driveItem** リソースは、ドライブに格納されているファイル、フォルダーなどのアイテムを表します。OneDrive および SharePoint 内のすべてのファイル システム オブジェクトが、**driveItem** リソースとして返されます。</span><span class="sxs-lookup"><span data-stu-id="ddeb0-p101">The **driveItem** resource represents a file, folder, or other item stored in a drive. All file system objects in OneDrive and SharePoint are returned as **driveItem** resources.</span></span>

<span data-ttu-id="ddeb0-106">**driveItem** リソースのアドレス指定には、主に 2 つの方法があります。</span><span class="sxs-lookup"><span data-stu-id="ddeb0-106">There are two primary ways of addressing a **driveItem** resource:</span></span>

* <span data-ttu-id="ddeb0-107">`drive/items/{item-id}` を使用した、**driveItem** 一意識別子による方法</span><span class="sxs-lookup"><span data-stu-id="ddeb0-107">By the **driveItem** unique identifier using `drive/items/{item-id}`</span></span>
* <span data-ttu-id="ddeb0-108">`/drive/root:/path/to/file` を使用した、ファイル システム パスによる方法</span><span class="sxs-lookup"><span data-stu-id="ddeb0-108">By file system path using `/drive/root:/path/to/file`</span></span>

<span data-ttu-id="ddeb0-p102">**DriveItem** リソースには、driveItem の ID および機能に関するデータを提供するプロパティとしてモデル化されたファセットがあります。例:</span><span class="sxs-lookup"><span data-stu-id="ddeb0-p102">**DriveItem** resources have facets modeled as properties that provide data about the driveItem's identities and capabilities. For example:</span></span>

* <span data-ttu-id="ddeb0-111">フォルダーには、[\*\*フォルダー ファセット \*\*][folder] があります。</span><span class="sxs-lookup"><span data-stu-id="ddeb0-111">Folders have a [**folder facet**][folder]</span></span>
* <span data-ttu-id="ddeb0-112">ファイルには、[\*\*ファイル ファセット \*\*][file] があります。</span><span class="sxs-lookup"><span data-stu-id="ddeb0-112">Files have a [**file facet**][file].</span></span>
* <span data-ttu-id="ddeb0-113">画像には[\*\*画像ファセット \*\*][image] とそのファイル ファセットがあります。</span><span class="sxs-lookup"><span data-stu-id="ddeb0-113">Images have an [**image facet**][image] in addition to their file facet.</span></span>
* <span data-ttu-id="ddeb0-114">カメラで撮影した画像 (写真) には[\*\*写真ファセット \*\*][photo] があります。写真ファセットは、アイテムを写真として識別し、撮影日時と撮影デバイスのプロパティを提供します。</span><span class="sxs-lookup"><span data-stu-id="ddeb0-114">Images taken with a camera (photos) have a [**photo facet**][photo] that identifies the item as a photo and provides the properties of when the photo was taken and with what device.</span></span>

<span data-ttu-id="ddeb0-115">**フォルダー** ファセットを持つアイテムは、アイテムのコンテナーとして機能するため、フォルダーに含まれる **driveItems** のコレクションを指す `children` 参照を持ちます。</span><span class="sxs-lookup"><span data-stu-id="ddeb0-115">Items with the **folder** facet act as containers of items and therefore have a `children` reference pointing to a collection of **driveItems** under the folder.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ddeb0-116">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ddeb0-116">JSON representation</span></span>

<span data-ttu-id="ddeb0-117">以下は、**driveItem** リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="ddeb0-117">Here is a JSON representation of a **driveItem** resource.</span></span>

<span data-ttu-id="ddeb0-118">**driveItem** リソースは [**baseItem**][baseItem] から派生し、そのリソースからプロパティを継承します。</span><span class="sxs-lookup"><span data-stu-id="ddeb0-118">The **driveItem** resource is derived from [**baseItem**][baseItem] and inherits properties from that resource.</span></span>

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
  "activities": [{"@odata.type": "microsoft.graph.itemActivity"}],
  "children": [{ "@odata.type": "microsoft.graph.driveItem" }],
  "createdByUser": { "@odata.type": "microsoft.graph.user" },
  "lastModifiedByUser": { "@odata.type": "microsoft.graph.user" },
  "permissions": [ {"@odata.type": "microsoft.graph.permission"} ],
  "subscriptions": [ {"@odata.type": "microsoft.graph.subscription"} ],
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

## <a name="properties"></a><span data-ttu-id="ddeb0-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ddeb0-119">Properties</span></span>

| <span data-ttu-id="ddeb0-120">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ddeb0-120">Property</span></span>             | <span data-ttu-id="ddeb0-121">型</span><span class="sxs-lookup"><span data-stu-id="ddeb0-121">Type</span></span>               | <span data-ttu-id="ddeb0-122">説明</span><span class="sxs-lookup"><span data-stu-id="ddeb0-122">Description</span></span>
|:---------------------|:-------------------|:---------------------------------
| <span data-ttu-id="ddeb0-123">audio</span><span class="sxs-lookup"><span data-stu-id="ddeb0-123">audio</span></span>                | <span data-ttu-id="ddeb0-124">[audio][]</span><span class="sxs-lookup"><span data-stu-id="ddeb0-124">[audio][]</span></span>          | <span data-ttu-id="ddeb0-p103">オーディオのメタデータ (アイテムがオーディオ ファイルである場合)。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="ddeb0-p103">Audio metadata, if the item is an audio file. Read-only.</span></span>
| <span data-ttu-id="ddeb0-127">content</span><span class="sxs-lookup"><span data-stu-id="ddeb0-127">content</span></span>              | <span data-ttu-id="ddeb0-128">Stream</span><span class="sxs-lookup"><span data-stu-id="ddeb0-128">Stream</span></span>             | <span data-ttu-id="ddeb0-129">コンテンツのストリーム (アイテムがファイルを表す場合)。</span><span class="sxs-lookup"><span data-stu-id="ddeb0-129">The content stream, if the item represents a file.</span></span>
| <span data-ttu-id="ddeb0-130">createdBy</span><span class="sxs-lookup"><span data-stu-id="ddeb0-130">createdBy</span></span>            | <span data-ttu-id="ddeb0-131">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="ddeb0-131">[identitySet][]</span></span>    | <span data-ttu-id="ddeb0-p104">そのアイテムを作成したユーザーの ID、デバイス、アプリケーション。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="ddeb0-p104">Identity of the user, device, and application which created the item. Read-only.</span></span>
| <span data-ttu-id="ddeb0-134">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ddeb0-134">createdDateTime</span></span>      | <span data-ttu-id="ddeb0-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ddeb0-135">DateTimeOffset</span></span>     | <span data-ttu-id="ddeb0-p105">アイテム作成の日時。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="ddeb0-p105">Date and time of item creation. Read-only.</span></span>
| <span data-ttu-id="ddeb0-138">cTag</span><span class="sxs-lookup"><span data-stu-id="ddeb0-138">cTag</span></span>                 | <span data-ttu-id="ddeb0-139">String</span><span class="sxs-lookup"><span data-stu-id="ddeb0-139">String</span></span>             | <span data-ttu-id="ddeb0-p106">アイテムのコンテンツの eTag。メタデータのみが変更された場合、この eTag は変更されません。**注:** アイテムがフォルダーである場合、このプロパティは返されません。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="ddeb0-p106">An eTag for the content of the item. This eTag is not changed if only the metadata is changed. **Note** This property is not returned if the item is a folder. Read-only.</span></span>
| <span data-ttu-id="ddeb0-144">deleted</span><span class="sxs-lookup"><span data-stu-id="ddeb0-144">deleted</span></span>              | <span data-ttu-id="ddeb0-145">[deleted][]</span><span class="sxs-lookup"><span data-stu-id="ddeb0-145">[deleted][]</span></span>        | <span data-ttu-id="ddeb0-p107">アイテムの削除状態に関する情報。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="ddeb0-p107">Information about the deleted state of the item. Read-only.</span></span>
| <span data-ttu-id="ddeb0-148">description</span><span class="sxs-lookup"><span data-stu-id="ddeb0-148">description</span></span>          | <span data-ttu-id="ddeb0-149">String</span><span class="sxs-lookup"><span data-stu-id="ddeb0-149">String</span></span>             | <span data-ttu-id="ddeb0-p108">ユーザーに表示されるアイテムの説明を提供します。読み取り/書き込み。OneDrive 個人用においてのみ</span><span class="sxs-lookup"><span data-stu-id="ddeb0-p108">Provides a user-visible description of the item. Read-write. Only on OneDrive Personal</span></span>
| <span data-ttu-id="ddeb0-153">eTag</span><span class="sxs-lookup"><span data-stu-id="ddeb0-153">eTag</span></span>                 | <span data-ttu-id="ddeb0-154">String</span><span class="sxs-lookup"><span data-stu-id="ddeb0-154">String</span></span>             | <span data-ttu-id="ddeb0-p109">アイテム全体 (メタデータおよびコンテンツ) の eTag。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="ddeb0-p109">eTag for the entire item (metadata + content). Read-only.</span></span>
| <span data-ttu-id="ddeb0-157">file</span><span class="sxs-lookup"><span data-stu-id="ddeb0-157">file</span></span>                 | <span data-ttu-id="ddeb0-158">[file][]</span><span class="sxs-lookup"><span data-stu-id="ddeb0-158">[file][]</span></span>           | <span data-ttu-id="ddeb0-p110">ファイルのメタデータ (アイテムがファイルである場合)。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="ddeb0-p110">File metadata, if the item is a file. Read-only.</span></span>
| <span data-ttu-id="ddeb0-161">fileSystemInfo</span><span class="sxs-lookup"><span data-stu-id="ddeb0-161">fileSystemInfo</span></span>       | <span data-ttu-id="ddeb0-162">[fileSystemInfo][]</span><span class="sxs-lookup"><span data-stu-id="ddeb0-162">[fileSystemInfo][]</span></span> | <span data-ttu-id="ddeb0-p111">クライアント上のファイル システム情報。読み取り/書き込み。</span><span class="sxs-lookup"><span data-stu-id="ddeb0-p111">File system information on client. Read-write.</span></span>
| <span data-ttu-id="ddeb0-165">folder</span><span class="sxs-lookup"><span data-stu-id="ddeb0-165">folder</span></span>               | <span data-ttu-id="ddeb0-166">[フォルダー][]</span><span class="sxs-lookup"><span data-stu-id="ddeb0-166">[folder][]</span></span>         | <span data-ttu-id="ddeb0-p112">フォルダーのメタデータ (アイテムがフォルダーである場合)。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="ddeb0-p112">Folder metadata, if the item is a folder. Read-only.</span></span>
| <span data-ttu-id="ddeb0-169">id</span><span class="sxs-lookup"><span data-stu-id="ddeb0-169">id</span></span>                   | <span data-ttu-id="ddeb0-170">文字列</span><span class="sxs-lookup"><span data-stu-id="ddeb0-170">String</span></span>             | <span data-ttu-id="ddeb0-p113">ドライブ内のアイテムの一意識別子。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="ddeb0-p113">The unique identifier of the item within the Drive. Read-only.</span></span>
| <span data-ttu-id="ddeb0-173">image</span><span class="sxs-lookup"><span data-stu-id="ddeb0-173">image</span></span>                | <span data-ttu-id="ddeb0-174">[image][]</span><span class="sxs-lookup"><span data-stu-id="ddeb0-174">[image][]</span></span>          | <span data-ttu-id="ddeb0-p114">画像のメタデータ (アイテムが画像である場合)。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="ddeb0-p114">Image metadata, if the item is an image. Read-only.</span></span>
| <span data-ttu-id="ddeb0-177">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="ddeb0-177">lastModifiedBy</span></span>       | <span data-ttu-id="ddeb0-178">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="ddeb0-178">[identitySet][]</span></span>    | <span data-ttu-id="ddeb0-p115">アイテムを最終更新したユーザーの ID、デバイス、アプリケーション。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="ddeb0-p115">Identity of the user, device, and application which last modified the item. Read-only.</span></span>
| <span data-ttu-id="ddeb0-181">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ddeb0-181">lastModifiedDateTime</span></span> | <span data-ttu-id="ddeb0-182">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ddeb0-182">DateTimeOffset</span></span>     | <span data-ttu-id="ddeb0-p116">アイテムが最後に変更された日時。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="ddeb0-p116">Date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="ddeb0-185">location</span><span class="sxs-lookup"><span data-stu-id="ddeb0-185">location</span></span>             | <span data-ttu-id="ddeb0-186">[geoCoordinates][]</span><span class="sxs-lookup"><span data-stu-id="ddeb0-186">[geoCoordinates][]</span></span> | <span data-ttu-id="ddeb0-p117">場所のメタデータ (アイテムに場所データが含まれている場合)。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="ddeb0-p117">Location metadata, if the item has location data. Read-only.</span></span>
| <span data-ttu-id="ddeb0-189">name</span><span class="sxs-lookup"><span data-stu-id="ddeb0-189">name</span></span>                 | <span data-ttu-id="ddeb0-190">文字列</span><span class="sxs-lookup"><span data-stu-id="ddeb0-190">String</span></span>             | <span data-ttu-id="ddeb0-p118">アイテムの名前 (ファイル名と拡張子)。読み取り/書き込み。</span><span class="sxs-lookup"><span data-stu-id="ddeb0-p118">The name of the item (filename and extension). Read-write.</span></span>
| <span data-ttu-id="ddeb0-193">package</span><span class="sxs-lookup"><span data-stu-id="ddeb0-193">package</span></span>              | <span data-ttu-id="ddeb0-194">[package][]</span><span class="sxs-lookup"><span data-stu-id="ddeb0-194">[package][]</span></span>        | <span data-ttu-id="ddeb0-p119">これがある場合、アイテムはフォルダーやファイルではなく、パッケージです。パッケージは、コンテキスト次第で、ファイルとして、あるいはフォルダーとして扱われます。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="ddeb0-p119">If present, indicates that this item is a package instead of a folder or file. Packages are treated like files in some contexts and folders in others. Read-only.</span></span>
| <span data-ttu-id="ddeb0-198">parentReference</span><span class="sxs-lookup"><span data-stu-id="ddeb0-198">parentReference</span></span>      | <span data-ttu-id="ddeb0-199">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="ddeb0-199">[itemReference][]</span></span>  | <span data-ttu-id="ddeb0-p120">親の情報 (アイテムに親がある場合)。読み取り/書き込み。</span><span class="sxs-lookup"><span data-stu-id="ddeb0-p120">Parent information, if the item has a parent. Read-write.</span></span>
| <span data-ttu-id="ddeb0-202">写真</span><span class="sxs-lookup"><span data-stu-id="ddeb0-202">photo</span></span>                | <span data-ttu-id="ddeb0-203">[photo][]</span><span class="sxs-lookup"><span data-stu-id="ddeb0-203">[photo][]</span></span>          | <span data-ttu-id="ddeb0-p121">写真のメタデータ (アイテムが写真である場合)。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="ddeb0-p121">Photo metadata, if the item is a photo. Read-only.</span></span>
| <span data-ttu-id="ddeb0-206">publication</span><span class="sxs-lookup"><span data-stu-id="ddeb0-206">publication</span></span>          | <span data-ttu-id="ddeb0-207">[publicationFacet][]</span><span class="sxs-lookup"><span data-stu-id="ddeb0-207">[publicationFacet][]</span></span> | <span data-ttu-id="ddeb0-208">アイテムが公開されているか、チェックアウトの状態かどうかの情報を、そのような操作をサポートする場所で提供します。</span><span class="sxs-lookup"><span data-stu-id="ddeb0-208">Provides information about the published or checked-out state of an item, in locations that support such actions.</span></span> <span data-ttu-id="ddeb0-209">既定では、このプロパティは返されません。</span><span class="sxs-lookup"><span data-stu-id="ddeb0-209">This property is not returned by default.</span></span> <span data-ttu-id="ddeb0-210">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="ddeb0-210">Read-only.</span></span> |
| <span data-ttu-id="ddeb0-211">remoteItem</span><span class="sxs-lookup"><span data-stu-id="ddeb0-211">remoteItem</span></span>           | <span data-ttu-id="ddeb0-212">[remoteItem][]</span><span class="sxs-lookup"><span data-stu-id="ddeb0-212">[remoteItem][]</span></span>     | <span data-ttu-id="ddeb0-p123">リモート アイテムのデータ (現在アクセス中のドライブ以外のドライブから共有されているアイテムの場合)。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="ddeb0-p123">Remote item data, if the item is shared from a drive other than the one being accessed. Read-only.</span></span>
| <span data-ttu-id="ddeb0-215">root</span><span class="sxs-lookup"><span data-stu-id="ddeb0-215">root</span></span>                 | <span data-ttu-id="ddeb0-216">[root][]</span><span class="sxs-lookup"><span data-stu-id="ddeb0-216">[root][]</span></span>           | <span data-ttu-id="ddeb0-217">このプロパティが null ではない場合は、driveItem がドライブで最上位の driveItem であることを示します。</span><span class="sxs-lookup"><span data-stu-id="ddeb0-217">If this property is non-null, it indicates that the driveItem is the top-most driveItem in the drive.</span></span>
| <span data-ttu-id="ddeb0-218">searchResult</span><span class="sxs-lookup"><span data-stu-id="ddeb0-218">searchResult</span></span>         | <span data-ttu-id="ddeb0-219">[searchResult][]</span><span class="sxs-lookup"><span data-stu-id="ddeb0-219">[searchResult][]</span></span>   | <span data-ttu-id="ddeb0-p124">検索のメタデータ (検索結果に由来するアイテムの場合)。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="ddeb0-p124">Search metadata, if the item is from a search result. Read-only.</span></span>
| <span data-ttu-id="ddeb0-222">共有</span><span class="sxs-lookup"><span data-stu-id="ddeb0-222">shared</span></span>               | <span data-ttu-id="ddeb0-223">[shared][]</span><span class="sxs-lookup"><span data-stu-id="ddeb0-223">[shared][]</span></span>         | <span data-ttu-id="ddeb0-p125">アイテムが他のユーザーと共有されていることを示し、アイテムの共有状態に関する情報を提供します。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="ddeb0-p125">Indicates that the item has been shared with others and provides information about the shared state of the item. Read-only.</span></span>
| <span data-ttu-id="ddeb0-226">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="ddeb0-226">sharepointIds</span></span>        | <span data-ttu-id="ddeb0-227">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="ddeb0-227">[sharepointIds][]</span></span>  | <span data-ttu-id="ddeb0-p126">SharePoint REST 互換性に役立つ識別子を返します。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="ddeb0-p126">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>
| <span data-ttu-id="ddeb0-230">size</span><span class="sxs-lookup"><span data-stu-id="ddeb0-230">size</span></span>                 | <span data-ttu-id="ddeb0-231">Int64</span><span class="sxs-lookup"><span data-stu-id="ddeb0-231">Int64</span></span>              | <span data-ttu-id="ddeb0-p127">アイテムのサイズ (バイト単位)。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="ddeb0-p127">Size of the item in bytes. Read-only.</span></span>
| <span data-ttu-id="ddeb0-234">specialFolder</span><span class="sxs-lookup"><span data-stu-id="ddeb0-234">specialFolder</span></span>        | <span data-ttu-id="ddeb0-235">[specialFolder][]</span><span class="sxs-lookup"><span data-stu-id="ddeb0-235">[specialFolder][]</span></span>  | <span data-ttu-id="ddeb0-p128">現在のアイテムが特別なフォルダーとしても使用可能な場合は、このファセットが返されます。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="ddeb0-p128">If the current item is also available as a special folder, this facet is returned. Read-only.</span></span>
| <span data-ttu-id="ddeb0-238">video</span><span class="sxs-lookup"><span data-stu-id="ddeb0-238">video</span></span>                | <span data-ttu-id="ddeb0-239">[video][]</span><span class="sxs-lookup"><span data-stu-id="ddeb0-239">[video][]</span></span>          | <span data-ttu-id="ddeb0-p129">ビデオのメタデータ (アイテムがビデオである場合)。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="ddeb0-p129">Video metadata, if the item is a video. Read-only.</span></span>
| <span data-ttu-id="ddeb0-242">webDavUrl</span><span class="sxs-lookup"><span data-stu-id="ddeb0-242">webDavUrl</span></span>            | <span data-ttu-id="ddeb0-243">String</span><span class="sxs-lookup"><span data-stu-id="ddeb0-243">String</span></span>             | <span data-ttu-id="ddeb0-244">アイテムの WebDAV 互換性のある URL。</span><span class="sxs-lookup"><span data-stu-id="ddeb0-244">WebDAV compatible URL for the item.</span></span>
| <span data-ttu-id="ddeb0-245">webUrl</span><span class="sxs-lookup"><span data-stu-id="ddeb0-245">webUrl</span></span>               | <span data-ttu-id="ddeb0-246">String</span><span class="sxs-lookup"><span data-stu-id="ddeb0-246">String</span></span>             | <span data-ttu-id="ddeb0-p130">ブラウザーでリソースを表示するための URL。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="ddeb0-p130">URL that displays the resource in the browser. Read-only.</span></span>

<span data-ttu-id="ddeb0-p131">**注:** eTag プロパティと cTag プロパティは、コンテナー (フォルダー) 上での機能が異なります。cTag 値は、フォルダーのいずれかの子孫のコンテンツまたはメタデータが変更されると変更されます。eTag 値は、子孫から派生したプロパティ (**childCount** や **lastModifiedDateTime** など) 以外のフォルダーのプロパティが変更されたときにのみ、変更されます。</span><span class="sxs-lookup"><span data-stu-id="ddeb0-p131">**Note:** The eTag and cTag properties work differently on containers (folders). The cTag value is modified when content or metadata of any descendant of the folder is changed. The eTag value is only modified when the folder's properties are changed, except for properties that are derived from descendants (like **childCount** or **lastModifiedDateTime**).</span></span>

## <a name="relationships"></a><span data-ttu-id="ddeb0-252">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="ddeb0-252">Relationships</span></span>

| <span data-ttu-id="ddeb0-253">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="ddeb0-253">Relationship</span></span>       | <span data-ttu-id="ddeb0-254">型</span><span class="sxs-lookup"><span data-stu-id="ddeb0-254">Type</span></span>                        | <span data-ttu-id="ddeb0-255">説明</span><span class="sxs-lookup"><span data-stu-id="ddeb0-255">Description</span></span>
|:-------------------|:----------------------------|:--------------------------
| <span data-ttu-id="ddeb0-256">アクティビティ</span><span class="sxs-lookup"><span data-stu-id="ddeb0-256">activities</span></span>         | <span data-ttu-id="ddeb0-257">[itemActivity][] コレクション</span><span class="sxs-lookup"><span data-stu-id="ddeb0-257">[itemActivity][] collection</span></span> | <span data-ttu-id="ddeb0-258">このアイテムに対して行われた最近のアクティビティのリストです。</span><span class="sxs-lookup"><span data-stu-id="ddeb0-258">The list of recent activities that took place on this item.</span></span>
| <span data-ttu-id="ddeb0-259">分析</span><span class="sxs-lookup"><span data-stu-id="ddeb0-259">analytics</span></span>          | <span data-ttu-id="ddeb0-260">[itemAnalytics][] リソース</span><span class="sxs-lookup"><span data-stu-id="ddeb0-260">[itemAnalytics][] resource</span></span>  | <span data-ttu-id="ddeb0-261">このアイテムについて行われたビュー アクティビティに関する分析。</span><span class="sxs-lookup"><span data-stu-id="ddeb0-261">Analytics about the view activities that took place on this item.</span></span>
| <span data-ttu-id="ddeb0-262">children</span><span class="sxs-lookup"><span data-stu-id="ddeb0-262">children</span></span>           | <span data-ttu-id="ddeb0-263">driveItem コレクション</span><span class="sxs-lookup"><span data-stu-id="ddeb0-263">driveItem collection</span></span>        | <span data-ttu-id="ddeb0-p132">アイテムの直接の子のアイテム オブジェクトを格納するコレクション。子が含まれるのは、フォルダーを表すアイテムのみです。読み取り専用です。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="ddeb0-p132">Collection containing Item objects for the immediate children of Item. Only items representing folders have children. Read-only. Nullable.</span></span>
| <span data-ttu-id="ddeb0-268">createdByUser</span><span class="sxs-lookup"><span data-stu-id="ddeb0-268">createdByUser</span></span>      | <span data-ttu-id="ddeb0-269">[user][]</span><span class="sxs-lookup"><span data-stu-id="ddeb0-269">[user][]</span></span>                    | <span data-ttu-id="ddeb0-270">アイテムを作成したユーザーの ID です。</span><span class="sxs-lookup"><span data-stu-id="ddeb0-270">Identity of the user who created the item.</span></span> <span data-ttu-id="ddeb0-271">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="ddeb0-271">Read-only.</span></span>
| <span data-ttu-id="ddeb0-272">lastModifiedByUser</span><span class="sxs-lookup"><span data-stu-id="ddeb0-272">lastModifiedByUser</span></span> | <span data-ttu-id="ddeb0-273">[user][]</span><span class="sxs-lookup"><span data-stu-id="ddeb0-273">[user][]</span></span>                    | <span data-ttu-id="ddeb0-274">アイテムを最後に変更したユーザーの ID です。</span><span class="sxs-lookup"><span data-stu-id="ddeb0-274">Identity of the user who last modified the item.</span></span> <span data-ttu-id="ddeb0-275">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="ddeb0-275">Read-only.</span></span>
| <span data-ttu-id="ddeb0-276">listItem</span><span class="sxs-lookup"><span data-stu-id="ddeb0-276">listItem</span></span>           | <span data-ttu-id="ddeb0-277">[listItem][]</span><span class="sxs-lookup"><span data-stu-id="ddeb0-277">[listItem][]</span></span>                | <span data-ttu-id="ddeb0-278">SharePoint のドライブの場合は、関連付けられているドキュメント ライブラリのリスト アイテム。</span><span class="sxs-lookup"><span data-stu-id="ddeb0-278">For drives in SharePoint, the associated document library list item.</span></span> <span data-ttu-id="ddeb0-279">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="ddeb0-279">Read-only.</span></span> <span data-ttu-id="ddeb0-280">Null 許容型です。</span><span class="sxs-lookup"><span data-stu-id="ddeb0-280">Nullable.</span></span>
| <span data-ttu-id="ddeb0-281">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="ddeb0-281">permissions</span></span>        | <span data-ttu-id="ddeb0-282">[permission][] コレクション</span><span class="sxs-lookup"><span data-stu-id="ddeb0-282">[permission][] collection</span></span>   | <span data-ttu-id="ddeb0-p136">アイテムのアクセス許可のセット。読み取り専用です。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="ddeb0-p136">The set of permissions for the item. Read-only. Nullable.</span></span>
| <span data-ttu-id="ddeb0-286">subscriptions</span><span class="sxs-lookup"><span data-stu-id="ddeb0-286">subscriptions</span></span>      | <span data-ttu-id="ddeb0-287">[subscription][] コレクション</span><span class="sxs-lookup"><span data-stu-id="ddeb0-287">[subscription][] collection</span></span> | <span data-ttu-id="ddeb0-288">アイテムのサブスクリプションのセット。</span><span class="sxs-lookup"><span data-stu-id="ddeb0-288">The set of subscriptions on the item.</span></span> <span data-ttu-id="ddeb0-289">ドライブのルートでのみサポートされています。</span><span class="sxs-lookup"><span data-stu-id="ddeb0-289">Only supported on the root of a drive.</span></span>
| <span data-ttu-id="ddeb0-290">thumbnails</span><span class="sxs-lookup"><span data-stu-id="ddeb0-290">thumbnails</span></span>         | <span data-ttu-id="ddeb0-291">[thumbnailSet][] コレクション</span><span class="sxs-lookup"><span data-stu-id="ddeb0-291">[thumbnailSet][] collection</span></span> | <span data-ttu-id="ddeb0-p138">アイテムに関連付けられた [ThumbnailSet][] オブジェクトを格納するコレクション。詳細については、[サムネイルの取得][]についてのページをご覧ください。読み取り専用です。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="ddeb0-p138">Collection containing [ThumbnailSet][] objects associated with the item. For more info, see [getting thumbnails][]. Read-only. Nullable.</span></span>
| <span data-ttu-id="ddeb0-296">versions</span><span class="sxs-lookup"><span data-stu-id="ddeb0-296">versions</span></span>           | <span data-ttu-id="ddeb0-297">[driveItemVersion][] コレクション</span><span class="sxs-lookup"><span data-stu-id="ddeb0-297">[driveItemVersion][] collection</span></span> | <span data-ttu-id="ddeb0-298">アイテムの以前のバージョンのリスト。</span><span class="sxs-lookup"><span data-stu-id="ddeb0-298">The list of previous versions of the item.</span></span> <span data-ttu-id="ddeb0-299">詳細については、「[バージョンの一覧表示][]」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ddeb0-299">For more info, see [getting previous versions][].</span></span> <span data-ttu-id="ddeb0-300">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="ddeb0-300">Read-only.</span></span> <span data-ttu-id="ddeb0-301">Null 許容型です。</span><span class="sxs-lookup"><span data-stu-id="ddeb0-301">Nullable.</span></span>
| <span data-ttu-id="ddeb0-302">workbook</span><span class="sxs-lookup"><span data-stu-id="ddeb0-302">workbook</span></span>           | <span data-ttu-id="ddeb0-303">[workbook][]</span><span class="sxs-lookup"><span data-stu-id="ddeb0-303">[workbook][]</span></span>                | <span data-ttu-id="ddeb0-304">Excel スプレッドシートであるファイルの場合、スプレッドシートのコンテンツを操作するためにブックの API にアクセスします。</span><span class="sxs-lookup"><span data-stu-id="ddeb0-304">For files that are Excel spreadsheets, accesses the workbook API to work with the spreadsheet's contents.</span></span> <span data-ttu-id="ddeb0-305">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="ddeb0-305">Nullable.</span></span>

## <a name="instance-attributes"></a><span data-ttu-id="ddeb0-306">インスタンスの属性</span><span class="sxs-lookup"><span data-stu-id="ddeb0-306">Instance Attributes</span></span>

<span data-ttu-id="ddeb0-p141">インスタンスの属性は、動作が特殊なプロパティです。これらのプロパティは一時的なものであり、a) サービスの動作を定義するか、b) 短期的なプロパティの値 (有効期限を持つアイテムのダウンロード URL など) を提供します。</span><span class="sxs-lookup"><span data-stu-id="ddeb0-p141">Instance attributes are properties with special behaviors. These properties are temporary and either a) define behavior the service should perform or b) provide short-term property values, like a download URL for an item that expires.</span></span>

| <span data-ttu-id="ddeb0-309">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="ddeb0-309">Property name</span></span>                     | <span data-ttu-id="ddeb0-310">種類</span><span class="sxs-lookup"><span data-stu-id="ddeb0-310">Type</span></span>   | <span data-ttu-id="ddeb0-311">説明</span><span class="sxs-lookup"><span data-stu-id="ddeb0-311">Description</span></span>
|:----------------------------------|:-------|:--------------------------------
| <span data-ttu-id="ddeb0-312">@microsoft.graph.conflictBehavior</span><span class="sxs-lookup"><span data-stu-id="ddeb0-312">@microsoft.graph.conflictBehavior</span></span> | <span data-ttu-id="ddeb0-313">string</span><span class="sxs-lookup"><span data-stu-id="ddeb0-313">string</span></span> | <span data-ttu-id="ddeb0-p142">新しいアイテムを作成するアクションの競合を解決する動作。*fail*、*replace*、*rename* という値を使用できます。PUT の既定値は *replace* です。この注釈とともにアイテムが返されることはありません。書き込み専用です。</span><span class="sxs-lookup"><span data-stu-id="ddeb0-p142">The conflict resolution behavior for actions that create a new item. You can use the values *fail*, *replace*, or *rename*. The default for PUT is *replace*. An item will never be returned with this annotation. Write-only.</span></span>
| <span data-ttu-id="ddeb0-319">@microsoft.graph.downloadUrl</span><span class="sxs-lookup"><span data-stu-id="ddeb0-319">@microsoft.graph.downloadUrl</span></span>      | <span data-ttu-id="ddeb0-320">string</span><span class="sxs-lookup"><span data-stu-id="ddeb0-320">string</span></span> | <span data-ttu-id="ddeb0-p143">このファイルのコンテンツをダウンロードするために使用できる URL。この URL では認証は必要ありません。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="ddeb0-p143">A URL that can be used to download this file's content. Authentication is not required with this URL. Read-only.</span></span>
| <span data-ttu-id="ddeb0-324">@microsoft.graph.sourceUrl</span><span class="sxs-lookup"><span data-stu-id="ddeb0-324">@microsoft.graph.sourceUrl</span></span>        | <span data-ttu-id="ddeb0-325">string</span><span class="sxs-lookup"><span data-stu-id="ddeb0-325">string</span></span> | <span data-ttu-id="ddeb0-p144">PUT 要求を発行するときにこのインスタンスの注釈を使用すると、サービスに対し、URL のコンテンツをダウンロードし、それをファイルとして保存するように指示できます。書き込み専用です。</span><span class="sxs-lookup"><span data-stu-id="ddeb0-p144">When issuing a PUT request, this instance annotation can be used to instruct the service to download the contents of the URL, and store it as the file. Write-only.</span></span>

<span data-ttu-id="ddeb0-328">**注:**@microsoft.graph.downloadUrl の値は短時間限定の URL であるため、キャッシュすることはできません。</span><span class="sxs-lookup"><span data-stu-id="ddeb0-328">**Note:** The @microsoft.graph.downloadUrl value is a short-lived URL and can't be cached.</span></span>
<span data-ttu-id="ddeb0-329">URL は短い期間 (1 時間) だけ使用でき、その後は無効になります。</span><span class="sxs-lookup"><span data-stu-id="ddeb0-329">The URL will only be available for a short period of time (1 hour) before it is invalidated.</span></span>
<span data-ttu-id="ddeb0-330">ユーザーのファイルへのアクセス許可を削除しても、すぐに URL が無効にならない場合があります。</span><span class="sxs-lookup"><span data-stu-id="ddeb0-330">Removing file permissions for a user may not immediately invalidate the URL.</span></span>

## <a name="methods"></a><span data-ttu-id="ddeb0-331">メソッド</span><span class="sxs-lookup"><span data-stu-id="ddeb0-331">Methods</span></span>

| <span data-ttu-id="ddeb0-332">Method</span><span class="sxs-lookup"><span data-stu-id="ddeb0-332">Method</span></span>                                                   | <span data-ttu-id="ddeb0-333">REST パス</span><span class="sxs-lookup"><span data-stu-id="ddeb0-333">REST Path</span></span>
|:---------------------------------------------------------|:------------------
| [<span data-ttu-id="ddeb0-334">アイテムを取得する</span><span class="sxs-lookup"><span data-stu-id="ddeb0-334">Get item</span></span>](../api/driveitem-get.md)                      | `GET /drive/items/{item-id}`
| [<span data-ttu-id="ddeb0-335">アクティビティを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="ddeb0-335">List activities</span></span>](../api/activities-list.md)             | `GET /drive/items/{item-id}/activities`
| <span data-ttu-id="ddeb0-336">[分析を取得する][]</span><span class="sxs-lookup"><span data-stu-id="ddeb0-336">[Get analytics][]</span></span>                                        | `GET /drive/items/{item-id}/analytics`
| <span data-ttu-id="ddeb0-337">[間隔によりアクティビティを取得する][]</span><span class="sxs-lookup"><span data-stu-id="ddeb0-337">[Get activities by interval][]</span></span>                           | `GET /drive/items/{item-id}/getActivitiesByInterval`
| [<span data-ttu-id="ddeb0-338">子を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="ddeb0-338">List children</span></span>](../api/driveitem-list-children.md)       | `GET /drive/items/{item-id}/children`
| [<span data-ttu-id="ddeb0-339">バージョンを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="ddeb0-339">List versions</span></span>](../api/driveitem-list-versions.md)       | `GET /drive/items/{item-id}/versions`
| [<span data-ttu-id="ddeb0-340">アイテムを作成する</span><span class="sxs-lookup"><span data-stu-id="ddeb0-340">Create item</span></span>](../api/driveitem-post-children.md)         | `POST /drive/items/{item-id}/children`
| [<span data-ttu-id="ddeb0-341">アイテムを更新する</span><span class="sxs-lookup"><span data-stu-id="ddeb0-341">Update item</span></span>](../api/driveitem-update.md)                | `PATCH /drive/items/{item-id}`
| [<span data-ttu-id="ddeb0-342">コンテンツをアップロードする</span><span class="sxs-lookup"><span data-stu-id="ddeb0-342">Upload content</span></span>](../api/driveitem-put-content.md)        | `PUT /drive/items/{item-id}/content`
| [<span data-ttu-id="ddeb0-343">コンテンツをダウンロードする</span><span class="sxs-lookup"><span data-stu-id="ddeb0-343">Download content</span></span>](../api/driveitem-get-content.md)      | `GET /drive/items/{item-id}/content`
| <span data-ttu-id="ddeb0-344">[特定のファイル形式をダウンロードする][download-format]</span><span class="sxs-lookup"><span data-stu-id="ddeb0-344">[Download specific file format][download-format]</span></span>         | `GET /drive/items/{item-id}/content?format={format}`
| [<span data-ttu-id="ddeb0-345">アイテムを削除する</span><span class="sxs-lookup"><span data-stu-id="ddeb0-345">Delete item</span></span>](../api/driveitem-delete.md)                | `DELETE /drive/items/{item-id}`
| [<span data-ttu-id="ddeb0-346">アイテムを移動する</span><span class="sxs-lookup"><span data-stu-id="ddeb0-346">Move item</span></span>](../api/driveitem-move.md)                    | `PATCH /drive/items/{item-id}`
| [<span data-ttu-id="ddeb0-347">アイテムをコピーする</span><span class="sxs-lookup"><span data-stu-id="ddeb0-347">Copy item</span></span>](../api/driveitem-copy.md)                    | `POST /drive/items/{item-id}/copy`
| [<span data-ttu-id="ddeb0-348">アイテムを検索する</span><span class="sxs-lookup"><span data-stu-id="ddeb0-348">Search items</span></span>](../api/driveitem-search.md)               | `GET /drive/items/{item-id}/search(q='text')`
| [<span data-ttu-id="ddeb0-349">ドライブ内の変更内容を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="ddeb0-349">List changes in a drive</span></span>](../api/driveitem-delta.md)     | `GET /drive/root/delta`
| [<span data-ttu-id="ddeb0-350">サムネイルを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="ddeb0-350">List thumbnails</span></span>](../api/driveitem-list-thumbnails.md)   | `GET /drive/items/{item-id}/thumbnails`
| [<span data-ttu-id="ddeb0-351">共有リンクを作成する</span><span class="sxs-lookup"><span data-stu-id="ddeb0-351">Create sharing link</span></span>](../api/driveitem-createlink.md)    | `POST /drive/items/{item-id}/createLink`
| [<span data-ttu-id="ddeb0-352">アクセス許可を追加する</span><span class="sxs-lookup"><span data-stu-id="ddeb0-352">Add permissions</span></span>](../api/driveitem-invite.md)            | `POST /drive/items/{item-id}/invite`
| [<span data-ttu-id="ddeb0-353">アクセス許可を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="ddeb0-353">List permissions</span></span>](../api/driveitem-list-permissions.md) | `GET /drive/items/{item-id}/permissions`
| [<span data-ttu-id="ddeb0-354">アクセス許可を削除する</span><span class="sxs-lookup"><span data-stu-id="ddeb0-354">Delete permission</span></span>](../api/permission-delete.md)         | `DELETE /drive/items/{item-id}/permissions/{perm-id}`
| <span data-ttu-id="ddeb0-355">[WebSocket チャネルを取得する][getWebSocket]</span><span class="sxs-lookup"><span data-stu-id="ddeb0-355">[Get WebSocket channel][getWebSocket]</span></span>                    | `GET /drive/root/subscriptions/socketIo`
| <span data-ttu-id="ddeb0-356">[アイテムをプレビューする][item-preview]</span><span class="sxs-lookup"><span data-stu-id="ddeb0-356">[Preview item][item-preview]</span></span>                             | `POST /drive/items/{item-id}/preview`

[item-preview]: ../api/driveitem-preview.md
[分析を取得する]: ../api/itemanalytics-get.md
[Get analytics]: ../api/itemanalytics-get.md
[間隔によりアクティビティを取得する]: ../api/itemactivity-getbyinterval.md
[Get activities by interval]: ../api/itemactivity-getbyinterval.md

## <a name="remarks"></a><span data-ttu-id="ddeb0-359">注釈</span><span class="sxs-lookup"><span data-stu-id="ddeb0-359">Remarks</span></span>

<span data-ttu-id="ddeb0-360">OneDrive for Business または SharePoint のドキュメント ライブラリでは、**driveItem** に[フォルダー][] ファセットがある場合、**cTag** プロパティは返されません。</span><span class="sxs-lookup"><span data-stu-id="ddeb0-360">In OneDrive for Business or SharePoint document libraries, the **cTag** property is not returned, if the **driveItem** has a [folder][] facet.</span></span>

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
[subscription]: subscription.md
[thumbnailSet]: thumbnailset.md
[ビデオ]: video.md
[video]: video.md
[workbook]: workbook.md
[ユーザー]: https://developer.microsoft.com/graph/docs/api-reference/v1.0/resources/users
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
  "suppressions": []
}
-->
