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
# <a name="driveitem-resource-type"></a><span data-ttu-id="4883a-102">DriveItem リソース型</span><span class="sxs-lookup"><span data-stu-id="4883a-102">DriveItem resource type</span></span>

<span data-ttu-id="4883a-p101">**driveItem** リソースは、ドライブに格納されているファイル、フォルダーなどのアイテムを表します。OneDrive および SharePoint 内のすべてのファイル システム オブジェクトが、**driveItem** リソースとして返されます。</span><span class="sxs-lookup"><span data-stu-id="4883a-p101">The **driveItem** resource represents a file, folder, or other item stored in a drive. All file system objects in OneDrive and SharePoint are returned as **driveItem** resources.</span></span>

<span data-ttu-id="4883a-105">**driveItem** リソースのアドレス指定には、主に 2 つの方法があります。</span><span class="sxs-lookup"><span data-stu-id="4883a-105">There are two primary ways of addressing a **driveItem** resource:</span></span>

* <span data-ttu-id="4883a-106">を使用した、**driveItem** 一意識別子による方法 `drive/items/{item-id}`</span><span class="sxs-lookup"><span data-stu-id="4883a-106">By the **driveItem** unique identifier using `drive/items/{item-id}`</span></span>
* <span data-ttu-id="4883a-107">を使用した、ファイル システム パスによる方法 `/drive/root:/path/to/file`</span><span class="sxs-lookup"><span data-stu-id="4883a-107">By file system path using `/drive/root:/path/to/file`</span></span>

<span data-ttu-id="4883a-p102">**DriveItem** リソースには、driveItem の ID および機能に関するデータを提供するプロパティとしてモデル化されたファセットがあります。例:</span><span class="sxs-lookup"><span data-stu-id="4883a-p102">**DriveItem** resources have facets modeled as properties that provide data about the driveItem's identities and capabilities. For example:</span></span>

* <span data-ttu-id="4883a-110">フォルダーには、[**フォルダー ファセット **][folder] があります</span><span class="sxs-lookup"><span data-stu-id="4883a-110">Folders have a [**folder facet**][folder]</span></span>
* <span data-ttu-id="4883a-111">ファイルには、[**ファイル ファセット **][file] があります。</span><span class="sxs-lookup"><span data-stu-id="4883a-111">Files have a [**file facet**][file].</span></span>
* <span data-ttu-id="4883a-112">画像には[**画像ファセット **][image] とそのファイル ファセットがあります。</span><span class="sxs-lookup"><span data-stu-id="4883a-112">Images have an [**image facet**][image] in addition to their file facet.</span></span>
* <span data-ttu-id="4883a-113">カメラで撮影した画像 (写真) には[**写真ファセット **][photo] があります。写真ファセットは、アイテムを写真として識別し、撮影日時と撮影デバイスのプロパティを提供します。</span><span class="sxs-lookup"><span data-stu-id="4883a-113">Images taken with a camera (photos) have a [**photo facet**][photo] that identifies the item as a photo and provides the properties of when the photo was taken and with what device.</span></span>

<span data-ttu-id="4883a-114">**フォルダー** ファセットを持つアイテムは、アイテムのコンテナーとして機能するため、フォルダーに含まれる **driveItems** のコレクションを指す `children` 参照を持ちます。</span><span class="sxs-lookup"><span data-stu-id="4883a-114">Items with the **folder** facet act as containers of items and therefore have a `children` reference pointing to a collection of **driveItems** under the folder.</span></span>

## <a name="json-representation"></a><span data-ttu-id="4883a-115">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="4883a-115">JSON representation</span></span>

<span data-ttu-id="4883a-116">以下は、**driveItem** リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="4883a-116">Here is a JSON representation of a **driveItem** resource.</span></span>

<span data-ttu-id="4883a-117">**driveItem** リソースは [**baseItem**][baseItem] から派生し、そのリソースからプロパティを継承します。</span><span class="sxs-lookup"><span data-stu-id="4883a-117">The **driveItem** resource is derived from [**baseItem**][baseItem] and inherits properties from that resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="4883a-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4883a-118">Properties</span></span>

| <span data-ttu-id="4883a-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4883a-119">Property</span></span>             | <span data-ttu-id="4883a-120">タイプ</span><span class="sxs-lookup"><span data-stu-id="4883a-120">Type</span></span>               | <span data-ttu-id="4883a-121">説明</span><span class="sxs-lookup"><span data-stu-id="4883a-121">Description</span></span>
|:---------------------|:-------------------|:---------------------------------
| <span data-ttu-id="4883a-122">オーディオ</span><span class="sxs-lookup"><span data-stu-id="4883a-122">audio</span></span>                | <span data-ttu-id="4883a-123">[オーディオ][]</span><span class="sxs-lookup"><span data-stu-id="4883a-123">[audio][]</span></span>          | <span data-ttu-id="4883a-p103">オーディオのメタデータ (アイテムがオーディオ ファイルである場合)。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="4883a-p103">Audio metadata, if the item is an audio file. Read-only.</span></span>
| <span data-ttu-id="4883a-126">コンテンツ</span><span class="sxs-lookup"><span data-stu-id="4883a-126">content</span></span>              | <span data-ttu-id="4883a-127">ストリーム</span><span class="sxs-lookup"><span data-stu-id="4883a-127">Stream</span></span>             | <span data-ttu-id="4883a-128">コンテンツのストリーム (アイテムがファイルを表す場合)。</span><span class="sxs-lookup"><span data-stu-id="4883a-128">The content stream, if the item represents a file.</span></span>
| <span data-ttu-id="4883a-129">createdBy</span><span class="sxs-lookup"><span data-stu-id="4883a-129">createdBy</span></span>            | <span data-ttu-id="4883a-130">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="4883a-130">[identitySet][]</span></span>    | <span data-ttu-id="4883a-p104">そのアイテムを作成したユーザーの ID、デバイス、アプリケーション。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="4883a-p104">Identity of the user, device, and application which created the item. Read-only.</span></span>
| <span data-ttu-id="4883a-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4883a-133">createdDateTime</span></span>      | <span data-ttu-id="4883a-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4883a-134">DateTimeOffset</span></span>     | <span data-ttu-id="4883a-p105">アイテム作成の日時。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="4883a-p105">Date and time of item creation. Read-only.</span></span>
| <span data-ttu-id="4883a-137">cTag</span><span class="sxs-lookup"><span data-stu-id="4883a-137">cTag</span></span>                 | <span data-ttu-id="4883a-138">文字列</span><span class="sxs-lookup"><span data-stu-id="4883a-138">String</span></span>             | <span data-ttu-id="4883a-p106">アイテムのコンテンツの eTag。メタデータのみが変更された場合、この eTag は変更されません。**注:** アイテムがフォルダーである場合、このプロパティは返されません。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="4883a-p106">An eTag for the content of the item. This eTag is not changed if only the metadata is changed. **Note** This property is not returned if the item is a folder. Read-only.</span></span>
| <span data-ttu-id="4883a-143">削除済み</span><span class="sxs-lookup"><span data-stu-id="4883a-143">deleted</span></span>              | <span data-ttu-id="4883a-144">[削除済み][]</span><span class="sxs-lookup"><span data-stu-id="4883a-144">[deleted][]</span></span>        | <span data-ttu-id="4883a-p107">アイテムの削除状態に関する情報。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="4883a-p107">Information about the deleted state of the item. Read-only.</span></span>
| <span data-ttu-id="4883a-147">説明</span><span class="sxs-lookup"><span data-stu-id="4883a-147">description</span></span>          | <span data-ttu-id="4883a-148">文字列</span><span class="sxs-lookup"><span data-stu-id="4883a-148">String</span></span>             | <span data-ttu-id="4883a-p108">ユーザーに表示されるアイテムの説明を提供します。読み取り/書き込み。OneDrive 個人用においてのみ</span><span class="sxs-lookup"><span data-stu-id="4883a-p108">Provides a user-visible description of the item. Read-write. Only on OneDrive Personal</span></span>
| <span data-ttu-id="4883a-152">eTag</span><span class="sxs-lookup"><span data-stu-id="4883a-152">eTag</span></span>                 | <span data-ttu-id="4883a-153">文字列</span><span class="sxs-lookup"><span data-stu-id="4883a-153">String</span></span>             | <span data-ttu-id="4883a-p109">アイテム全体 (メタデータおよびコンテンツ) の eTag。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="4883a-p109">eTag for the entire item (metadata + content). Read-only.</span></span>
| <span data-ttu-id="4883a-156">ファイル</span><span class="sxs-lookup"><span data-stu-id="4883a-156">file</span></span>                 | <span data-ttu-id="4883a-157">[ファイル][]</span><span class="sxs-lookup"><span data-stu-id="4883a-157">[file][]</span></span>           | <span data-ttu-id="4883a-p110">ファイルのメタデータ (アイテムがファイルである場合)。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="4883a-p110">File metadata, if the item is a file. Read-only.</span></span>
| <span data-ttu-id="4883a-160">fileSystemInfo</span><span class="sxs-lookup"><span data-stu-id="4883a-160">fileSystemInfo</span></span>       | <span data-ttu-id="4883a-161">[fileSystemInfo][]</span><span class="sxs-lookup"><span data-stu-id="4883a-161">[fileSystemInfo][]</span></span> | <span data-ttu-id="4883a-p111">クライアント上のファイル システム情報。読み取り/書き込み。</span><span class="sxs-lookup"><span data-stu-id="4883a-p111">File system information on client. Read-write.</span></span>
| <span data-ttu-id="4883a-164">フォルダー</span><span class="sxs-lookup"><span data-stu-id="4883a-164">folder</span></span>               | <span data-ttu-id="4883a-165">[フォルダー][]</span><span class="sxs-lookup"><span data-stu-id="4883a-165">[folder][]</span></span>         | <span data-ttu-id="4883a-p112">フォルダーのメタデータ (アイテムがフォルダーである場合)。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="4883a-p112">Folder metadata, if the item is a folder. Read-only.</span></span>
| <span data-ttu-id="4883a-168">ID</span><span class="sxs-lookup"><span data-stu-id="4883a-168">id</span></span>                   | <span data-ttu-id="4883a-169">文字列</span><span class="sxs-lookup"><span data-stu-id="4883a-169">String</span></span>             | <span data-ttu-id="4883a-p113">ドライブ内のアイテムの一意識別子。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="4883a-p113">The unique identifier of the item within the Drive. Read-only.</span></span>
| <span data-ttu-id="4883a-172">イメージ</span><span class="sxs-lookup"><span data-stu-id="4883a-172">image</span></span>                | <span data-ttu-id="4883a-173">[イメージ][]</span><span class="sxs-lookup"><span data-stu-id="4883a-173">[image][]</span></span>          | <span data-ttu-id="4883a-p114">画像のメタデータ (アイテムが画像である場合)。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="4883a-p114">Image metadata, if the item is an image. Read-only.</span></span>
| <span data-ttu-id="4883a-176">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="4883a-176">lastModifiedBy</span></span>       | <span data-ttu-id="4883a-177">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="4883a-177">[identitySet][]</span></span>    | <span data-ttu-id="4883a-p115">アイテムを最終更新したユーザーの ID、デバイス、アプリケーション。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="4883a-p115">Identity of the user, device, and application which last modified the item. Read-only.</span></span>
| <span data-ttu-id="4883a-180">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4883a-180">lastModifiedDateTime</span></span> | <span data-ttu-id="4883a-181">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4883a-181">DateTimeOffset</span></span>     | <span data-ttu-id="4883a-p116">アイテムが最後に変更された日時。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="4883a-p116">Date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="4883a-184">場所</span><span class="sxs-lookup"><span data-stu-id="4883a-184">location</span></span>             | <span data-ttu-id="4883a-185">[geoCoordinates][]</span><span class="sxs-lookup"><span data-stu-id="4883a-185">[geoCoordinates][]</span></span> | <span data-ttu-id="4883a-p117">場所のメタデータ (アイテムに場所データが含まれている場合)。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="4883a-p117">Location metadata, if the item has location data. Read-only.</span></span>
| <span data-ttu-id="4883a-188">名前</span><span class="sxs-lookup"><span data-stu-id="4883a-188">name</span></span>                 | <span data-ttu-id="4883a-189">文字列</span><span class="sxs-lookup"><span data-stu-id="4883a-189">String</span></span>             | <span data-ttu-id="4883a-p118">アイテムの名前 (ファイル名と拡張子)。読み取り/書き込み。</span><span class="sxs-lookup"><span data-stu-id="4883a-p118">The name of the item (filename and extension). Read-write.</span></span>
| <span data-ttu-id="4883a-192">パッケージ</span><span class="sxs-lookup"><span data-stu-id="4883a-192">package</span></span>              | <span data-ttu-id="4883a-193">[パッケージ][]</span><span class="sxs-lookup"><span data-stu-id="4883a-193">[package][]</span></span>        | <span data-ttu-id="4883a-p119">これがある場合、アイテムはフォルダーやファイルではなく、パッケージです。パッケージは、コンテキスト次第で、ファイルとして、あるいはフォルダーとして扱われます。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="4883a-p119">If present, indicates that this item is a package instead of a folder or file. Packages are treated like files in some contexts and folders in others. Read-only.</span></span>
| <span data-ttu-id="4883a-197">parentReference</span><span class="sxs-lookup"><span data-stu-id="4883a-197">parentReference</span></span>      | <span data-ttu-id="4883a-198">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="4883a-198">[itemReference][]</span></span>  | <span data-ttu-id="4883a-p120">親の情報 (アイテムに親がある場合)。読み取り/書き込み。</span><span class="sxs-lookup"><span data-stu-id="4883a-p120">Parent information, if the item has a parent. Read-write.</span></span>
| <span data-ttu-id="4883a-201">写真</span><span class="sxs-lookup"><span data-stu-id="4883a-201">photo</span></span>                | <span data-ttu-id="4883a-202">[写真][]</span><span class="sxs-lookup"><span data-stu-id="4883a-202">[photo][]</span></span>          | <span data-ttu-id="4883a-p121">写真のメタデータ (アイテムが写真である場合)。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="4883a-p121">Photo metadata, if the item is a photo. Read-only.</span></span>
| <span data-ttu-id="4883a-205">パブリケーション</span><span class="sxs-lookup"><span data-stu-id="4883a-205">publication</span></span>          | <span data-ttu-id="4883a-206">[publicationFacet][]</span><span class="sxs-lookup"><span data-stu-id="4883a-206">[publicationFacet][]</span></span> | <span data-ttu-id="4883a-207">アイテムが公開されているか、チェックアウトの状態かどうかの情報を、そのような操作をサポートする場所で提供します。</span><span class="sxs-lookup"><span data-stu-id="4883a-207">Provides information about the published or checked-out state of an item, in locations that support such actions.</span></span> <span data-ttu-id="4883a-208">既定では、このプロパティは返されません。</span><span class="sxs-lookup"><span data-stu-id="4883a-208">This property is not returned by default.</span></span> <span data-ttu-id="4883a-209">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="4883a-209">Read-only.</span></span> |
| <span data-ttu-id="4883a-210">remoteItem</span><span class="sxs-lookup"><span data-stu-id="4883a-210">remoteItem</span></span>           | <span data-ttu-id="4883a-211">[remoteItem][]</span><span class="sxs-lookup"><span data-stu-id="4883a-211">[remoteItem][]</span></span>     | <span data-ttu-id="4883a-p123">リモート アイテムのデータ (現在アクセス中のドライブ以外のドライブから共有されているアイテムの場合)。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="4883a-p123">Remote item data, if the item is shared from a drive other than the one being accessed. Read-only.</span></span>
| <span data-ttu-id="4883a-214">ルート</span><span class="sxs-lookup"><span data-stu-id="4883a-214">root</span></span>                 | <span data-ttu-id="4883a-215">[ルート][]</span><span class="sxs-lookup"><span data-stu-id="4883a-215">[root][]</span></span>           | <span data-ttu-id="4883a-216">このプロパティが null ではない場合は、driveItem がドライブで最上位の driveItem であることを示します。</span><span class="sxs-lookup"><span data-stu-id="4883a-216">If this property is non-null, it indicates that the driveItem is the top-most driveItem in the drive.</span></span>
| <span data-ttu-id="4883a-217">searchResult</span><span class="sxs-lookup"><span data-stu-id="4883a-217">searchResult</span></span>         | <span data-ttu-id="4883a-218">[searchResult][]</span><span class="sxs-lookup"><span data-stu-id="4883a-218">[searchResult][]</span></span>   | <span data-ttu-id="4883a-p124">検索のメタデータ (検索結果に由来するアイテムの場合)。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="4883a-p124">Search metadata, if the item is from a search result. Read-only.</span></span>
| <span data-ttu-id="4883a-221">共有済み</span><span class="sxs-lookup"><span data-stu-id="4883a-221">shared</span></span>               | <span data-ttu-id="4883a-222">[共有済み][]</span><span class="sxs-lookup"><span data-stu-id="4883a-222">[shared][]</span></span>         | <span data-ttu-id="4883a-p125">アイテムが他のユーザーと共有されていることを示し、アイテムの共有状態に関する情報を提供します。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="4883a-p125">Indicates that the item has been shared with others and provides information about the shared state of the item. Read-only.</span></span>
| <span data-ttu-id="4883a-225">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="4883a-225">sharepointIds</span></span>        | <span data-ttu-id="4883a-226">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="4883a-226">[sharepointIds][]</span></span>  | <span data-ttu-id="4883a-p126">SharePoint REST 互換性に役立つ識別子を返します。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="4883a-p126">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>
| <span data-ttu-id="4883a-229">サイズ</span><span class="sxs-lookup"><span data-stu-id="4883a-229">size</span></span>                 | <span data-ttu-id="4883a-230">Int64</span><span class="sxs-lookup"><span data-stu-id="4883a-230">Int64</span></span>              | <span data-ttu-id="4883a-p127">アイテムのサイズ (バイト単位)。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="4883a-p127">Size of the item in bytes. Read-only.</span></span>
| <span data-ttu-id="4883a-233">specialFolder</span><span class="sxs-lookup"><span data-stu-id="4883a-233">specialFolder</span></span>        | <span data-ttu-id="4883a-234">[specialFolder][]</span><span class="sxs-lookup"><span data-stu-id="4883a-234">[specialFolder][]</span></span>  | <span data-ttu-id="4883a-p128">現在のアイテムが特別なフォルダーとしても使用可能な場合は、このファセットが返されます。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="4883a-p128">If the current item is also available as a special folder, this facet is returned. Read-only.</span></span>
| <span data-ttu-id="4883a-237">ビデオ</span><span class="sxs-lookup"><span data-stu-id="4883a-237">video</span></span>                | <span data-ttu-id="4883a-238">[ビデオ][]</span><span class="sxs-lookup"><span data-stu-id="4883a-238">[video][]</span></span>          | <span data-ttu-id="4883a-p129">ビデオのメタデータ (アイテムがビデオである場合)。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="4883a-p129">Video metadata, if the item is a video. Read-only.</span></span>
| <span data-ttu-id="4883a-241">webDavUrl</span><span class="sxs-lookup"><span data-stu-id="4883a-241">webDavUrl</span></span>            | <span data-ttu-id="4883a-242">文字列</span><span class="sxs-lookup"><span data-stu-id="4883a-242">String</span></span>             | <span data-ttu-id="4883a-243">アイテムの WebDAV 互換性のある URL。</span><span class="sxs-lookup"><span data-stu-id="4883a-243">WebDAV compatible URL for the item.</span></span>
| <span data-ttu-id="4883a-244">webUrl</span><span class="sxs-lookup"><span data-stu-id="4883a-244">webUrl</span></span>               | <span data-ttu-id="4883a-245">文字列</span><span class="sxs-lookup"><span data-stu-id="4883a-245">String</span></span>             | <span data-ttu-id="4883a-p130">ブラウザーでリソースを表示するための URL。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="4883a-p130">URL that displays the resource in the browser. Read-only.</span></span>

<span data-ttu-id="4883a-p131">**注:** eTag プロパティと cTag プロパティは、コンテナー (フォルダー) 上での機能が異なります。cTag 値は、フォルダーのいずれかの子孫のコンテンツまたはメタデータが変更されると変更されます。eTag 値は、子孫から派生したプロパティ (**childCount** や **lastModifiedDateTime** など) 以外のフォルダーのプロパティが変更されたときにのみ、変更されます。</span><span class="sxs-lookup"><span data-stu-id="4883a-p131">**Note:** The eTag and cTag properties work differently on containers (folders). The cTag value is modified when content or metadata of any descendant of the folder is changed. The eTag value is only modified when the folder's properties are changed, except for properties that are derived from descendants (like **childCount** or **lastModifiedDateTime**).</span></span>

## <a name="relationships"></a><span data-ttu-id="4883a-251">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="4883a-251">Relationships</span></span>

| <span data-ttu-id="4883a-252">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="4883a-252">Relationship</span></span>       | <span data-ttu-id="4883a-253">型</span><span class="sxs-lookup"><span data-stu-id="4883a-253">Type</span></span>                        | <span data-ttu-id="4883a-254">説明</span><span class="sxs-lookup"><span data-stu-id="4883a-254">Description</span></span>
|:-------------------|:----------------------------|:--------------------------
| <span data-ttu-id="4883a-255">子</span><span class="sxs-lookup"><span data-stu-id="4883a-255">children</span></span>           | <span data-ttu-id="4883a-256">driveitem コレクション</span><span class="sxs-lookup"><span data-stu-id="4883a-256">driveitem collection</span></span>        | <span data-ttu-id="4883a-p132">アイテムの直接の子のアイテム オブジェクトを格納するコレクション。子が含まれるのは、フォルダーを表すアイテムのみです。読み取り専用です。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="4883a-p132">Collection containing Item objects for the immediate children of Item. Only items representing folders have children. Read-only. Nullable.</span></span>
| <span data-ttu-id="4883a-261">createdByUser</span><span class="sxs-lookup"><span data-stu-id="4883a-261">createdByUser</span></span>      | <span data-ttu-id="4883a-262">[ユーザー][]</span><span class="sxs-lookup"><span data-stu-id="4883a-262">[user][]</span></span>                    | <span data-ttu-id="4883a-263">アイテムを作成したユーザーの ID です。</span><span class="sxs-lookup"><span data-stu-id="4883a-263">Identity of the user who created the item.</span></span> <span data-ttu-id="4883a-264">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="4883a-264">Read-only.</span></span>
| <span data-ttu-id="4883a-265">lastModifiedByUser</span><span class="sxs-lookup"><span data-stu-id="4883a-265">lastModifiedByUser</span></span> | <span data-ttu-id="4883a-266">[ユーザー][]</span><span class="sxs-lookup"><span data-stu-id="4883a-266">[user][]</span></span>                    | <span data-ttu-id="4883a-267">アイテムを最後に変更したユーザーの ID です。</span><span class="sxs-lookup"><span data-stu-id="4883a-267">Identity of the user who last modified the item.</span></span> <span data-ttu-id="4883a-268">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="4883a-268">Read-only.</span></span>
| <span data-ttu-id="4883a-269">listItem</span><span class="sxs-lookup"><span data-stu-id="4883a-269">listItem</span></span>           | <span data-ttu-id="4883a-270">[listItem][]</span><span class="sxs-lookup"><span data-stu-id="4883a-270">[listItem][]</span></span>                | <span data-ttu-id="4883a-271">SharePoint のドライブ用の、関連付けられたドキュメント ライブラリのリスト アイテムです。</span><span class="sxs-lookup"><span data-stu-id="4883a-271">For drives in SharePoint, the associated document library list item.</span></span> <span data-ttu-id="4883a-272">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="4883a-272">Read-only.</span></span> <span data-ttu-id="4883a-273">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="4883a-273">Nullable.</span></span>
| <span data-ttu-id="4883a-274">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="4883a-274">permissions</span></span>        | <span data-ttu-id="4883a-275">[permission][] コレクション</span><span class="sxs-lookup"><span data-stu-id="4883a-275">[permission][] collection</span></span>   | <span data-ttu-id="4883a-p136">アイテムのアクセス許可のセット。読み取り専用です。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="4883a-p136">The set of permissions for the item. Read-only. Nullable.</span></span>
| <span data-ttu-id="4883a-279">サムネイル</span><span class="sxs-lookup"><span data-stu-id="4883a-279">thumbnails</span></span>         | <span data-ttu-id="4883a-280">[thumbnailSet][] コレクション</span><span class="sxs-lookup"><span data-stu-id="4883a-280">[thumbnailSet][] collection</span></span> | <span data-ttu-id="4883a-p137">アイテムに関連付けられた [ThumbnailSet][] オブジェクトを格納するコレクション。詳細については、[サムネイルの取得][]についてのページをご覧ください。読み取り専用です。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="4883a-p137">Collection containing [ThumbnailSet][] objects associated with the item. For more info, see [getting thumbnails][]. Read-only. Nullable.</span></span>
| <span data-ttu-id="4883a-285">バージョン</span><span class="sxs-lookup"><span data-stu-id="4883a-285">versions</span></span>           | <span data-ttu-id="4883a-286">[driveItemVersion][] コレクション</span><span class="sxs-lookup"><span data-stu-id="4883a-286">[driveItemVersion][] collection</span></span> | <span data-ttu-id="4883a-287">項目の以前のバージョンの一覧です。</span><span class="sxs-lookup"><span data-stu-id="4883a-287">The list of previous versions of the item.</span></span> <span data-ttu-id="4883a-288">詳細については、「[以前のバージョンを取得する][]」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4883a-288">For more info, see [getting previous versions][].</span></span> <span data-ttu-id="4883a-289">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="4883a-289">Read-only.</span></span> <span data-ttu-id="4883a-290">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="4883a-290">Nullable.</span></span>
| <span data-ttu-id="4883a-291">ブック</span><span class="sxs-lookup"><span data-stu-id="4883a-291">workbook</span></span>           | <span data-ttu-id="4883a-292">[ブック][]</span><span class="sxs-lookup"><span data-stu-id="4883a-292">[workbook][]</span></span>                | <span data-ttu-id="4883a-293">ファイルが Excel のスプレッドシートである場合、スプレッドシートのコンテンツを扱うためにブック API にアクセスします。</span><span class="sxs-lookup"><span data-stu-id="4883a-293">For files that are Excel spreadsheets, accesses the workbook API to work with the spreadsheet's contents.</span></span> <span data-ttu-id="4883a-294">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="4883a-294">Nullable.</span></span>

## <a name="instance-attributes"></a><span data-ttu-id="4883a-295">インスタンスの属性</span><span class="sxs-lookup"><span data-stu-id="4883a-295">Instance Attributes</span></span>

<span data-ttu-id="4883a-p140">インスタンスの属性は、動作が特殊なプロパティです。これらのプロパティは一時的なものであり、a) サービスの動作を定義するか、b) 短期的なプロパティの値 (有効期限を持つアイテムのダウンロード URL など) を提供します。</span><span class="sxs-lookup"><span data-stu-id="4883a-p140">Instance attributes are properties with special behaviors. These properties are temporary and either a) define behavior the service should perform or b) provide short-term property values, like a download URL for an item that expires.</span></span>

| <span data-ttu-id="4883a-298">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="4883a-298">Property name</span></span>                     | <span data-ttu-id="4883a-299">型</span><span class="sxs-lookup"><span data-stu-id="4883a-299">Type</span></span>   | <span data-ttu-id="4883a-300">説明</span><span class="sxs-lookup"><span data-stu-id="4883a-300">Description</span></span>
|:----------------------------------|:-------|:--------------------------------
| <span data-ttu-id="4883a-301">@microsoft.graph.conflictBehavior</span><span class="sxs-lookup"><span data-stu-id="4883a-301">@microsoft.graph.conflictBehavior</span></span> | <span data-ttu-id="4883a-302">文字列</span><span class="sxs-lookup"><span data-stu-id="4883a-302">string</span></span> | <span data-ttu-id="4883a-p141">新しいアイテムを作成するアクションの競合を解決する動作。*fail*、*replace*、*rename* という値を使用できます。PUT の既定値は *replace* です。この注釈とともにアイテムが返されることはありません。書き込み専用です。</span><span class="sxs-lookup"><span data-stu-id="4883a-p141">The conflict resolution behavior for actions that create a new item. You can use the values *fail*, *replace*, or *rename*. The default for PUT is *replace*. An item will never be returned with this annotation. Write-only.</span></span>
| <span data-ttu-id="4883a-308">@microsoft.graph.downloadUrl</span><span class="sxs-lookup"><span data-stu-id="4883a-308">@microsoft.graph.downloadUrl</span></span>      | <span data-ttu-id="4883a-309">文字列</span><span class="sxs-lookup"><span data-stu-id="4883a-309">string</span></span> | <span data-ttu-id="4883a-p142">このファイルのコンテンツをダウンロードするために使用できる URL。この URL では認証は必要ありません。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="4883a-p142">A URL that can be used to download this file's content. Authentication is not required with this URL. Read-only.</span></span>
| <span data-ttu-id="4883a-313">@microsoft.graph.sourceUrl</span><span class="sxs-lookup"><span data-stu-id="4883a-313">@microsoft.graph.sourceUrl</span></span>        | <span data-ttu-id="4883a-314">文字列</span><span class="sxs-lookup"><span data-stu-id="4883a-314">string</span></span> | <span data-ttu-id="4883a-p143">PUT 要求を発行するときにこのインスタンスの注釈を使用すると、サービスに対し、URL のコンテンツをダウンロードし、それをファイルとして保存するように指示できます。書き込み専用です。</span><span class="sxs-lookup"><span data-stu-id="4883a-p143">When issuing a PUT request, this instance annotation can be used to instruct the service to download the contents of the URL, and store it as the file. Write-only.</span></span>

<span data-ttu-id="4883a-p144">**注:**@microsoft.graph.downloadUrl の値は短時間限定の URL であるため、キャッシュすることはできません。URL は短い期間 (1 時間) だけ使用でき、その後は無効になります。</span><span class="sxs-lookup"><span data-stu-id="4883a-p144">**Note:** The @microsoft.graph.downloadUrl value is a short-lived URL and can't be cached. The URL will only be available for a short period of time (1 hour) before it is invalidated.</span></span>

## <a name="methods"></a><span data-ttu-id="4883a-319">メソッド</span><span class="sxs-lookup"><span data-stu-id="4883a-319">Methods</span></span>

| <span data-ttu-id="4883a-320">メソッド</span><span class="sxs-lookup"><span data-stu-id="4883a-320">Method</span></span>                                                   | <span data-ttu-id="4883a-321">REST パス</span><span class="sxs-lookup"><span data-stu-id="4883a-321">REST Path</span></span>
|:---------------------------------------------------------|:------------------
| [<span data-ttu-id="4883a-322">アイテムを取得する</span><span class="sxs-lookup"><span data-stu-id="4883a-322">Get item</span></span>](../api/driveitem_get.md)                      | `GET /drive/items/{item-id}`
| [<span data-ttu-id="4883a-323">子を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="4883a-323">List children</span></span>](../api/driveitem_list_children.md)       | `GET /drive/items/{item-id}/children`
| [<span data-ttu-id="4883a-324">バージョンの一覧表示</span><span class="sxs-lookup"><span data-stu-id="4883a-324">List versions</span></span>](../api/driveitem_list_versions.md)       | `GET /drive/items/{item-id}/versions`
| [<span data-ttu-id="4883a-325">アイテムを作成する</span><span class="sxs-lookup"><span data-stu-id="4883a-325">Create item</span></span>](../api/driveitem_post_children.md)         | `POST /drive/items/{item-id}/children`
| [<span data-ttu-id="4883a-326">アイテムを更新する</span><span class="sxs-lookup"><span data-stu-id="4883a-326">Update item</span></span>](../api/driveitem_update.md)                | `PATCH /drive/items/{item-id}`
| [<span data-ttu-id="4883a-327">コンテンツをアップロードする</span><span class="sxs-lookup"><span data-stu-id="4883a-327">Upload content</span></span>](../api/driveitem_put_content.md)        | `PUT /drive/items/{item-id}/content`
| [<span data-ttu-id="4883a-328">コンテンツをダウンロードする</span><span class="sxs-lookup"><span data-stu-id="4883a-328">Download content</span></span>](../api/driveitem_get_content.md)      | `GET /drive/items/{item-id}/content`
| <span data-ttu-id="4883a-329">[特定のファイル形式をダウンロードする][download-format]</span><span class="sxs-lookup"><span data-stu-id="4883a-329">[Download specific file format][download-format]</span></span>         | `GET /drive/items/{item-id}/content?format={format}`
| [<span data-ttu-id="4883a-330">アイテムを削除する</span><span class="sxs-lookup"><span data-stu-id="4883a-330">Delete item</span></span>](../api/driveitem_delete.md)                | `DELETE /drive/items/{item-id}`
| [<span data-ttu-id="4883a-331">アイテムを移動する</span><span class="sxs-lookup"><span data-stu-id="4883a-331">Move item</span></span>](../api/driveitem_move.md)                    | `PATCH /drive/items/{item-id}`
| [<span data-ttu-id="4883a-332">アイテムをコピーする</span><span class="sxs-lookup"><span data-stu-id="4883a-332">Copy item</span></span>](../api/driveitem_copy.md)                    | `POST /drive/items/{item-id}/copy`
| [<span data-ttu-id="4883a-333">アイテムを検索する</span><span class="sxs-lookup"><span data-stu-id="4883a-333">Search items</span></span>](../api/driveitem_search.md)               | `GET /drive/items/{item-id}/search(q='text')`
| [<span data-ttu-id="4883a-334">ドライブ内の変更内容を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="4883a-334">List changes in a drive</span></span>](../api/driveitem_delta.md)     | `GET /drive/root/delta`
| [<span data-ttu-id="4883a-335">サムネイルを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="4883a-335">List thumbnails</span></span>](../api/driveitem_list_thumbnails.md)   | `GET /drive/items/{item-id}/thumbnails`
| [<span data-ttu-id="4883a-336">共有リンクを作成する</span><span class="sxs-lookup"><span data-stu-id="4883a-336">Create sharing link</span></span>](../api/driveitem_createlink.md)    | `POST /drive/items/{item-id}/createLink`
| [<span data-ttu-id="4883a-337">アクセス許可を追加する</span><span class="sxs-lookup"><span data-stu-id="4883a-337">Add permissions</span></span>](../api/driveitem_invite.md)            | `POST /drive/items/{item-id}/invite`
| [<span data-ttu-id="4883a-338">アクセス許可を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="4883a-338">List permissions</span></span>](../api/driveitem_list_permissions.md) | `GET /drive/items/{item-id}/permissions`
| [<span data-ttu-id="4883a-339">アクセス許可を削除する</span><span class="sxs-lookup"><span data-stu-id="4883a-339">Delete permission</span></span>](../api/permission_delete.md)         | `DELETE /drive/items/{item-id}/permissions/{perm-id}`


## <a name="remarks"></a><span data-ttu-id="4883a-340">備考</span><span class="sxs-lookup"><span data-stu-id="4883a-340">Remarks</span></span>

<span data-ttu-id="4883a-341">OneDrive for Business または SharePoint のドキュメント ライブラリでは、**driveItem** に[フォルダー][] ファセットがある場合、**cTag** プロパティは返されません。</span><span class="sxs-lookup"><span data-stu-id="4883a-341">In OneDrive for Business or SharePoint document libraries, the **cTag** property is not returned, if the **driveItem** has a [folder][] facet.</span></span>

[オーディオ]: audio.md
[audio]: audio.md
[baseItem]: baseItem.md
[削除済み]: deleted.md
[deleted]: deleted.md
[download-format]: ../api/driveitem_get_content_format.md
[driveItemVersion]: driveItemVersion.md
[ファイル]: file.md
[file]: file.md
[fileSystemInfo]: fileSystemInfo.md
[フォルダー]: folder.md
[folder]: folder.md
[以前のバージョンを取得する]: ../api/driveitem_list_versions.md
[getting previous versions]: ../api/driveitem_list_versions.md
[サムネイルの取得]: ../api/driveitem_list_thumbnails.md
[getting thumbnails]: ../api/driveitem_list_thumbnails.md
[identitySet]: identitySet.md
[イメージ]: image.md
[image]: image.md
[itemReference]: itemReference.md
[geoCoordinates]: geoCoordinates.md
[listItem]: listItem.md
[パッケージ]: package.md
[package]: package.md
[アクセス許可]: permission.md
[permission]: permission.md
[写真]: photo.md
[photo]: photo.md
[remoteItem]: remoteItem.md
[ルート]: root.md
[root]: root.md
[searchResult]: searchResult.md
[共有]: shared.md
[shared]: shared.md
[sharepointIds]: sharepointIds.md
[specialFolder]: specialFolder.md
[thumbnailSet]: thumbnailSet.md
[ビデオ]: video.md
[video]: video.md
[ブック]: workbook.md
[workbook]: workbook.md
[ユーザー]: https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/users
[user]: https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/users
[publicationFacet]: publicationfacet.md

<!-- {
  "type": "#page.annotation",
  "description": "Item is the main data model in the OneDrive API. Everything is an item.",
  "keywords": "item,facet,resource",
  "section": "documentation",
  "tocPath": "Items",
  "tocBookmarks": { "Resources/Item": "#" }
} -->
