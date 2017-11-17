---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: DriveItem
ms.openlocfilehash: 526001ad9a6c52c5b031c1734466772861f1c67e
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/28/2017
---
# <a name="driveitem-resource-type"></a><span data-ttu-id="dfda8-102">DriveItem リソース型</span><span class="sxs-lookup"><span data-stu-id="dfda8-102">DriveItem resource type</span></span>

<span data-ttu-id="dfda8-p101">**driveItem** リソースは、ドライブに格納されているファイル、フォルダーなどのアイテムを表します。OneDrive および SharePoint 内のすべてのファイル システム オブジェクトが、**driveItem** リソースとして返されます。</span><span class="sxs-lookup"><span data-stu-id="dfda8-p101">The **driveItem** resource represents a file, folder, or other item stored in a drive. All file system objects in OneDrive and SharePoint are returned as **driveItem** resources.</span></span>

<span data-ttu-id="dfda8-105">**driveItem** リソースのアドレス指定には、主に 2 つの方法があります。</span><span class="sxs-lookup"><span data-stu-id="dfda8-105">There are two primary ways of addressing a **driveItem** resource:</span></span>

* <span data-ttu-id="dfda8-106">`drive/items/{item-id}` を使用した、**driveItem** 一意識別子による方法</span><span class="sxs-lookup"><span data-stu-id="dfda8-106">By the **driveItem** unique identifier using `drive/items/{item-id}`</span></span>
* <span data-ttu-id="dfda8-107">`/drive/root:/path/to/file` を使用した、ファイル システム パスによる方法</span><span class="sxs-lookup"><span data-stu-id="dfda8-107">By file system path using `/drive/root:/path/to/file`</span></span>

<span data-ttu-id="dfda8-p102">**DriveItem** リソースには、driveItem の ID および機能に関するデータを提供するプロパティとしてモデル化されたファセットがあります。例:</span><span class="sxs-lookup"><span data-stu-id="dfda8-p102">**DriveItem** resources have facets modeled as properties that provide data about the driveItem's identities and capabilities. For example:</span></span>

* <span data-ttu-id="dfda8-110">フォルダーには、[**フォルダー ファセット **][folder] があります。</span><span class="sxs-lookup"><span data-stu-id="dfda8-110">Folders have a [**folder facet**]</span></span>
* <span data-ttu-id="dfda8-111">ファイルには、[**ファイル ファセット **][file] があります。</span><span class="sxs-lookup"><span data-stu-id="dfda8-111">Files have a [**file facet**].</span></span>
* <span data-ttu-id="dfda8-112">画像には[**画像ファセット **][image] とそのファイル ファセットがあります。</span><span class="sxs-lookup"><span data-stu-id="dfda8-112">Images have an [**image facet**] in addition to their file facet.</span></span>
* <span data-ttu-id="dfda8-113">カメラで撮影した画像 (写真) には[**写真ファセット **][photo] があります。写真ファセットは、アイテムを写真として識別し、撮影日時と撮影デバイスのプロパティを提供します。</span><span class="sxs-lookup"><span data-stu-id="dfda8-113">Images taken with a camera (photos) have a [**photo facet**] that identifies the item as a photo and provides the properties of when the photo was taken and with what device.</span></span>

<span data-ttu-id="dfda8-114">**フォルダー** ファセットを持つアイテムは、アイテムのコンテナーとして機能するため、フォルダーに含まれる **driveItems** のコレクションを指す `children` 参照を持ちます。</span><span class="sxs-lookup"><span data-stu-id="dfda8-114">Items with the **folder** facet act as containers of items and therefore have a `children` reference pointing to a collection of **driveItems** under the folder.</span></span>

## <a name="json-representation"></a><span data-ttu-id="dfda8-115">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="dfda8-115">JSON representation</span></span>

<span data-ttu-id="dfda8-116">以下は、**driveItem** リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="dfda8-116">Here is a JSON representation of a **driveItem** resource.</span></span>

<span data-ttu-id="dfda8-117">**driveItem** リソースは [**baseItem**][baseItem] から派生し、そのリソースからプロパティを継承します。</span><span class="sxs-lookup"><span data-stu-id="dfda8-117">The **driveItem** resource is derived from [**baseItem**] and inherits properties from that resource.</span></span>

<!-- { "blockType": "resource", "@type": "microsoft.graph.driveItem", "@type.aka": "oneDrive.item",
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

## <a name="properties"></a><span data-ttu-id="dfda8-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="dfda8-118">Properties</span></span>

| <span data-ttu-id="dfda8-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="dfda8-119">Property</span></span>             | <span data-ttu-id="dfda8-120">型</span><span class="sxs-lookup"><span data-stu-id="dfda8-120">Type</span></span>               | <span data-ttu-id="dfda8-121">説明</span><span class="sxs-lookup"><span data-stu-id="dfda8-121">Description</span></span>
|:---------------------|:-------------------|:---------------------------------
| <span data-ttu-id="dfda8-122">audio</span><span class="sxs-lookup"><span data-stu-id="dfda8-122">audio</span></span>                | <span data-ttu-id="dfda8-123">[audio][]</span><span class="sxs-lookup"><span data-stu-id="dfda8-123">[audio][]</span></span>          | <span data-ttu-id="dfda8-p103">オーディオのメタデータ (アイテムがオーディオ ファイルである場合)。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="dfda8-p103">Audio metadata, if the item is an audio file. Read-only.</span></span>
| <span data-ttu-id="dfda8-126">createdBy</span><span class="sxs-lookup"><span data-stu-id="dfda8-126">createdBy</span></span>            | <span data-ttu-id="dfda8-127">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="dfda8-127">[identitySet][]</span></span>    | <span data-ttu-id="dfda8-p104">そのアイテムを作成したユーザーの ID、デバイス、アプリケーション。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="dfda8-p104">Identity of the user, device, and application which created the item. Read-only.</span></span>
| <span data-ttu-id="dfda8-130">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="dfda8-130">createdDateTime</span></span>      | <span data-ttu-id="dfda8-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dfda8-131">DateTimeOffset</span></span>     | <span data-ttu-id="dfda8-p105">アイテム作成の日時。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="dfda8-p105">Date and time of item creation. Read-only.</span></span>
| <span data-ttu-id="dfda8-134">cTag</span><span class="sxs-lookup"><span data-stu-id="dfda8-134">cTag</span></span>                 | <span data-ttu-id="dfda8-135">String</span><span class="sxs-lookup"><span data-stu-id="dfda8-135">String</span></span>             | <span data-ttu-id="dfda8-p106">アイテムのコンテンツの eTag。メタデータのみが変更された場合、この eTag は変更されません。**注:** アイテムがフォルダーである場合、このプロパティは返されません。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="dfda8-p106">An eTag for the content of the item. This eTag is not changed if only the metadata is changed. **Note** This property is not returned if the item is a folder. Read-only.</span></span>
| <span data-ttu-id="dfda8-140">deleted</span><span class="sxs-lookup"><span data-stu-id="dfda8-140">deleted</span></span>              | <span data-ttu-id="dfda8-141">[deleted][]</span><span class="sxs-lookup"><span data-stu-id="dfda8-141">[deleted][]</span></span>        | <span data-ttu-id="dfda8-p107">アイテムの削除状態に関する情報。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="dfda8-p107">Information about the deleted state of the item. Read-only.</span></span>
| <span data-ttu-id="dfda8-144">description</span><span class="sxs-lookup"><span data-stu-id="dfda8-144">description</span></span>          | <span data-ttu-id="dfda8-145">String</span><span class="sxs-lookup"><span data-stu-id="dfda8-145">String</span></span>             | <span data-ttu-id="dfda8-p108">ユーザーに表示されるアイテムの説明を提供します。読み取り/書き込み。OneDrive 個人用においてのみ</span><span class="sxs-lookup"><span data-stu-id="dfda8-p108">Provides a user-visible description of the item. Read-write. Only on OneDrive Personal</span></span>
| <span data-ttu-id="dfda8-149">eTag</span><span class="sxs-lookup"><span data-stu-id="dfda8-149">eTag</span></span>                 | <span data-ttu-id="dfda8-150">String</span><span class="sxs-lookup"><span data-stu-id="dfda8-150">String</span></span>             | <span data-ttu-id="dfda8-p109">アイテム全体 (メタデータおよびコンテンツ) の eTag。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="dfda8-p109">eTag for the entire item (metadata + content). Read-only.</span></span>
| <span data-ttu-id="dfda8-153">file</span><span class="sxs-lookup"><span data-stu-id="dfda8-153">file</span></span>                 | <span data-ttu-id="dfda8-154">[file][]</span><span class="sxs-lookup"><span data-stu-id="dfda8-154">[file][]</span></span>           | <span data-ttu-id="dfda8-p110">ファイルのメタデータ (アイテムがファイルである場合)。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="dfda8-p110">File metadata, if the item is a file. Read-only.</span></span>
| <span data-ttu-id="dfda8-157">fileSystemInfo</span><span class="sxs-lookup"><span data-stu-id="dfda8-157">fileSystemInfo</span></span>       | <span data-ttu-id="dfda8-158">[fileSystemInfo][]</span><span class="sxs-lookup"><span data-stu-id="dfda8-158">[fileSystemInfo][]</span></span> | <span data-ttu-id="dfda8-p111">クライアント上のファイル システム情報。読み取り/書き込み。</span><span class="sxs-lookup"><span data-stu-id="dfda8-p111">File system information on client. Read-write.</span></span>
| <span data-ttu-id="dfda8-161">folder</span><span class="sxs-lookup"><span data-stu-id="dfda8-161">folder</span></span>               | <span data-ttu-id="dfda8-162">[folder][]</span><span class="sxs-lookup"><span data-stu-id="dfda8-162">[folder][]</span></span>         | <span data-ttu-id="dfda8-p112">フォルダーのメタデータ (アイテムがフォルダーである場合)。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="dfda8-p112">Folder metadata, if the item is a folder. Read-only.</span></span>
| <span data-ttu-id="dfda8-165">id</span><span class="sxs-lookup"><span data-stu-id="dfda8-165">id</span></span>                   | <span data-ttu-id="dfda8-166">String</span><span class="sxs-lookup"><span data-stu-id="dfda8-166">String</span></span>             | <span data-ttu-id="dfda8-p113">ドライブ内のアイテムの一意識別子。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="dfda8-p113">The unique identifier of the item within the Drive. Read-only.</span></span>
| <span data-ttu-id="dfda8-169">image</span><span class="sxs-lookup"><span data-stu-id="dfda8-169">image</span></span>                | <span data-ttu-id="dfda8-170">[image][]</span><span class="sxs-lookup"><span data-stu-id="dfda8-170">[image][]</span></span>          | <span data-ttu-id="dfda8-p114">画像のメタデータ (アイテムが画像である場合)。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="dfda8-p114">Image metadata, if the item is an image. Read-only.</span></span>
| <span data-ttu-id="dfda8-173">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="dfda8-173">lastModifiedBy</span></span>       | <span data-ttu-id="dfda8-174">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="dfda8-174">[identitySet][]</span></span>    | <span data-ttu-id="dfda8-p115">アイテムを最終更新したユーザーの ID、デバイス、アプリケーション。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="dfda8-p115">Identity of the user, device, and application which last modified the item. Read-only.</span></span>
| <span data-ttu-id="dfda8-177">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="dfda8-177">lastModifiedDateTime</span></span> | <span data-ttu-id="dfda8-178">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dfda8-178">DateTimeOffset</span></span>     | <span data-ttu-id="dfda8-p116">アイテムが最後に変更された日時。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="dfda8-p116">Date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="dfda8-181">location</span><span class="sxs-lookup"><span data-stu-id="dfda8-181">location</span></span>             | <span data-ttu-id="dfda8-182">[geoCoordinates][]</span><span class="sxs-lookup"><span data-stu-id="dfda8-182">[geoCoordinates][]</span></span> | <span data-ttu-id="dfda8-p117">場所のメタデータ (アイテムに場所データが含まれている場合)。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="dfda8-p117">Location metadata, if the item has location data. Read-only.</span></span>
| <span data-ttu-id="dfda8-185">name</span><span class="sxs-lookup"><span data-stu-id="dfda8-185">name</span></span>                 | <span data-ttu-id="dfda8-186">String</span><span class="sxs-lookup"><span data-stu-id="dfda8-186">String</span></span>             | <span data-ttu-id="dfda8-p118">アイテムの名前 (ファイル名と拡張子)。読み取り/書き込み。</span><span class="sxs-lookup"><span data-stu-id="dfda8-p118">The name of the item (filename and extension). Read-write.</span></span>
| <span data-ttu-id="dfda8-189">package</span><span class="sxs-lookup"><span data-stu-id="dfda8-189">package</span></span>              | <span data-ttu-id="dfda8-190">[package][]</span><span class="sxs-lookup"><span data-stu-id="dfda8-190">[package][]</span></span>        | <span data-ttu-id="dfda8-p119">これがある場合、アイテムはフォルダーやファイルではなく、パッケージです。パッケージは、コンテキスト次第で、ファイルとして、あるいはフォルダーとして扱われます。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="dfda8-p119">If present, indicates that this item is a package instead of a folder or file. Packages are treated like files in some contexts and folders in others. Read-only.</span></span>
| <span data-ttu-id="dfda8-194">parentReference</span><span class="sxs-lookup"><span data-stu-id="dfda8-194">parentReference</span></span>      | <span data-ttu-id="dfda8-195">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="dfda8-195">[itemReference][]</span></span>  | <span data-ttu-id="dfda8-p120">親の情報 (アイテムに親がある場合)。読み取り/書き込み。</span><span class="sxs-lookup"><span data-stu-id="dfda8-p120">Parent information, if the item has a parent. Read-write.</span></span>
| <span data-ttu-id="dfda8-198">写真</span><span class="sxs-lookup"><span data-stu-id="dfda8-198">photo</span></span>                | <span data-ttu-id="dfda8-199">[photo][]</span><span class="sxs-lookup"><span data-stu-id="dfda8-199">[photo][]</span></span>          | <span data-ttu-id="dfda8-p121">写真のメタデータ (アイテムが写真である場合)。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="dfda8-p121">Photo metadata, if the item is a photo. Read-only.</span></span>
| <span data-ttu-id="dfda8-202">remoteItem</span><span class="sxs-lookup"><span data-stu-id="dfda8-202">remoteItem</span></span>           | <span data-ttu-id="dfda8-203">[remoteItem][]</span><span class="sxs-lookup"><span data-stu-id="dfda8-203">[remoteItem][]</span></span>     | <span data-ttu-id="dfda8-p122">リモート アイテムのデータ (現在アクセス中のドライブ以外のドライブから共有されているアイテムの場合)。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="dfda8-p122">Remote item data, if the item is shared from a drive other than the one being accessed. Read-only.</span></span>
| <span data-ttu-id="dfda8-206">root</span><span class="sxs-lookup"><span data-stu-id="dfda8-206">root</span></span>                 | <span data-ttu-id="dfda8-207">[root][]</span><span class="sxs-lookup"><span data-stu-id="dfda8-207">[root][]</span></span>           | <span data-ttu-id="dfda8-208">このプロパティが null ではない場合は、driveItem がドライブで最上位の driveItem であることを示します。</span><span class="sxs-lookup"><span data-stu-id="dfda8-208">If this property is non-null, it indicates that the driveItem is the top-most driveItem in the drive.</span></span>
| <span data-ttu-id="dfda8-209">searchResult</span><span class="sxs-lookup"><span data-stu-id="dfda8-209">searchResult</span></span>         | <span data-ttu-id="dfda8-210">[searchResult][]</span><span class="sxs-lookup"><span data-stu-id="dfda8-210">[searchResult][]</span></span>   | <span data-ttu-id="dfda8-p123">検索のメタデータ (検索結果に由来するアイテムの場合)。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="dfda8-p123">Search metadata, if the item is from a search result. Read-only.</span></span>
| <span data-ttu-id="dfda8-213">共有</span><span class="sxs-lookup"><span data-stu-id="dfda8-213">shared</span></span>               | <span data-ttu-id="dfda8-214">[shared][]</span><span class="sxs-lookup"><span data-stu-id="dfda8-214">[shared][]</span></span>         | <span data-ttu-id="dfda8-p124">アイテムが他のユーザーと共有されていることを示し、アイテムの共有状態に関する情報を提供します。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="dfda8-p124">Indicates that the item has been shared with others and provides information about the shared state of the item. Read-only.</span></span>
| <span data-ttu-id="dfda8-217">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="dfda8-217">sharepointIds</span></span>        | <span data-ttu-id="dfda8-218">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="dfda8-218">[sharepointIds][]</span></span>  | <span data-ttu-id="dfda8-p125">SharePoint REST 互換性に役立つ識別子を返します。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="dfda8-p125">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>
| <span data-ttu-id="dfda8-221">size</span><span class="sxs-lookup"><span data-stu-id="dfda8-221">size</span></span>                 | <span data-ttu-id="dfda8-222">Int64</span><span class="sxs-lookup"><span data-stu-id="dfda8-222">Int64</span></span>              | <span data-ttu-id="dfda8-p126">アイテムのサイズ (バイト単位)。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="dfda8-p126">Size of the item in bytes. Read-only.</span></span>
| <span data-ttu-id="dfda8-225">specialFolder</span><span class="sxs-lookup"><span data-stu-id="dfda8-225">specialFolder</span></span>        | <span data-ttu-id="dfda8-226">[specialFolder][]</span><span class="sxs-lookup"><span data-stu-id="dfda8-226">[specialFolder][]</span></span>  | <span data-ttu-id="dfda8-p127">現在のアイテムが特別なフォルダーとしても使用可能な場合は、このファセットが返されます。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="dfda8-p127">If the current item is also available as a special folder, this facet is returned. Read-only.</span></span>
| <span data-ttu-id="dfda8-229">video</span><span class="sxs-lookup"><span data-stu-id="dfda8-229">video</span></span>                | <span data-ttu-id="dfda8-230">[video][]</span><span class="sxs-lookup"><span data-stu-id="dfda8-230">[video][]</span></span>          | <span data-ttu-id="dfda8-p128">ビデオのメタデータ (アイテムがビデオである場合)。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="dfda8-p128">Video metadata, if the item is a video. Read-only.</span></span>
| <span data-ttu-id="dfda8-233">webDavUrl</span><span class="sxs-lookup"><span data-stu-id="dfda8-233">webDavUrl</span></span>            | <span data-ttu-id="dfda8-234">String</span><span class="sxs-lookup"><span data-stu-id="dfda8-234">String</span></span>             | <span data-ttu-id="dfda8-235">アイテムの WebDAV 互換性のある URL。</span><span class="sxs-lookup"><span data-stu-id="dfda8-235">WebDAV compatible URL for the item.</span></span>
| <span data-ttu-id="dfda8-236">webUrl</span><span class="sxs-lookup"><span data-stu-id="dfda8-236">webUrl</span></span>               | <span data-ttu-id="dfda8-237">String</span><span class="sxs-lookup"><span data-stu-id="dfda8-237">String</span></span>             | <span data-ttu-id="dfda8-p129">ブラウザーでリソースを表示するための URL。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="dfda8-p129">URL that displays the resource in the browser. Read-only.</span></span>

<span data-ttu-id="dfda8-p130">**注:**eTag プロパティと cTag プロパティは、コンテナー (フォルダー) 上での機能が異なります。cTag 値は、フォルダーのいずれかの子孫のコンテンツまたはメタデータが変更されると変更されます。eTag 値は、子孫から派生したプロパティ (**childCount** や **lastModifiedDateTime** など) 以外のフォルダーのプロパティが変更されたときにのみ、変更されます。</span><span class="sxs-lookup"><span data-stu-id="dfda8-p130">**Note:** The eTag and cTag properties work differently on containers (folders). The cTag value is modified when content or metadata of any descendant of the folder is changed. The eTag value is only modified when the folder's properties are changed, except for properties that are derived from descendants (like **childCount** or **lastModifiedDateTime**).</span></span>

## <a name="relationships"></a><span data-ttu-id="dfda8-243">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="dfda8-243">Relationships</span></span>

| <span data-ttu-id="dfda8-244">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="dfda8-244">Relationship</span></span>       | <span data-ttu-id="dfda8-245">型</span><span class="sxs-lookup"><span data-stu-id="dfda8-245">Type</span></span>                        | <span data-ttu-id="dfda8-246">説明</span><span class="sxs-lookup"><span data-stu-id="dfda8-246">Description</span></span>
|:-------------------|:----------------------------|:--------------------------
| <span data-ttu-id="dfda8-247">content</span><span class="sxs-lookup"><span data-stu-id="dfda8-247">content</span></span>            | <span data-ttu-id="dfda8-248">Stream</span><span class="sxs-lookup"><span data-stu-id="dfda8-248">Stream</span></span>                      | <span data-ttu-id="dfda8-249">コンテンツのストリーム (アイテムがファイルを表す場合)。</span><span class="sxs-lookup"><span data-stu-id="dfda8-249">The content stream, if the item represents a file.</span></span>
| <span data-ttu-id="dfda8-250">children</span><span class="sxs-lookup"><span data-stu-id="dfda8-250">children</span></span>           | <span data-ttu-id="dfda8-251">driveitem コレクション</span><span class="sxs-lookup"><span data-stu-id="dfda8-251">driveitem collection</span></span>        | <span data-ttu-id="dfda8-p131">アイテムの直接の子のアイテム オブジェクトを格納するコレクション。子が含まれるのは、フォルダーを表すアイテムのみです。読み取り専用です。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="dfda8-p131">Collection containing Item objects for the immediate children of Item. Only items representing folders have children. Read-only. Nullable.</span></span>
| <span data-ttu-id="dfda8-256">createdByUser</span><span class="sxs-lookup"><span data-stu-id="dfda8-256">createdByUser</span></span>      | <span data-ttu-id="dfda8-257">[user][]</span><span class="sxs-lookup"><span data-stu-id="dfda8-257">[user][]</span></span>                    | <span data-ttu-id="dfda8-258">アイテムを作成したユーザーの ID です。</span><span class="sxs-lookup"><span data-stu-id="dfda8-258">Identity of the user who created the item.</span></span> <span data-ttu-id="dfda8-259">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="dfda8-259">Read-only.</span></span>
| <span data-ttu-id="dfda8-260">lastModifiedByUser</span><span class="sxs-lookup"><span data-stu-id="dfda8-260">lastModifiedByUser</span></span> | <span data-ttu-id="dfda8-261">[user][]</span><span class="sxs-lookup"><span data-stu-id="dfda8-261">[user][]</span></span>                    | <span data-ttu-id="dfda8-262">アイテムを最後に変更したユーザーの ID です。</span><span class="sxs-lookup"><span data-stu-id="dfda8-262">Identity of the user, device, and application which last modified the item. Read-only.</span></span> <span data-ttu-id="dfda8-263">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="dfda8-263">Read-only.</span></span>
| <span data-ttu-id="dfda8-264">permissions</span><span class="sxs-lookup"><span data-stu-id="dfda8-264">permissions</span></span>        | <span data-ttu-id="dfda8-265">[permission][] コレクション</span><span class="sxs-lookup"><span data-stu-id="dfda8-265">[permission][] collection</span></span>   | <span data-ttu-id="dfda8-p134">アイテムのアクセス許可のセット。読み取り専用です。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="dfda8-p134">The set of permissions for the item. Read-only. Nullable.</span></span>
| <span data-ttu-id="dfda8-269">thumbnails</span><span class="sxs-lookup"><span data-stu-id="dfda8-269">thumbnails</span></span>         | <span data-ttu-id="dfda8-270">[thumbnailSet][] コレクション</span><span class="sxs-lookup"><span data-stu-id="dfda8-270">[thumbnailSet][] collection</span></span> | <span data-ttu-id="dfda8-p135">アイテムに関連付けられた [ThumbnailSet][] オブジェクトを格納するコレクション。詳細については、[サムネイルの取得][]についてのページをご覧ください。読み取り専用です。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="dfda8-p135">Collection containing [ThumbnailSet][] objects associated with the item. For more info, see [getting thumbnails][]. Read-only. Nullable.</span></span>

## <a name="instance-attributes"></a><span data-ttu-id="dfda8-275">インスタンスの属性</span><span class="sxs-lookup"><span data-stu-id="dfda8-275">Instance Attributes</span></span>

<span data-ttu-id="dfda8-p136">インスタンスの属性は、動作が特殊なプロパティです。これらのプロパティは一時的なものであり、a) サービスの動作を定義するか、b) 短期的なプロパティの値 (有効期限を持つアイテムのダウンロード URL など) を提供します。</span><span class="sxs-lookup"><span data-stu-id="dfda8-p136">Instance attributes are properties with special behaviors. These properties are temporary and either a) define behavior the service should perform or b) provide short-term property values, like a download URL for an item that expires.</span></span>

| <span data-ttu-id="dfda8-278">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="dfda8-278">Property name</span></span>                     | <span data-ttu-id="dfda8-279">種類</span><span class="sxs-lookup"><span data-stu-id="dfda8-279">Type</span></span>   | <span data-ttu-id="dfda8-280">説明</span><span class="sxs-lookup"><span data-stu-id="dfda8-280">Description</span></span>
|:----------------------------------|:-------|:--------------------------------
| <span data-ttu-id="dfda8-281">@microsoft.graph.conflictBehavior</span><span class="sxs-lookup"><span data-stu-id="dfda8-281">@microsoft.graph.conflictBehavior</span></span> | <span data-ttu-id="dfda8-282">string</span><span class="sxs-lookup"><span data-stu-id="dfda8-282">string</span></span> | <span data-ttu-id="dfda8-p137">新しいアイテムを作成するアクションの競合を解決する動作。*fail*、*replace*、*rename* という値を使用できます。PUT の既定値は *replace* です。この注釈とともにアイテムが返されることはありません。書き込み専用です。</span><span class="sxs-lookup"><span data-stu-id="dfda8-p137">The conflict resolution behavior for actions that create a new item. You can use the values *fail*, *replace*, or *rename*. The default for PUT is *replace*. An item will never be returned with this annotation. Write-only.</span></span>
| <span data-ttu-id="dfda8-288">@microsoft.graph.downloadUrl</span><span class="sxs-lookup"><span data-stu-id="dfda8-288">@microsoft.graph.downloadUrl</span></span>      | <span data-ttu-id="dfda8-289">string</span><span class="sxs-lookup"><span data-stu-id="dfda8-289">string</span></span> | <span data-ttu-id="dfda8-p138">このファイルのコンテンツをダウンロードするために使用できる URL。この URL では認証は必要ありません。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="dfda8-p138">A URL that can be used to download this file's content. Authentication is not required with this URL. Read-only.</span></span>
| <span data-ttu-id="dfda8-293">@microsoft.graph.sourceUrl</span><span class="sxs-lookup"><span data-stu-id="dfda8-293">@microsoft.graph.sourceUrl</span></span>        | <span data-ttu-id="dfda8-294">string</span><span class="sxs-lookup"><span data-stu-id="dfda8-294">string</span></span> | <span data-ttu-id="dfda8-p139">PUT 要求を発行するときにこのインスタンスの注釈を使用すると、サービスに対し、URL のコンテンツをダウンロードし、それをファイルとして保存するように指示できます。書き込み専用です。</span><span class="sxs-lookup"><span data-stu-id="dfda8-p139">When issuing a PUT request, this instance annotation can be used to instruct the service to download the contents of the URL, and store it as the file. Write-only.</span></span>

<span data-ttu-id="dfda8-p140">**注:**@microsoft.graph.downloadUrl の値は短時間限定の URL であるため、キャッシュすることはできません。URL は短い期間 (1 時間) だけ使用でき、その後は無効になります。</span><span class="sxs-lookup"><span data-stu-id="dfda8-p140">**Note:** The @microsoft.graph.downloadUrl value is a short-lived URL and can't be cached. The URL will only be available for a short period of time (1 hour) before it is invalidated.</span></span>

## <a name="methods"></a><span data-ttu-id="dfda8-299">メソッド</span><span class="sxs-lookup"><span data-stu-id="dfda8-299">Methods</span></span>

| <span data-ttu-id="dfda8-300">Method</span><span class="sxs-lookup"><span data-stu-id="dfda8-300">Method</span></span>                                                   | <span data-ttu-id="dfda8-301">REST パス</span><span class="sxs-lookup"><span data-stu-id="dfda8-301">REST Path</span></span>
|:---------------------------------------------------------|:------------------
| [<span data-ttu-id="dfda8-302">アイテムを取得する</span><span class="sxs-lookup"><span data-stu-id="dfda8-302">Get item</span></span>](../api/driveitem_get.md)                      | `GET /drive/items/{item-id}`
| [<span data-ttu-id="dfda8-303">子を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="dfda8-303">List children</span></span>](../api/driveitem_list_children.md)       | `GET /drive/items/{item-id}/children`
| [<span data-ttu-id="dfda8-304">アイテムを作成する</span><span class="sxs-lookup"><span data-stu-id="dfda8-304">Create item</span></span>](../api/driveitem_post_children.md)         | `POST /drive/items/{item-id}/children`
| [<span data-ttu-id="dfda8-305">アイテムを更新する</span><span class="sxs-lookup"><span data-stu-id="dfda8-305">Update item</span></span>](../api/driveitem_update.md)                | `PATCH /drive/items/{item-id}`
| [<span data-ttu-id="dfda8-306">コンテンツをアップロードする</span><span class="sxs-lookup"><span data-stu-id="dfda8-306">Upload content</span></span>](../api/driveitem_put_content.md)        | `PUT /drive/items/{item-id}/content`
| [<span data-ttu-id="dfda8-307">コンテンツをダウンロードする</span><span class="sxs-lookup"><span data-stu-id="dfda8-307">Download content</span></span>](../api/driveitem_get_content.md)      | `GET /drive/items/{item-id}/content`
| <span data-ttu-id="dfda8-308">[特定のファイル形式をダウンロードする][download-format]</span><span class="sxs-lookup"><span data-stu-id="dfda8-308">[Download specific file format][download-format]</span></span>         | `GET /drive/items/{item-id}/content?format={format}`
| [<span data-ttu-id="dfda8-309">アイテムを削除する</span><span class="sxs-lookup"><span data-stu-id="dfda8-309">Delete item</span></span>](../api/driveitem_delete.md)                | `DELETE /drive/items/{item-id}`
| [<span data-ttu-id="dfda8-310">アイテムを移動する</span><span class="sxs-lookup"><span data-stu-id="dfda8-310">Move item</span></span>](../api/driveitem_move.md)                    | `PATCH /drive/items/{item-id}`
| [<span data-ttu-id="dfda8-311">アイテムをコピーする</span><span class="sxs-lookup"><span data-stu-id="dfda8-311">Copy item</span></span>](../api/driveitem_copy.md)                    | `POST /drive/items/{item-id}/copy`
| [<span data-ttu-id="dfda8-312">アイテムを検索する</span><span class="sxs-lookup"><span data-stu-id="dfda8-312">Search items</span></span>](../api/driveitem_search.md)               | `GET /drive/items/{item-id}/search(q='text')`
| [<span data-ttu-id="dfda8-313">ドライブ内の変更内容を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="dfda8-313">List changes in a drive</span></span>](../api/driveitem_delta.md)     | `GET /drive/root/delta`
| [<span data-ttu-id="dfda8-314">サムネイルを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="dfda8-314">List thumbnails</span></span>](../api/driveitem_list_thumbnails.md)   | `GET /drive/items/{item-id}/thumbnails`
| [<span data-ttu-id="dfda8-315">共有リンクを作成する</span><span class="sxs-lookup"><span data-stu-id="dfda8-315">Create sharing link</span></span>](../api/driveitem_createlink.md)    | `POST /drive/items/{item-id}/createLink`
| [<span data-ttu-id="dfda8-316">アクセス許可を追加する</span><span class="sxs-lookup"><span data-stu-id="dfda8-316">Add permissions</span></span>](../api/driveitem_invite.md)            | `POST /drive/items/{item-id}/invite`
| [<span data-ttu-id="dfda8-317">アクセス許可を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="dfda8-317">List permissions</span></span>](../api/driveitem_list_permissions.md) | `GET /drive/items/{item-id}/permissions`
| [<span data-ttu-id="dfda8-318">アクセス許可を削除する</span><span class="sxs-lookup"><span data-stu-id="dfda8-318">Delete permission</span></span>](../api/permission_delete.md)         | `DELETE /drive/items/{item-id}/permissions/{perm-id}`


## <a name="remarks"></a><span data-ttu-id="dfda8-319">備考</span><span class="sxs-lookup"><span data-stu-id="dfda8-319">Remarks</span></span>

<span data-ttu-id="dfda8-320">OneDrive for Business または SharePoint のドキュメント ライブラリでは、**driveItem** に[フォルダー][] ファセットがある場合、**cTag** プロパティは返されません。</span><span class="sxs-lookup"><span data-stu-id="dfda8-320">In OneDrive for Business or SharePoint document libraries, the **cTag** property is not returned, if the **driveItem** has a [folder][] facet.</span></span>

[audio]: audio.md
[baseItem]: baseItem.md
[deleted]: deleted.md
[download-format]: ../api/driveitem_get_content_format.md
[file]: file.md
[fileSystemInfo]: fileSystemInfo.md
[folder]: folder.md
[getting thumbnails]: ../api/driveitem_list_thumbnails.md
[identitySet]: identitySet.md
[image]: image.md
[itemReference]: itemReference.md
[geoCoordinates]: geoCoordinates.md
[package]: package.md
[permission]: permission.md
[photo]: photo.md
[remoteItem]: remoteItem.md
[root]: root.md
[searchResult]: searchResult.md
[shared]: shared.md
[sharepointIds]: sharepointIds.md
[specialFolder]: specialFolder.md
[thumbnailSet]: thumbnailSet.md
[video]: video.md
[user]: https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/users

<!-- {
  "type": "#page.annotation",
  "description": "Item is the main data model in the OneDrive API. Everything is an item.",
  "keywords": "item,facet,resource",
  "section": "documentation",
  "tocPath": "Items",
  "tocBookmarks": { "Resources/Item": "#" }
} -->
