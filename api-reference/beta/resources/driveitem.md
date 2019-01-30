---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: DriveItem
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: fa172301e633a6f001133d44cb3332a5e133efe2
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/30/2019
ms.locfileid: "29641380"
---
# <a name="driveitem-resource-type"></a><span data-ttu-id="ae72b-102">driveItem リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ae72b-102">driveItem resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ae72b-p101">**driveItem** リソースは、ドライブに格納されているファイル、フォルダーなどのアイテムを表します。OneDrive および SharePoint 内のすべてのファイル システム オブジェクトが、**driveItem** リソースとして返されます。</span><span class="sxs-lookup"><span data-stu-id="ae72b-p101">The **driveItem** resource represents a file, folder, or other item stored in a drive. All file system objects in OneDrive and SharePoint are returned as **driveItem** resources.</span></span>

<span data-ttu-id="ae72b-105">**driveItem** リソースのアドレス指定には、主に 2 つの方法があります。</span><span class="sxs-lookup"><span data-stu-id="ae72b-105">There are two primary ways of addressing a **driveItem** resource:</span></span>

* <span data-ttu-id="ae72b-106">`drive/items/{item-id}` を使用した、**driveItem** 一意識別子による方法</span><span class="sxs-lookup"><span data-stu-id="ae72b-106">By the **driveItem** unique identifier using `drive/items/{item-id}`</span></span>
* <span data-ttu-id="ae72b-107">`/drive/root:/path/to/file` を使用した、ファイル システム パスによる方法</span><span class="sxs-lookup"><span data-stu-id="ae72b-107">By file system path using `/drive/root:/path/to/file`</span></span>

<span data-ttu-id="ae72b-p102">**DriveItem** リソースには、driveItem の ID および機能に関するデータを提供するプロパティとしてモデル化されたファセットがあります。例:</span><span class="sxs-lookup"><span data-stu-id="ae72b-p102">**DriveItem** resources have facets modeled as properties that provide data about the driveItem's identities and capabilities. For example:</span></span>

* <span data-ttu-id="ae72b-110">フォルダーには、[\*\*フォルダー ファセット \*\*][folder] があります</span><span class="sxs-lookup"><span data-stu-id="ae72b-110">Folders have a [**folder facet**][folder]</span></span>
* <span data-ttu-id="ae72b-111">ファイルには、[\*\*ファイル ファセット \*\*][file] があります。</span><span class="sxs-lookup"><span data-stu-id="ae72b-111">Files have a [**file facet**][file].</span></span>
* <span data-ttu-id="ae72b-112">画像には[\*\*画像ファセット \*\*][image] とそのファイル ファセットがあります。</span><span class="sxs-lookup"><span data-stu-id="ae72b-112">Images have an [**image facet**][image] in addition to their file facet.</span></span>
* <span data-ttu-id="ae72b-113">カメラで撮影した画像 (写真) には[\*\*写真ファセット \*\*][photo] があります。写真ファセットは、アイテムを写真として識別し、撮影日時と撮影デバイスのプロパティを提供します。</span><span class="sxs-lookup"><span data-stu-id="ae72b-113">Images taken with a camera (photos) have a [**photo facet**][photo] that identifies the item as a photo and provides the properties of when the photo was taken and with what device.</span></span>

<span data-ttu-id="ae72b-114">**フォルダー** ファセットを持つアイテムは、アイテムのコンテナーとして機能するため、フォルダーに含まれる **driveItems** のコレクションを指す `children` 参照を持ちます。</span><span class="sxs-lookup"><span data-stu-id="ae72b-114">Items with the **folder** facet act as containers of items and therefore have a `children` reference pointing to a collection of **driveItems** under the folder.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ae72b-115">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ae72b-115">JSON representation</span></span>

<span data-ttu-id="ae72b-116">以下は、**driveItem** リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="ae72b-116">Here is a JSON representation of a **driveItem** resource.</span></span>

<span data-ttu-id="ae72b-117">**driveItem** リソースは [**baseItem**][baseItem] から派生し、そのリソースからプロパティを継承します。</span><span class="sxs-lookup"><span data-stu-id="ae72b-117">The **driveItem** resource is derived from [**baseItem**][baseItem] and inherits properties from that resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="ae72b-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ae72b-118">Properties</span></span>

| <span data-ttu-id="ae72b-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ae72b-119">Property</span></span>             | <span data-ttu-id="ae72b-120">型</span><span class="sxs-lookup"><span data-stu-id="ae72b-120">Type</span></span>               | <span data-ttu-id="ae72b-121">説明</span><span class="sxs-lookup"><span data-stu-id="ae72b-121">Description</span></span>
|:---------------------|:-------------------|:---------------------------------
| <span data-ttu-id="ae72b-122">audio</span><span class="sxs-lookup"><span data-stu-id="ae72b-122">audio</span></span>                | <span data-ttu-id="ae72b-123">[audio][]</span><span class="sxs-lookup"><span data-stu-id="ae72b-123">[audio][]</span></span>          | <span data-ttu-id="ae72b-p103">オーディオのメタデータ (アイテムがオーディオ ファイルである場合)。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="ae72b-p103">Audio metadata, if the item is an audio file. Read-only.</span></span>
| <span data-ttu-id="ae72b-126">createdBy</span><span class="sxs-lookup"><span data-stu-id="ae72b-126">createdBy</span></span>            | <span data-ttu-id="ae72b-127">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="ae72b-127">[identitySet][]</span></span>    | <span data-ttu-id="ae72b-p104">そのアイテムを作成したユーザーの ID、デバイス、アプリケーション。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="ae72b-p104">Identity of the user, device, and application which created the item. Read-only.</span></span>
| <span data-ttu-id="ae72b-130">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ae72b-130">createdDateTime</span></span>      | <span data-ttu-id="ae72b-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ae72b-131">DateTimeOffset</span></span>     | <span data-ttu-id="ae72b-p105">アイテム作成の日時。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="ae72b-p105">Date and time of item creation. Read-only.</span></span>
| <span data-ttu-id="ae72b-134">cTag</span><span class="sxs-lookup"><span data-stu-id="ae72b-134">cTag</span></span>                 | <span data-ttu-id="ae72b-135">String</span><span class="sxs-lookup"><span data-stu-id="ae72b-135">String</span></span>             | <span data-ttu-id="ae72b-p106">アイテムのコンテンツの eTag。メタデータのみが変更された場合、この eTag は変更されません。**注:** アイテムがフォルダーである場合、このプロパティは返されません。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="ae72b-p106">An eTag for the content of the item. This eTag is not changed if only the metadata is changed. **Note** This property is not returned if the item is a folder. Read-only.</span></span>
| <span data-ttu-id="ae72b-140">deleted</span><span class="sxs-lookup"><span data-stu-id="ae72b-140">deleted</span></span>              | <span data-ttu-id="ae72b-141">[deleted][]</span><span class="sxs-lookup"><span data-stu-id="ae72b-141">[deleted][]</span></span>        | <span data-ttu-id="ae72b-p107">アイテムの削除状態に関する情報。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="ae72b-p107">Information about the deleted state of the item. Read-only.</span></span>
| <span data-ttu-id="ae72b-144">description</span><span class="sxs-lookup"><span data-stu-id="ae72b-144">description</span></span>          | <span data-ttu-id="ae72b-145">String</span><span class="sxs-lookup"><span data-stu-id="ae72b-145">String</span></span>             | <span data-ttu-id="ae72b-p108">ユーザーに表示されるアイテムの説明を提供します。読み取り/書き込み。OneDrive 個人用においてのみ</span><span class="sxs-lookup"><span data-stu-id="ae72b-p108">Provides a user-visible description of the item. Read-write. Only on OneDrive Personal</span></span>
| <span data-ttu-id="ae72b-149">eTag</span><span class="sxs-lookup"><span data-stu-id="ae72b-149">eTag</span></span>                 | <span data-ttu-id="ae72b-150">String</span><span class="sxs-lookup"><span data-stu-id="ae72b-150">String</span></span>             | <span data-ttu-id="ae72b-p109">アイテム全体 (メタデータおよびコンテンツ) の eTag。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="ae72b-p109">eTag for the entire item (metadata + content). Read-only.</span></span>
| <span data-ttu-id="ae72b-153">file</span><span class="sxs-lookup"><span data-stu-id="ae72b-153">file</span></span>                 | <span data-ttu-id="ae72b-154">[file][]</span><span class="sxs-lookup"><span data-stu-id="ae72b-154">[file][]</span></span>           | <span data-ttu-id="ae72b-p110">ファイルのメタデータ (アイテムがファイルである場合)。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="ae72b-p110">File metadata, if the item is a file. Read-only.</span></span>
| <span data-ttu-id="ae72b-157">fileSystemInfo</span><span class="sxs-lookup"><span data-stu-id="ae72b-157">fileSystemInfo</span></span>       | <span data-ttu-id="ae72b-158">[fileSystemInfo][]</span><span class="sxs-lookup"><span data-stu-id="ae72b-158">[fileSystemInfo][]</span></span> | <span data-ttu-id="ae72b-p111">クライアント上のファイル システム情報。読み取り/書き込み。</span><span class="sxs-lookup"><span data-stu-id="ae72b-p111">File system information on client. Read-write.</span></span>
| <span data-ttu-id="ae72b-161">folder</span><span class="sxs-lookup"><span data-stu-id="ae72b-161">folder</span></span>               | <span data-ttu-id="ae72b-162">[フォルダー][]</span><span class="sxs-lookup"><span data-stu-id="ae72b-162">[folder][]</span></span>         | <span data-ttu-id="ae72b-p112">フォルダーのメタデータ (アイテムがフォルダーである場合)。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="ae72b-p112">Folder metadata, if the item is a folder. Read-only.</span></span>
| <span data-ttu-id="ae72b-165">id</span><span class="sxs-lookup"><span data-stu-id="ae72b-165">id</span></span>                   | <span data-ttu-id="ae72b-166">String</span><span class="sxs-lookup"><span data-stu-id="ae72b-166">String</span></span>             | <span data-ttu-id="ae72b-p113">ドライブ内のアイテムの一意識別子。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="ae72b-p113">The unique identifier of the item within the Drive. Read-only.</span></span>
| <span data-ttu-id="ae72b-169">image</span><span class="sxs-lookup"><span data-stu-id="ae72b-169">image</span></span>                | <span data-ttu-id="ae72b-170">[image][]</span><span class="sxs-lookup"><span data-stu-id="ae72b-170">[image][]</span></span>          | <span data-ttu-id="ae72b-p114">画像のメタデータ (アイテムが画像である場合)。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="ae72b-p114">Image metadata, if the item is an image. Read-only.</span></span>
| <span data-ttu-id="ae72b-173">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="ae72b-173">lastModifiedBy</span></span>       | <span data-ttu-id="ae72b-174">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="ae72b-174">[identitySet][]</span></span>    | <span data-ttu-id="ae72b-p115">アイテムを最終更新したユーザーの ID、デバイス、アプリケーション。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="ae72b-p115">Identity of the user, device, and application which last modified the item. Read-only.</span></span>
| <span data-ttu-id="ae72b-177">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ae72b-177">lastModifiedDateTime</span></span> | <span data-ttu-id="ae72b-178">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ae72b-178">DateTimeOffset</span></span>     | <span data-ttu-id="ae72b-p116">アイテムが最後に変更された日時。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="ae72b-p116">Date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="ae72b-181">location</span><span class="sxs-lookup"><span data-stu-id="ae72b-181">location</span></span>             | <span data-ttu-id="ae72b-182">[geoCoordinates][]</span><span class="sxs-lookup"><span data-stu-id="ae72b-182">[geoCoordinates][]</span></span> | <span data-ttu-id="ae72b-p117">場所のメタデータ (アイテムに場所データが含まれている場合)。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="ae72b-p117">Location metadata, if the item has location data. Read-only.</span></span>
| <span data-ttu-id="ae72b-185">name</span><span class="sxs-lookup"><span data-stu-id="ae72b-185">name</span></span>                 | <span data-ttu-id="ae72b-186">String</span><span class="sxs-lookup"><span data-stu-id="ae72b-186">String</span></span>             | <span data-ttu-id="ae72b-p118">アイテムの名前 (ファイル名と拡張子)。読み取り/書き込み。</span><span class="sxs-lookup"><span data-stu-id="ae72b-p118">The name of the item (filename and extension). Read-write.</span></span>
| <span data-ttu-id="ae72b-189">package</span><span class="sxs-lookup"><span data-stu-id="ae72b-189">package</span></span>              | <span data-ttu-id="ae72b-190">[package][]</span><span class="sxs-lookup"><span data-stu-id="ae72b-190">[package][]</span></span>        | <span data-ttu-id="ae72b-p119">これがある場合、アイテムはフォルダーやファイルではなく、パッケージです。パッケージは、コンテキスト次第で、ファイルとして、あるいはフォルダーとして扱われます。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="ae72b-p119">If present, indicates that this item is a package instead of a folder or file. Packages are treated like files in some contexts and folders in others. Read-only.</span></span>
| <span data-ttu-id="ae72b-194">parentReference</span><span class="sxs-lookup"><span data-stu-id="ae72b-194">parentReference</span></span>      | <span data-ttu-id="ae72b-195">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="ae72b-195">[itemReference][]</span></span>  | <span data-ttu-id="ae72b-p120">親の情報 (アイテムに親がある場合)。読み取り/書き込み。</span><span class="sxs-lookup"><span data-stu-id="ae72b-p120">Parent information, if the item has a parent. Read-write.</span></span>
| <span data-ttu-id="ae72b-198">写真</span><span class="sxs-lookup"><span data-stu-id="ae72b-198">photo</span></span>                | <span data-ttu-id="ae72b-199">[photo][]</span><span class="sxs-lookup"><span data-stu-id="ae72b-199">[photo][]</span></span>          | <span data-ttu-id="ae72b-p121">写真のメタデータ (アイテムが写真である場合)。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="ae72b-p121">Photo metadata, if the item is a photo. Read-only.</span></span>
| <span data-ttu-id="ae72b-202">publication</span><span class="sxs-lookup"><span data-stu-id="ae72b-202">publication</span></span>          | <span data-ttu-id="ae72b-203">[publicationFacet][]</span><span class="sxs-lookup"><span data-stu-id="ae72b-203">[publicationFacet][]</span></span> | <span data-ttu-id="ae72b-204">アイテムが公開されているか、チェックアウトの状態かどうかの情報を、そのような操作をサポートする場所で提供します。</span><span class="sxs-lookup"><span data-stu-id="ae72b-204">Provides information about the published or checked-out state of an item, in locations that support such actions.</span></span> <span data-ttu-id="ae72b-205">既定では、このプロパティは返されません。</span><span class="sxs-lookup"><span data-stu-id="ae72b-205">This property is not returned by default.</span></span> <span data-ttu-id="ae72b-206">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="ae72b-206">Read-only.</span></span> |
| <span data-ttu-id="ae72b-207">remoteItem</span><span class="sxs-lookup"><span data-stu-id="ae72b-207">remoteItem</span></span>           | <span data-ttu-id="ae72b-208">[remoteItem][]</span><span class="sxs-lookup"><span data-stu-id="ae72b-208">[remoteItem][]</span></span>     | <span data-ttu-id="ae72b-p123">リモート アイテムのデータ (現在アクセス中のドライブ以外のドライブから共有されているアイテムの場合)。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="ae72b-p123">Remote item data, if the item is shared from a drive other than the one being accessed. Read-only.</span></span>
| <span data-ttu-id="ae72b-211">root</span><span class="sxs-lookup"><span data-stu-id="ae72b-211">root</span></span>                 | <span data-ttu-id="ae72b-212">[root][]</span><span class="sxs-lookup"><span data-stu-id="ae72b-212">[root][]</span></span>           | <span data-ttu-id="ae72b-213">このプロパティが null ではない場合は、driveItem がドライブで最上位の driveItem であることを示します。</span><span class="sxs-lookup"><span data-stu-id="ae72b-213">If this property is non-null, it indicates that the driveItem is the top-most driveItem in the drive.</span></span>
| <span data-ttu-id="ae72b-214">searchResult</span><span class="sxs-lookup"><span data-stu-id="ae72b-214">searchResult</span></span>         | <span data-ttu-id="ae72b-215">[searchResult][]</span><span class="sxs-lookup"><span data-stu-id="ae72b-215">[searchResult][]</span></span>   | <span data-ttu-id="ae72b-p124">検索のメタデータ (検索結果に由来するアイテムの場合)。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="ae72b-p124">Search metadata, if the item is from a search result. Read-only.</span></span>
| <span data-ttu-id="ae72b-218">共有</span><span class="sxs-lookup"><span data-stu-id="ae72b-218">shared</span></span>               | <span data-ttu-id="ae72b-219">[shared][]</span><span class="sxs-lookup"><span data-stu-id="ae72b-219">[shared][]</span></span>         | <span data-ttu-id="ae72b-p125">アイテムが他のユーザーと共有されていることを示し、アイテムの共有状態に関する情報を提供します。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="ae72b-p125">Indicates that the item has been shared with others and provides information about the shared state of the item. Read-only.</span></span>
| <span data-ttu-id="ae72b-222">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="ae72b-222">sharepointIds</span></span>        | <span data-ttu-id="ae72b-223">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="ae72b-223">[sharepointIds][]</span></span>  | <span data-ttu-id="ae72b-p126">SharePoint REST 互換性に役立つ識別子を返します。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="ae72b-p126">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>
| <span data-ttu-id="ae72b-226">size</span><span class="sxs-lookup"><span data-stu-id="ae72b-226">size</span></span>                 | <span data-ttu-id="ae72b-227">Int64</span><span class="sxs-lookup"><span data-stu-id="ae72b-227">Int64</span></span>              | <span data-ttu-id="ae72b-p127">アイテムのサイズ (バイト単位)。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="ae72b-p127">Size of the item in bytes. Read-only.</span></span>
| <span data-ttu-id="ae72b-230">specialFolder</span><span class="sxs-lookup"><span data-stu-id="ae72b-230">specialFolder</span></span>        | <span data-ttu-id="ae72b-231">[specialFolder][]</span><span class="sxs-lookup"><span data-stu-id="ae72b-231">[specialFolder][]</span></span>  | <span data-ttu-id="ae72b-p128">現在のアイテムが特別なフォルダーとしても使用可能な場合は、このファセットが返されます。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="ae72b-p128">If the current item is also available as a special folder, this facet is returned. Read-only.</span></span>
| <span data-ttu-id="ae72b-234">video</span><span class="sxs-lookup"><span data-stu-id="ae72b-234">video</span></span>                | <span data-ttu-id="ae72b-235">[video][]</span><span class="sxs-lookup"><span data-stu-id="ae72b-235">[video][]</span></span>          | <span data-ttu-id="ae72b-p129">ビデオのメタデータ (アイテムがビデオである場合)。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="ae72b-p129">Video metadata, if the item is a video. Read-only.</span></span>
| <span data-ttu-id="ae72b-238">webDavUrl</span><span class="sxs-lookup"><span data-stu-id="ae72b-238">webDavUrl</span></span>            | <span data-ttu-id="ae72b-239">String</span><span class="sxs-lookup"><span data-stu-id="ae72b-239">String</span></span>             | <span data-ttu-id="ae72b-240">アイテムの WebDAV 互換性のある URL。</span><span class="sxs-lookup"><span data-stu-id="ae72b-240">WebDAV compatible URL for the item.</span></span>
| <span data-ttu-id="ae72b-241">webUrl</span><span class="sxs-lookup"><span data-stu-id="ae72b-241">webUrl</span></span>               | <span data-ttu-id="ae72b-242">String</span><span class="sxs-lookup"><span data-stu-id="ae72b-242">String</span></span>             | <span data-ttu-id="ae72b-p130">ブラウザーでリソースを表示するための URL。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="ae72b-p130">URL that displays the resource in the browser. Read-only.</span></span>

<span data-ttu-id="ae72b-p131">**注:** eTag プロパティと cTag プロパティは、コンテナー (フォルダー) 上での機能が異なります。cTag 値は、フォルダーのいずれかの子孫のコンテンツまたはメタデータが変更されると変更されます。eTag 値は、子孫から派生したプロパティ (**childCount** や **lastModifiedDateTime** など) 以外のフォルダーのプロパティが変更されたときにのみ、変更されます。</span><span class="sxs-lookup"><span data-stu-id="ae72b-p131">**Note:** The eTag and cTag properties work differently on containers (folders). The cTag value is modified when content or metadata of any descendant of the folder is changed. The eTag value is only modified when the folder's properties are changed, except for properties that are derived from descendants (like **childCount** or **lastModifiedDateTime**).</span></span>

## <a name="relationships"></a><span data-ttu-id="ae72b-248">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="ae72b-248">Relationships</span></span>

| <span data-ttu-id="ae72b-249">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="ae72b-249">Relationship</span></span>       | <span data-ttu-id="ae72b-250">型</span><span class="sxs-lookup"><span data-stu-id="ae72b-250">Type</span></span>                            | <span data-ttu-id="ae72b-251">説明</span><span class="sxs-lookup"><span data-stu-id="ae72b-251">Description</span></span>
|:-------------------|:--------------------------------|:--------------------------
| <span data-ttu-id="ae72b-252">アクティビティ</span><span class="sxs-lookup"><span data-stu-id="ae72b-252">activities</span></span>         | <span data-ttu-id="ae72b-253">[itemActivity][] コレクション</span><span class="sxs-lookup"><span data-stu-id="ae72b-253">[itemActivity][] collection</span></span>     | <span data-ttu-id="ae72b-254">このアイテムに対して行われた最近のアクティビティのリストです。</span><span class="sxs-lookup"><span data-stu-id="ae72b-254">The list of recent activities that took place on this item.</span></span>
| <span data-ttu-id="ae72b-255">分析</span><span class="sxs-lookup"><span data-stu-id="ae72b-255">analytics</span></span>          | <span data-ttu-id="ae72b-256">[itemAnalytics][]リソース</span><span class="sxs-lookup"><span data-stu-id="ae72b-256">[itemAnalytics][] resource</span></span>      | <span data-ttu-id="ae72b-257">この項目に対して行われた活動の表示について分析します。</span><span class="sxs-lookup"><span data-stu-id="ae72b-257">Analytics about the view activities that took place on this item.</span></span>
| <span data-ttu-id="ae72b-258">content</span><span class="sxs-lookup"><span data-stu-id="ae72b-258">content</span></span>            | <span data-ttu-id="ae72b-259">Stream</span><span class="sxs-lookup"><span data-stu-id="ae72b-259">Stream</span></span>                          | <span data-ttu-id="ae72b-260">コンテンツのストリーム (アイテムがファイルを表す場合)。</span><span class="sxs-lookup"><span data-stu-id="ae72b-260">The content stream, if the item represents a file.</span></span>
| <span data-ttu-id="ae72b-261">children</span><span class="sxs-lookup"><span data-stu-id="ae72b-261">children</span></span>           | <span data-ttu-id="ae72b-262">driveitem コレクション</span><span class="sxs-lookup"><span data-stu-id="ae72b-262">driveitem collection</span></span>            | <span data-ttu-id="ae72b-p132">アイテムの直接の子のアイテム オブジェクトを格納するコレクション。子が含まれるのは、フォルダーを表すアイテムのみです。読み取り専用です。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="ae72b-p132">Collection containing Item objects for the immediate children of Item. Only items representing folders have children. Read-only. Nullable.</span></span>
| <span data-ttu-id="ae72b-267">listItem</span><span class="sxs-lookup"><span data-stu-id="ae72b-267">listItem</span></span>           | <span data-ttu-id="ae72b-268">[listItem][]</span><span class="sxs-lookup"><span data-stu-id="ae72b-268">[listItem][]</span></span>                    | <span data-ttu-id="ae72b-269">SharePoint 内のドライブ、関連するドキュメント ライブラリのアイテムをリストします。</span><span class="sxs-lookup"><span data-stu-id="ae72b-269">For drives in SharePoint, the associated document library list item.</span></span> <span data-ttu-id="ae72b-270">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="ae72b-270">Read-only.</span></span> <span data-ttu-id="ae72b-271">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="ae72b-271">Nullable.</span></span>
| <span data-ttu-id="ae72b-272">permissions</span><span class="sxs-lookup"><span data-stu-id="ae72b-272">permissions</span></span>        | <span data-ttu-id="ae72b-273">[permission][] コレクション</span><span class="sxs-lookup"><span data-stu-id="ae72b-273">[permission][] collection</span></span>       | <span data-ttu-id="ae72b-p134">アイテムのアクセス許可のセット。読み取り専用です。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="ae72b-p134">The set of permissions for the item. Read-only. Nullable.</span></span>
| <span data-ttu-id="ae72b-277">thumbnails</span><span class="sxs-lookup"><span data-stu-id="ae72b-277">thumbnails</span></span>         | <span data-ttu-id="ae72b-278">[thumbnailSet][] コレクション</span><span class="sxs-lookup"><span data-stu-id="ae72b-278">[thumbnailSet][] collection</span></span>     | <span data-ttu-id="ae72b-p135">アイテムに関連付けられた [ThumbnailSet][] オブジェクトを格納するコレクション。詳細については、[サムネイルの取得][]についてのページをご覧ください。読み取り専用です。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="ae72b-p135">Collection containing [ThumbnailSet][] objects associated with the item. For more info, see [getting thumbnails][]. Read-only. Nullable.</span></span>
| <span data-ttu-id="ae72b-283">versions</span><span class="sxs-lookup"><span data-stu-id="ae72b-283">versions</span></span>           | <span data-ttu-id="ae72b-284">[driveItemVersion][]コレクション</span><span class="sxs-lookup"><span data-stu-id="ae72b-284">[driveItemVersion][] collection</span></span> | <span data-ttu-id="ae72b-285">アイテムの以前のバージョンの一覧です。</span><span class="sxs-lookup"><span data-stu-id="ae72b-285">The list of previous versions of the item.</span></span> <span data-ttu-id="ae72b-286">詳細については、[以前のバージョンを取得する][]を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ae72b-286">For more info, see [getting previous versions][].</span></span> <span data-ttu-id="ae72b-287">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="ae72b-287">Read-only.</span></span> <span data-ttu-id="ae72b-288">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="ae72b-288">Nullable.</span></span>

## <a name="instance-attributes"></a><span data-ttu-id="ae72b-289">インスタンスの属性</span><span class="sxs-lookup"><span data-stu-id="ae72b-289">Instance Attributes</span></span>

<span data-ttu-id="ae72b-p137">インスタンスの属性は、動作が特殊なプロパティです。これらのプロパティは一時的なものであり、a) サービスの動作を定義するか、b) 短期的なプロパティの値 (有効期限を持つアイテムのダウンロード URL など) を提供します。</span><span class="sxs-lookup"><span data-stu-id="ae72b-p137">Instance attributes are properties with special behaviors. These properties are temporary and either a) define behavior the service should perform or b) provide short-term property values, like a download URL for an item that expires.</span></span>

| <span data-ttu-id="ae72b-292">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="ae72b-292">Property name</span></span>                     | <span data-ttu-id="ae72b-293">型</span><span class="sxs-lookup"><span data-stu-id="ae72b-293">Type</span></span>   | <span data-ttu-id="ae72b-294">説明</span><span class="sxs-lookup"><span data-stu-id="ae72b-294">Description</span></span>
|:----------------------------------|:-------|:--------------------------------
| <span data-ttu-id="ae72b-295">@microsoft.graph.conflictBehavior</span><span class="sxs-lookup"><span data-stu-id="ae72b-295">@microsoft.graph.conflictBehavior</span></span> | <span data-ttu-id="ae72b-296">string</span><span class="sxs-lookup"><span data-stu-id="ae72b-296">string</span></span> | <span data-ttu-id="ae72b-p138">新しいアイテムを作成するアクションの競合を解決する動作。*fail*、*replace*、*rename* という値を使用できます。PUT の既定値は *replace* です。この注釈とともにアイテムが返されることはありません。書き込み専用です。</span><span class="sxs-lookup"><span data-stu-id="ae72b-p138">The conflict resolution behavior for actions that create a new item. You can use the values *fail*, *replace*, or *rename*. The default for PUT is *replace*. An item will never be returned with this annotation. Write-only.</span></span>
| <span data-ttu-id="ae72b-302">@microsoft.graph.downloadUrl</span><span class="sxs-lookup"><span data-stu-id="ae72b-302">@microsoft.graph.downloadUrl</span></span>      | <span data-ttu-id="ae72b-303">string</span><span class="sxs-lookup"><span data-stu-id="ae72b-303">string</span></span> | <span data-ttu-id="ae72b-p139">このファイルのコンテンツをダウンロードするために使用できる URL。この URL では認証は必要ありません。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="ae72b-p139">A URL that can be used to download this file's content. Authentication is not required with this URL. Read-only.</span></span>
| <span data-ttu-id="ae72b-307">@microsoft.graph.sourceUrl</span><span class="sxs-lookup"><span data-stu-id="ae72b-307">@microsoft.graph.sourceUrl</span></span>        | <span data-ttu-id="ae72b-308">string</span><span class="sxs-lookup"><span data-stu-id="ae72b-308">string</span></span> | <span data-ttu-id="ae72b-p140">PUT 要求を発行するときにこのインスタンスの注釈を使用すると、サービスに対し、URL のコンテンツをダウンロードし、それをファイルとして保存するように指示できます。書き込み専用です。</span><span class="sxs-lookup"><span data-stu-id="ae72b-p140">When issuing a PUT request, this instance annotation can be used to instruct the service to download the contents of the URL, and store it as the file. Write-only.</span></span>

<span data-ttu-id="ae72b-311">**注:**@Microsoft.graph.downloadUrl 値は短時間の URL であるため、キャッシュすることはできません。</span><span class="sxs-lookup"><span data-stu-id="ae72b-311">**Note:** The @microsoft.graph.downloadUrl value is a short-lived URL and can't be cached.</span></span>
<span data-ttu-id="ae72b-312">URL は、短時間 (1 時間) が無効になる前にのみ使用できます。</span><span class="sxs-lookup"><span data-stu-id="ae72b-312">The URL will only be available for a short period of time (1 hour) before it is invalidated.</span></span> <span data-ttu-id="ae72b-313">ユーザーに対するファイル アクセス許可を削除する可能性がありますすぐに無効の URL。</span><span class="sxs-lookup"><span data-stu-id="ae72b-313">Removing file permissions for a user may not immediately invalidate the URL.</span></span>

## <a name="methods"></a><span data-ttu-id="ae72b-314">メソッド</span><span class="sxs-lookup"><span data-stu-id="ae72b-314">Methods</span></span>

| <span data-ttu-id="ae72b-315">メソッド</span><span class="sxs-lookup"><span data-stu-id="ae72b-315">Method</span></span>                                                   | <span data-ttu-id="ae72b-316">REST パス</span><span class="sxs-lookup"><span data-stu-id="ae72b-316">REST Path</span></span>
|:---------------------------------------------------------|:------------------
| [<span data-ttu-id="ae72b-317">アイテムを取得する</span><span class="sxs-lookup"><span data-stu-id="ae72b-317">Get item</span></span>](../api/driveitem-get.md)                      | `GET /drive/items/{item-id}`
| [<span data-ttu-id="ae72b-318">アクティビティを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="ae72b-318">List activities</span></span>](../api/activities-list.md)             | `GET /drive/items/{item-id}/activities`
| <span data-ttu-id="ae72b-319">[分析を取得します。][]</span><span class="sxs-lookup"><span data-stu-id="ae72b-319">[Get analytics][]</span></span>                                        | `GET /drive/items/{item-id}/analytics`
| <span data-ttu-id="ae72b-320">[間隔によってアクティビティを取得します。][]</span><span class="sxs-lookup"><span data-stu-id="ae72b-320">[Get activities by interval][]</span></span>                           | `GET /drive/items/{item-id}/getActivitiesByInterval`
| [<span data-ttu-id="ae72b-321">子を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="ae72b-321">List children</span></span>](../api/driveitem-list-children.md)       | `GET /drive/items/{item-id}/children`
| [<span data-ttu-id="ae72b-322">バージョンの一覧表示</span><span class="sxs-lookup"><span data-stu-id="ae72b-322">List versions</span></span>](../api/driveitem-list-versions.md)       | `GET /drive/items/{item-id}/versions`
| [<span data-ttu-id="ae72b-323">アイテムを作成する</span><span class="sxs-lookup"><span data-stu-id="ae72b-323">Create item</span></span>](../api/driveitem-post-children.md)         | `POST /drive/items/{item-id}/children`
| [<span data-ttu-id="ae72b-324">アイテムを更新する</span><span class="sxs-lookup"><span data-stu-id="ae72b-324">Update item</span></span>](../api/driveitem-update.md)                | `PATCH /drive/items/{item-id}`
| [<span data-ttu-id="ae72b-325">コンテンツをアップロードする</span><span class="sxs-lookup"><span data-stu-id="ae72b-325">Upload content</span></span>](../api/driveitem-put-content.md)        | `PUT /drive/items/{item-id}/content`
| [<span data-ttu-id="ae72b-326">コンテンツをダウンロードする</span><span class="sxs-lookup"><span data-stu-id="ae72b-326">Download content</span></span>](../api/driveitem-get-content.md)      | `GET /drive/items/{item-id}/content`
| <span data-ttu-id="ae72b-327">[特定のファイル形式をダウンロードする][download-format]</span><span class="sxs-lookup"><span data-stu-id="ae72b-327">[Download specific file format][download-format]</span></span>         | `GET /drive/items/{item-id}/content?format={format}`
| [<span data-ttu-id="ae72b-328">アイテムを削除する</span><span class="sxs-lookup"><span data-stu-id="ae72b-328">Delete item</span></span>](../api/driveitem-delete.md)                | `DELETE /drive/items/{item-id}`
| [<span data-ttu-id="ae72b-329">アイテムを移動する</span><span class="sxs-lookup"><span data-stu-id="ae72b-329">Move item</span></span>](../api/driveitem-move.md)                    | `PATCH /drive/items/{item-id}`
| [<span data-ttu-id="ae72b-330">アイテムをコピーする</span><span class="sxs-lookup"><span data-stu-id="ae72b-330">Copy item</span></span>](../api/driveitem-copy.md)                    | `POST /drive/items/{item-id}/copy`
| [<span data-ttu-id="ae72b-331">アイテムを検索する</span><span class="sxs-lookup"><span data-stu-id="ae72b-331">Search items</span></span>](../api/driveitem-search.md)               | `GET /drive/items/{item-id}/search(q='text')`
| [<span data-ttu-id="ae72b-332">ドライブ内の変更内容を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="ae72b-332">List changes in a drive</span></span>](../api/driveitem-delta.md)     | `GET /drive/root/delta`
| [<span data-ttu-id="ae72b-333">サムネイルを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="ae72b-333">List thumbnails</span></span>](../api/driveitem-list-thumbnails.md)   | `GET /drive/items/{item-id}/thumbnails`
| [<span data-ttu-id="ae72b-334">共有リンクを作成する</span><span class="sxs-lookup"><span data-stu-id="ae72b-334">Create sharing link</span></span>](../api/driveitem-createlink.md)    | `POST /drive/items/{item-id}/createLink`
| [<span data-ttu-id="ae72b-335">アクセス許可を追加する</span><span class="sxs-lookup"><span data-stu-id="ae72b-335">Add permissions</span></span>](../api/driveitem-invite.md)            | `POST /drive/items/{item-id}/invite`
| [<span data-ttu-id="ae72b-336">アクセス許可を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="ae72b-336">List permissions</span></span>](../api/driveitem-list-permissions.md) | `GET /drive/items/{item-id}/permissions`
| [<span data-ttu-id="ae72b-337">アクセス許可を削除する</span><span class="sxs-lookup"><span data-stu-id="ae72b-337">Delete permission</span></span>](../api/permission-delete.md)         | `DELETE /drive/items/{item-id}/permissions/{perm-id}`
| <span data-ttu-id="ae72b-338">[WebSocket のチャネルを取得します。][getWebSocket]</span><span class="sxs-lookup"><span data-stu-id="ae72b-338">[Get WebSocket channel][getWebSocket]</span></span>                    | `GET /drive/root/subscriptions/socketIo`
| <span data-ttu-id="ae72b-339">[アイテムのプレビュー][item-preview]</span><span class="sxs-lookup"><span data-stu-id="ae72b-339">[Preview item][item-preview]</span></span>                             | `POST /drive/items/{item-id}/preview`

[item-preview]: ../api/driveitem-preview.md
[分析を取得します。]: ../api/itemanalytics-get.md
[Get analytics]: ../api/itemanalytics-get.md
[間隔によってアクティビティを取得します。]: ../api/itemactivity-getbyinterval.md
[Get activities by interval]: ../api/itemactivity-getbyinterval.md

## <a name="remarks"></a><span data-ttu-id="ae72b-342">備考</span><span class="sxs-lookup"><span data-stu-id="ae72b-342">Remarks</span></span>

<span data-ttu-id="ae72b-343">OneDrive for Business または SharePoint のドキュメント ライブラリでは、**driveItem** に[フォルダー][] ファセットがある場合、**cTag** プロパティは返されません。</span><span class="sxs-lookup"><span data-stu-id="ae72b-343">In OneDrive for Business or SharePoint document libraries, the **cTag** property is not returned, if the **driveItem** has a [folder][] facet.</span></span>

[audio]: audio.md
[baseItem]: baseitem.md
[deleted]: deleted.md
[download-format]: ../api/driveitem-get-content-format.md
[driveItemVersion]: driveitemversion.md
[file]: file.md
[fileSystemInfo]: filesysteminfo.md
[folder]: folder.md
[以前のバージョンを取得します。]: ../api/driveitem-list-versions.md
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
