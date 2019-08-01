---
author: JeremyKelley
ms.author: JeremyKelley
title: DriveItem リソース型
description: アイテムは、OneDrive API での主要なデータ モデルです。 すべてがアイテムです。
localization_priority: Priority
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: a098da44ea4d6861a7d4372c907452721bfc881b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36029373"
---
# <a name="driveitem-resource-type"></a><span data-ttu-id="b7690-104">driveItem リソース型</span><span class="sxs-lookup"><span data-stu-id="b7690-104">driveItem resource type</span></span>

<span data-ttu-id="b7690-p102">**driveItem** リソースは、ドライブに格納されているファイル、フォルダーなどのアイテムを表します。OneDrive および SharePoint 内のすべてのファイル システム オブジェクトが、**driveItem** リソースとして返されます。</span><span class="sxs-lookup"><span data-stu-id="b7690-p102">The **driveItem** resource represents a file, folder, or other item stored in a drive. All file system objects in OneDrive and SharePoint are returned as **driveItem** resources.</span></span>

<span data-ttu-id="b7690-107">**driveItem** リソースのアドレス指定には、主に 2 つの方法があります。</span><span class="sxs-lookup"><span data-stu-id="b7690-107">There are two primary ways of addressing a **driveItem** resource:</span></span>

* <span data-ttu-id="b7690-108">`drive/items/{item-id}` を使用した、**driveItem** 一意識別子による方法</span><span class="sxs-lookup"><span data-stu-id="b7690-108">By the **driveItem** unique identifier using `drive/items/{item-id}`</span></span>
* <span data-ttu-id="b7690-109">`/drive/root:/path/to/file` を使用した、ファイル システム パスによる方法</span><span class="sxs-lookup"><span data-stu-id="b7690-109">By file system path using `/drive/root:/path/to/file`</span></span>

<span data-ttu-id="b7690-110">**DriveItem** リソースには、driveItem の ID および機能に関するデータを提供するプロパティとしてモデル化されたファセットがあります。</span><span class="sxs-lookup"><span data-stu-id="b7690-110">**driveItem** resources have facets modeled as properties that provide data about the driveItem's identities and capabilities.</span></span>
<span data-ttu-id="b7690-111">次に例を示します。</span><span class="sxs-lookup"><span data-stu-id="b7690-111">For example:</span></span>

* <span data-ttu-id="b7690-112">フォルダーには、[\*\*フォルダー ファセット \*\*][folder] があります。</span><span class="sxs-lookup"><span data-stu-id="b7690-112">Folders have a [**folder facet**][folder]</span></span>
* <span data-ttu-id="b7690-113">ファイルには、[\*\*ファイル ファセット \*\*][file] があります。</span><span class="sxs-lookup"><span data-stu-id="b7690-113">Files have a [**file facet**][file].</span></span>
* <span data-ttu-id="b7690-114">画像には[\*\*画像ファセット \*\*][image] とそのファイル ファセットがあります。</span><span class="sxs-lookup"><span data-stu-id="b7690-114">Images have an [**image facet**][image] in addition to their file facet.</span></span>
* <span data-ttu-id="b7690-115">カメラで撮影した画像 (写真) には[\*\*写真ファセット \*\*][photo] があります。写真ファセットは、アイテムを写真として識別し、撮影日時と撮影デバイスのプロパティを提供します。</span><span class="sxs-lookup"><span data-stu-id="b7690-115">Images taken with a camera (photos) have a [**photo facet**][photo] that identifies the item as a photo and provides the properties of when the photo was taken and with what device.</span></span>

<span data-ttu-id="b7690-116">**フォルダー** ファセットを持つアイテムは、アイテムのコンテナーとして機能するため、フォルダーに含まれる **driveItems** のコレクションを指す `children` 参照を持ちます。</span><span class="sxs-lookup"><span data-stu-id="b7690-116">Items with the **folder** facet act as containers of items and therefore have a `children` reference pointing to a collection of **driveItems** under the folder.</span></span>

><span data-ttu-id="b7690-117">**注:** OneDrive for Business または SharePoint のドキュメント ライブラリでは、**driveItem** に[フォルダー][] ファセットがある場合、**cTag** プロパティは返されません。</span><span class="sxs-lookup"><span data-stu-id="b7690-117">**Note:** In OneDrive for Business or SharePoint document libraries, the **cTag** property is not returned, if the **driveItem** has a [folder][] facet.</span></span>

## <a name="properties"></a><span data-ttu-id="b7690-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b7690-118">Properties</span></span>

| <span data-ttu-id="b7690-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b7690-119">Property</span></span>             | <span data-ttu-id="b7690-120">型</span><span class="sxs-lookup"><span data-stu-id="b7690-120">Type</span></span>               | <span data-ttu-id="b7690-121">説明</span><span class="sxs-lookup"><span data-stu-id="b7690-121">Description</span></span>
|:---------------------|:-------------------|:---------------------------------
| <span data-ttu-id="b7690-122">audio</span><span class="sxs-lookup"><span data-stu-id="b7690-122">audio</span></span>                | <span data-ttu-id="b7690-123">[audio][]</span><span class="sxs-lookup"><span data-stu-id="b7690-123">[audio][]</span></span>          | <span data-ttu-id="b7690-p104">オーディオのメタデータ (アイテムがオーディオ ファイルである場合)。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="b7690-p104">Audio metadata, if the item is an audio file. Read-only.</span></span>
| <span data-ttu-id="b7690-126">content</span><span class="sxs-lookup"><span data-stu-id="b7690-126">content</span></span>              | <span data-ttu-id="b7690-127">Stream</span><span class="sxs-lookup"><span data-stu-id="b7690-127">Stream</span></span>             | <span data-ttu-id="b7690-128">コンテンツのストリーム (アイテムがファイルを表す場合)。</span><span class="sxs-lookup"><span data-stu-id="b7690-128">The content stream, if the item represents a file.</span></span>
| <span data-ttu-id="b7690-129">createdBy</span><span class="sxs-lookup"><span data-stu-id="b7690-129">createdBy</span></span>            | <span data-ttu-id="b7690-130">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="b7690-130">[identitySet][]</span></span>    | <span data-ttu-id="b7690-p105">そのアイテムを作成したユーザーの ID、デバイス、アプリケーション。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="b7690-p105">Identity of the user, device, and application which created the item. Read-only.</span></span>
| <span data-ttu-id="b7690-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b7690-133">createdDateTime</span></span>      | <span data-ttu-id="b7690-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b7690-134">DateTimeOffset</span></span>     | <span data-ttu-id="b7690-p106">アイテム作成の日時。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="b7690-p106">Date and time of item creation. Read-only.</span></span>
| <span data-ttu-id="b7690-137">cTag</span><span class="sxs-lookup"><span data-stu-id="b7690-137">cTag</span></span>                 | <span data-ttu-id="b7690-138">String</span><span class="sxs-lookup"><span data-stu-id="b7690-138">String</span></span>             | <span data-ttu-id="b7690-p107">アイテムのコンテンツの eTag。メタデータのみが変更された場合、この eTag は変更されません。**注:** アイテムがフォルダーである場合、このプロパティは返されません。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="b7690-p107">An eTag for the content of the item. This eTag is not changed if only the metadata is changed. **Note** This property is not returned if the item is a folder. Read-only.</span></span>
| <span data-ttu-id="b7690-143">deleted</span><span class="sxs-lookup"><span data-stu-id="b7690-143">deleted</span></span>              | <span data-ttu-id="b7690-144">[deleted][]</span><span class="sxs-lookup"><span data-stu-id="b7690-144">[deleted][]</span></span>        | <span data-ttu-id="b7690-p108">アイテムの削除状態に関する情報。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="b7690-p108">Information about the deleted state of the item. Read-only.</span></span>
| <span data-ttu-id="b7690-147">description</span><span class="sxs-lookup"><span data-stu-id="b7690-147">description</span></span>          | <span data-ttu-id="b7690-148">String</span><span class="sxs-lookup"><span data-stu-id="b7690-148">String</span></span>             | <span data-ttu-id="b7690-p109">ユーザーに表示されるアイテムの説明を提供します。読み取り/書き込み。OneDrive 個人用においてのみ</span><span class="sxs-lookup"><span data-stu-id="b7690-p109">Provides a user-visible description of the item. Read-write. Only on OneDrive Personal</span></span>
| <span data-ttu-id="b7690-152">eTag</span><span class="sxs-lookup"><span data-stu-id="b7690-152">eTag</span></span>                 | <span data-ttu-id="b7690-153">String</span><span class="sxs-lookup"><span data-stu-id="b7690-153">String</span></span>             | <span data-ttu-id="b7690-p110">アイテム全体 (メタデータおよびコンテンツ) の eTag。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="b7690-p110">eTag for the entire item (metadata + content). Read-only.</span></span>
| <span data-ttu-id="b7690-156">file</span><span class="sxs-lookup"><span data-stu-id="b7690-156">file</span></span>                 | <span data-ttu-id="b7690-157">[file][]</span><span class="sxs-lookup"><span data-stu-id="b7690-157">[file][]</span></span>           | <span data-ttu-id="b7690-p111">ファイルのメタデータ (アイテムがファイルである場合)。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="b7690-p111">File metadata, if the item is a file. Read-only.</span></span>
| <span data-ttu-id="b7690-160">fileSystemInfo</span><span class="sxs-lookup"><span data-stu-id="b7690-160">fileSystemInfo</span></span>       | <span data-ttu-id="b7690-161">[fileSystemInfo][]</span><span class="sxs-lookup"><span data-stu-id="b7690-161">[fileSystemInfo][]</span></span> | <span data-ttu-id="b7690-p112">クライアント上のファイル システム情報。読み取り/書き込み。</span><span class="sxs-lookup"><span data-stu-id="b7690-p112">File system information on client. Read-write.</span></span>
| <span data-ttu-id="b7690-164">folder</span><span class="sxs-lookup"><span data-stu-id="b7690-164">folder</span></span>               | <span data-ttu-id="b7690-165">[フォルダー][]</span><span class="sxs-lookup"><span data-stu-id="b7690-165">[folder][]</span></span>         | <span data-ttu-id="b7690-p113">フォルダーのメタデータ (アイテムがフォルダーである場合)。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="b7690-p113">Folder metadata, if the item is a folder. Read-only.</span></span>
| <span data-ttu-id="b7690-168">id</span><span class="sxs-lookup"><span data-stu-id="b7690-168">id</span></span>                   | <span data-ttu-id="b7690-169">String</span><span class="sxs-lookup"><span data-stu-id="b7690-169">String</span></span>             | <span data-ttu-id="b7690-p114">ドライブ内のアイテムの一意識別子。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="b7690-p114">The unique identifier of the item within the Drive. Read-only.</span></span>
| <span data-ttu-id="b7690-172">image</span><span class="sxs-lookup"><span data-stu-id="b7690-172">image</span></span>                | <span data-ttu-id="b7690-173">[image][]</span><span class="sxs-lookup"><span data-stu-id="b7690-173">[image][]</span></span>          | <span data-ttu-id="b7690-p115">画像のメタデータ (アイテムが画像である場合)。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="b7690-p115">Image metadata, if the item is an image. Read-only.</span></span>
| <span data-ttu-id="b7690-176">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="b7690-176">lastModifiedBy</span></span>       | <span data-ttu-id="b7690-177">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="b7690-177">[identitySet][]</span></span>    | <span data-ttu-id="b7690-p116">アイテムを最終更新したユーザーの ID、デバイス、アプリケーション。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="b7690-p116">Identity of the user, device, and application which last modified the item. Read-only.</span></span>
| <span data-ttu-id="b7690-180">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b7690-180">lastModifiedDateTime</span></span> | <span data-ttu-id="b7690-181">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b7690-181">DateTimeOffset</span></span>     | <span data-ttu-id="b7690-p117">アイテムが最後に変更された日時。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="b7690-p117">Date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="b7690-184">location</span><span class="sxs-lookup"><span data-stu-id="b7690-184">location</span></span>             | <span data-ttu-id="b7690-185">[geoCoordinates][]</span><span class="sxs-lookup"><span data-stu-id="b7690-185">[geoCoordinates][]</span></span> | <span data-ttu-id="b7690-p118">場所のメタデータ (アイテムに場所データが含まれている場合)。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="b7690-p118">Location metadata, if the item has location data. Read-only.</span></span>
| <span data-ttu-id="b7690-188">name</span><span class="sxs-lookup"><span data-stu-id="b7690-188">name</span></span>                 | <span data-ttu-id="b7690-189">String</span><span class="sxs-lookup"><span data-stu-id="b7690-189">String</span></span>             | <span data-ttu-id="b7690-p119">アイテムの名前 (ファイル名と拡張子)。読み取り/書き込み。</span><span class="sxs-lookup"><span data-stu-id="b7690-p119">The name of the item (filename and extension). Read-write.</span></span>
| <span data-ttu-id="b7690-192">package</span><span class="sxs-lookup"><span data-stu-id="b7690-192">package</span></span>              | <span data-ttu-id="b7690-193">[package][]</span><span class="sxs-lookup"><span data-stu-id="b7690-193">[package][]</span></span>        | <span data-ttu-id="b7690-p120">これがある場合、アイテムはフォルダーやファイルではなく、パッケージです。パッケージは、コンテキスト次第で、ファイルとして、あるいはフォルダーとして扱われます。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="b7690-p120">If present, indicates that this item is a package instead of a folder or file. Packages are treated like files in some contexts and folders in others. Read-only.</span></span>
| <span data-ttu-id="b7690-197">parentReference</span><span class="sxs-lookup"><span data-stu-id="b7690-197">parentReference</span></span>      | <span data-ttu-id="b7690-198">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="b7690-198">[itemReference][]</span></span>  | <span data-ttu-id="b7690-p121">親の情報 (アイテムに親がある場合)。読み取り/書き込み。</span><span class="sxs-lookup"><span data-stu-id="b7690-p121">Parent information, if the item has a parent. Read-write.</span></span>
| <span data-ttu-id="b7690-201">写真</span><span class="sxs-lookup"><span data-stu-id="b7690-201">photo</span></span>                | <span data-ttu-id="b7690-202">[photo][]</span><span class="sxs-lookup"><span data-stu-id="b7690-202">[photo][]</span></span>          | <span data-ttu-id="b7690-p122">写真のメタデータ (アイテムが写真である場合)。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="b7690-p122">Photo metadata, if the item is a photo. Read-only.</span></span>
| <span data-ttu-id="b7690-205">publication</span><span class="sxs-lookup"><span data-stu-id="b7690-205">publication</span></span>          | <span data-ttu-id="b7690-206">[publicationFacet][]</span><span class="sxs-lookup"><span data-stu-id="b7690-206">[publicationFacet][]</span></span> | <span data-ttu-id="b7690-207">アイテムが公開されているか、チェックアウトの状態かどうかの情報を、そのような操作をサポートする場所で提供します。</span><span class="sxs-lookup"><span data-stu-id="b7690-207">Provides information about the published or checked-out state of an item, in locations that support such actions.</span></span> <span data-ttu-id="b7690-208">既定では、このプロパティは返されません。</span><span class="sxs-lookup"><span data-stu-id="b7690-208">This property is not returned by default.</span></span> <span data-ttu-id="b7690-209">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="b7690-209">Read-only.</span></span> |
| <span data-ttu-id="b7690-210">remoteItem</span><span class="sxs-lookup"><span data-stu-id="b7690-210">remoteItem</span></span>           | <span data-ttu-id="b7690-211">[remoteItem][]</span><span class="sxs-lookup"><span data-stu-id="b7690-211">[remoteItem][]</span></span>     | <span data-ttu-id="b7690-p124">リモート アイテムのデータ (現在アクセス中のドライブ以外のドライブから共有されているアイテムの場合)。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="b7690-p124">Remote item data, if the item is shared from a drive other than the one being accessed. Read-only.</span></span>
| <span data-ttu-id="b7690-214">root</span><span class="sxs-lookup"><span data-stu-id="b7690-214">root</span></span>                 | <span data-ttu-id="b7690-215">[root][]</span><span class="sxs-lookup"><span data-stu-id="b7690-215">[root][]</span></span>           | <span data-ttu-id="b7690-216">このプロパティが null ではない場合は、driveItem がドライブで最上位の driveItem であることを示します。</span><span class="sxs-lookup"><span data-stu-id="b7690-216">If this property is non-null, it indicates that the driveItem is the top-most driveItem in the drive.</span></span>
| <span data-ttu-id="b7690-217">searchResult</span><span class="sxs-lookup"><span data-stu-id="b7690-217">searchResult</span></span>         | <span data-ttu-id="b7690-218">[searchResult][]</span><span class="sxs-lookup"><span data-stu-id="b7690-218">[searchResult][]</span></span>   | <span data-ttu-id="b7690-p125">検索のメタデータ (検索結果に由来するアイテムの場合)。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="b7690-p125">Search metadata, if the item is from a search result. Read-only.</span></span>
| <span data-ttu-id="b7690-221">共有</span><span class="sxs-lookup"><span data-stu-id="b7690-221">shared</span></span>               | <span data-ttu-id="b7690-222">[shared][]</span><span class="sxs-lookup"><span data-stu-id="b7690-222">[shared][]</span></span>         | <span data-ttu-id="b7690-p126">アイテムが他のユーザーと共有されていることを示し、アイテムの共有状態に関する情報を提供します。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="b7690-p126">Indicates that the item has been shared with others and provides information about the shared state of the item. Read-only.</span></span>
| <span data-ttu-id="b7690-225">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="b7690-225">sharepointIds</span></span>        | <span data-ttu-id="b7690-226">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="b7690-226">[sharepointIds][]</span></span>  | <span data-ttu-id="b7690-p127">SharePoint REST 互換性に役立つ識別子を返します。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="b7690-p127">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>
| <span data-ttu-id="b7690-229">size</span><span class="sxs-lookup"><span data-stu-id="b7690-229">size</span></span>                 | <span data-ttu-id="b7690-230">Int64</span><span class="sxs-lookup"><span data-stu-id="b7690-230">Int64</span></span>              | <span data-ttu-id="b7690-p128">アイテムのサイズ (バイト単位)。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="b7690-p128">Size of the item in bytes. Read-only.</span></span>
| <span data-ttu-id="b7690-233">specialFolder</span><span class="sxs-lookup"><span data-stu-id="b7690-233">specialFolder</span></span>        | <span data-ttu-id="b7690-234">[specialFolder][]</span><span class="sxs-lookup"><span data-stu-id="b7690-234">[specialFolder][]</span></span>  | <span data-ttu-id="b7690-p129">現在のアイテムが特別なフォルダーとしても使用可能な場合は、このファセットが返されます。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="b7690-p129">If the current item is also available as a special folder, this facet is returned. Read-only.</span></span>
| <span data-ttu-id="b7690-237">video</span><span class="sxs-lookup"><span data-stu-id="b7690-237">video</span></span>                | <span data-ttu-id="b7690-238">[video][]</span><span class="sxs-lookup"><span data-stu-id="b7690-238">[video][]</span></span>          | <span data-ttu-id="b7690-p130">ビデオのメタデータ (アイテムがビデオである場合)。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="b7690-p130">Video metadata, if the item is a video. Read-only.</span></span>
| <span data-ttu-id="b7690-241">webDavUrl</span><span class="sxs-lookup"><span data-stu-id="b7690-241">webDavUrl</span></span>            | <span data-ttu-id="b7690-242">String</span><span class="sxs-lookup"><span data-stu-id="b7690-242">String</span></span>             | <span data-ttu-id="b7690-243">アイテムの WebDAV 互換性のある URL。</span><span class="sxs-lookup"><span data-stu-id="b7690-243">WebDAV compatible URL for the item.</span></span>
| <span data-ttu-id="b7690-244">webUrl</span><span class="sxs-lookup"><span data-stu-id="b7690-244">webUrl</span></span>               | <span data-ttu-id="b7690-245">String</span><span class="sxs-lookup"><span data-stu-id="b7690-245">String</span></span>             | <span data-ttu-id="b7690-p131">ブラウザーでリソースを表示するための URL。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="b7690-p131">URL that displays the resource in the browser. Read-only.</span></span>

<span data-ttu-id="b7690-p132">**注:** eTag プロパティと cTag プロパティは、コンテナー (フォルダー) 上での機能が異なります。cTag 値は、フォルダーのいずれかの子孫のコンテンツまたはメタデータが変更されると変更されます。eTag 値は、子孫から派生したプロパティ (**childCount** や **lastModifiedDateTime** など) 以外のフォルダーのプロパティが変更されたときにのみ、変更されます。</span><span class="sxs-lookup"><span data-stu-id="b7690-p132">**Note:** The eTag and cTag properties work differently on containers (folders). The cTag value is modified when content or metadata of any descendant of the folder is changed. The eTag value is only modified when the folder's properties are changed, except for properties that are derived from descendants (like **childCount** or **lastModifiedDateTime**).</span></span>

## <a name="relationships"></a><span data-ttu-id="b7690-251">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="b7690-251">Relationships</span></span>

| <span data-ttu-id="b7690-252">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="b7690-252">Relationship</span></span>       | <span data-ttu-id="b7690-253">型</span><span class="sxs-lookup"><span data-stu-id="b7690-253">Type</span></span>                        | <span data-ttu-id="b7690-254">説明</span><span class="sxs-lookup"><span data-stu-id="b7690-254">Description</span></span>
|:-------------------|:----------------------------|:--------------------------
| <span data-ttu-id="b7690-255">アクティビティ</span><span class="sxs-lookup"><span data-stu-id="b7690-255">activities</span></span>         | <span data-ttu-id="b7690-256">[itemActivity][] コレクション</span><span class="sxs-lookup"><span data-stu-id="b7690-256">[itemActivity][] collection</span></span> | <span data-ttu-id="b7690-257">このアイテムに対して行われた最近のアクティビティのリストです。</span><span class="sxs-lookup"><span data-stu-id="b7690-257">The list of recent activities that took place on this item.</span></span>
| <span data-ttu-id="b7690-258">分析</span><span class="sxs-lookup"><span data-stu-id="b7690-258">analytics</span></span>          | <span data-ttu-id="b7690-259">[itemAnalytics][] リソース</span><span class="sxs-lookup"><span data-stu-id="b7690-259">[itemAnalytics][] resource</span></span>  | <span data-ttu-id="b7690-260">このアイテムについて行われたビュー アクティビティに関する分析。</span><span class="sxs-lookup"><span data-stu-id="b7690-260">Analytics about the view activities that took place on this item.</span></span>
| <span data-ttu-id="b7690-261">children</span><span class="sxs-lookup"><span data-stu-id="b7690-261">children</span></span>           | <span data-ttu-id="b7690-262">driveItem コレクション</span><span class="sxs-lookup"><span data-stu-id="b7690-262">driveItem collection</span></span>        | <span data-ttu-id="b7690-p133">アイテムの直接の子のアイテム オブジェクトを格納するコレクション。子が含まれるのは、フォルダーを表すアイテムのみです。読み取り専用です。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="b7690-p133">Collection containing Item objects for the immediate children of Item. Only items representing folders have children. Read-only. Nullable.</span></span>
| <span data-ttu-id="b7690-267">createdByUser</span><span class="sxs-lookup"><span data-stu-id="b7690-267">createdByUser</span></span>      | <span data-ttu-id="b7690-268">[user][]</span><span class="sxs-lookup"><span data-stu-id="b7690-268">[user][]</span></span>                    | <span data-ttu-id="b7690-269">アイテムを作成したユーザーの ID です。</span><span class="sxs-lookup"><span data-stu-id="b7690-269">Identity of the user who created the item.</span></span> <span data-ttu-id="b7690-270">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="b7690-270">Read-only.</span></span>
| <span data-ttu-id="b7690-271">lastModifiedByUser</span><span class="sxs-lookup"><span data-stu-id="b7690-271">lastModifiedByUser</span></span> | <span data-ttu-id="b7690-272">[user][]</span><span class="sxs-lookup"><span data-stu-id="b7690-272">[user][]</span></span>                    | <span data-ttu-id="b7690-273">アイテムを最後に変更したユーザーの ID です。</span><span class="sxs-lookup"><span data-stu-id="b7690-273">Identity of the user who last modified the item.</span></span> <span data-ttu-id="b7690-274">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="b7690-274">Read-only.</span></span>
| <span data-ttu-id="b7690-275">listItem</span><span class="sxs-lookup"><span data-stu-id="b7690-275">listItem</span></span>           | <span data-ttu-id="b7690-276">[listItem][]</span><span class="sxs-lookup"><span data-stu-id="b7690-276">[listItem][]</span></span>                | <span data-ttu-id="b7690-277">SharePoint のドライブの場合は、関連付けられているドキュメント ライブラリのリスト アイテム。</span><span class="sxs-lookup"><span data-stu-id="b7690-277">For drives in SharePoint, the associated document library list item.</span></span> <span data-ttu-id="b7690-278">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="b7690-278">Read-only.</span></span> <span data-ttu-id="b7690-279">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="b7690-279">Nullable.</span></span>
| <span data-ttu-id="b7690-280">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="b7690-280">permissions</span></span>        | <span data-ttu-id="b7690-281">[permission][] コレクション</span><span class="sxs-lookup"><span data-stu-id="b7690-281">[permission][] collection</span></span>   | <span data-ttu-id="b7690-p137">アイテムのアクセス許可のセット。読み取り専用です。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="b7690-p137">The set of permissions for the item. Read-only. Nullable.</span></span>
| <span data-ttu-id="b7690-285">subscriptions</span><span class="sxs-lookup"><span data-stu-id="b7690-285">subscriptions</span></span>      | <span data-ttu-id="b7690-286">[subscription][] コレクション</span><span class="sxs-lookup"><span data-stu-id="b7690-286">[subscription][] collection</span></span> | <span data-ttu-id="b7690-287">アイテムのサブスクリプションのセット。</span><span class="sxs-lookup"><span data-stu-id="b7690-287">The set of subscriptions on the item.</span></span> <span data-ttu-id="b7690-288">ドライブのルートでのみサポートされています。</span><span class="sxs-lookup"><span data-stu-id="b7690-288">Only supported on the root of a drive.</span></span>
| <span data-ttu-id="b7690-289">thumbnails</span><span class="sxs-lookup"><span data-stu-id="b7690-289">thumbnails</span></span>         | <span data-ttu-id="b7690-290">[thumbnailSet][] コレクション</span><span class="sxs-lookup"><span data-stu-id="b7690-290">[thumbnailSet][] collection</span></span> | <span data-ttu-id="b7690-p139">アイテムに関連付けられた [ThumbnailSet][] オブジェクトを格納するコレクション。詳細については、[サムネイルの取得][]についてのページをご覧ください。読み取り専用です。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="b7690-p139">Collection containing [ThumbnailSet][] objects associated with the item. For more info, see [getting thumbnails][]. Read-only. Nullable.</span></span>
| <span data-ttu-id="b7690-295">versions</span><span class="sxs-lookup"><span data-stu-id="b7690-295">versions</span></span>           | <span data-ttu-id="b7690-296">[driveItemVersion][] コレクション</span><span class="sxs-lookup"><span data-stu-id="b7690-296">[driveItemVersion][] collection</span></span> | <span data-ttu-id="b7690-297">アイテムの以前のバージョンのリスト。</span><span class="sxs-lookup"><span data-stu-id="b7690-297">The list of previous versions of the item.</span></span> <span data-ttu-id="b7690-298">詳細については、「[バージョンの一覧表示][]」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b7690-298">For more info, see [getting previous versions][].</span></span> <span data-ttu-id="b7690-299">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="b7690-299">Read-only.</span></span> <span data-ttu-id="b7690-300">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="b7690-300">Nullable.</span></span>
| <span data-ttu-id="b7690-301">workbook</span><span class="sxs-lookup"><span data-stu-id="b7690-301">workbook</span></span>           | <span data-ttu-id="b7690-302">[workbook][]</span><span class="sxs-lookup"><span data-stu-id="b7690-302">[workbook][]</span></span>                | <span data-ttu-id="b7690-303">Excel スプレッドシートであるファイルの場合、スプレッドシートのコンテンツを操作するためにブックの API にアクセスします。</span><span class="sxs-lookup"><span data-stu-id="b7690-303">For files that are Excel spreadsheets, accesses the workbook API to work with the spreadsheet's contents.</span></span> <span data-ttu-id="b7690-304">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="b7690-304">Nullable.</span></span>

## <a name="instance-attributes"></a><span data-ttu-id="b7690-305">インスタンスの属性</span><span class="sxs-lookup"><span data-stu-id="b7690-305">Instance Attributes</span></span>

<span data-ttu-id="b7690-p142">インスタンスの属性は、動作が特殊なプロパティです。これらのプロパティは一時的なものであり、a) サービスの動作を定義するか、b) 短期的なプロパティの値 (有効期限を持つアイテムのダウンロード URL など) を提供します。</span><span class="sxs-lookup"><span data-stu-id="b7690-p142">Instance attributes are properties with special behaviors. These properties are temporary and either a) define behavior the service should perform or b) provide short-term property values, like a download URL for an item that expires.</span></span>

| <span data-ttu-id="b7690-308">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="b7690-308">Property name</span></span>                     | <span data-ttu-id="b7690-309">種類</span><span class="sxs-lookup"><span data-stu-id="b7690-309">Type</span></span>   | <span data-ttu-id="b7690-310">説明</span><span class="sxs-lookup"><span data-stu-id="b7690-310">Description</span></span>
|:----------------------------------|:-------|:--------------------------------
| <span data-ttu-id="b7690-311">@microsoft.graph.conflictBehavior</span><span class="sxs-lookup"><span data-stu-id="b7690-311">@microsoft.graph.conflictBehavior</span></span> | <span data-ttu-id="b7690-312">string</span><span class="sxs-lookup"><span data-stu-id="b7690-312">string</span></span> | <span data-ttu-id="b7690-p143">新しいアイテムを作成するアクションの競合を解決する動作。*fail*、*replace*、*rename* という値を使用できます。PUT の既定値は *replace* です。この注釈とともにアイテムが返されることはありません。書き込み専用です。</span><span class="sxs-lookup"><span data-stu-id="b7690-p143">The conflict resolution behavior for actions that create a new item. You can use the values *fail*, *replace*, or *rename*. The default for PUT is *replace*. An item will never be returned with this annotation. Write-only.</span></span>
| <span data-ttu-id="b7690-318">@microsoft.graph.downloadUrl</span><span class="sxs-lookup"><span data-stu-id="b7690-318">@microsoft.graph.downloadUrl</span></span>      | <span data-ttu-id="b7690-319">string</span><span class="sxs-lookup"><span data-stu-id="b7690-319">string</span></span> | <span data-ttu-id="b7690-p144">このファイルのコンテンツをダウンロードするために使用できる URL。この URL では認証は必要ありません。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="b7690-p144">A URL that can be used to download this file's content. Authentication is not required with this URL. Read-only.</span></span>
| <span data-ttu-id="b7690-323">@microsoft.graph.sourceUrl</span><span class="sxs-lookup"><span data-stu-id="b7690-323">@microsoft.graph.sourceUrl</span></span>        | <span data-ttu-id="b7690-324">string</span><span class="sxs-lookup"><span data-stu-id="b7690-324">string</span></span> | <span data-ttu-id="b7690-p145">PUT 要求を発行するときにこのインスタンスの注釈を使用すると、サービスに対し、URL のコンテンツをダウンロードし、それをファイルとして保存するように指示できます。書き込み専用です。</span><span class="sxs-lookup"><span data-stu-id="b7690-p145">When issuing a PUT request, this instance annotation can be used to instruct the service to download the contents of the URL, and store it as the file. Write-only.</span></span>

<span data-ttu-id="b7690-327">**注:**@microsoft.graph.downloadUrl の値は短時間限定の URL であるため、キャッシュすることはできません。</span><span class="sxs-lookup"><span data-stu-id="b7690-327">**Note:** The @microsoft.graph.downloadUrl value is a short-lived URL and can't be cached.</span></span>
<span data-ttu-id="b7690-328">URL は短い期間 (1 時間) だけ使用でき、その後は無効になります。</span><span class="sxs-lookup"><span data-stu-id="b7690-328">The URL will only be available for a short period of time (1 hour) before it is invalidated.</span></span>
<span data-ttu-id="b7690-329">ユーザーのファイルへのアクセス許可を削除しても、すぐに URL が無効にならない場合があります。</span><span class="sxs-lookup"><span data-stu-id="b7690-329">Removing file permissions for a user may not immediately invalidate the URL.</span></span>

## <a name="json-representation"></a><span data-ttu-id="b7690-330">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b7690-330">JSON representation</span></span>

<span data-ttu-id="b7690-331">以下は、**driveItem** リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="b7690-331">Here is a JSON representation of a **driveItem** resource.</span></span>

<span data-ttu-id="b7690-332">
            \*\*driveItem\*\* リソースは [\*\*baseItem\*\*][baseItem] から派生し、そのリソースからプロパティを継承します。</span><span class="sxs-lookup"><span data-stu-id="b7690-332">The **driveItem** resource is derived from [**baseItem**][baseItem] and inherits properties from that resource.</span></span>

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
  "analytics": {"@odata.type": "microsoft.graph.itemAnalytics"},
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

## <a name="methods"></a><span data-ttu-id="b7690-333">メソッド</span><span class="sxs-lookup"><span data-stu-id="b7690-333">Methods</span></span>

| <span data-ttu-id="b7690-334">メソッド</span><span class="sxs-lookup"><span data-stu-id="b7690-334">Method</span></span>                                                   | <span data-ttu-id="b7690-335">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="b7690-335">Return Type</span></span> | <span data-ttu-id="b7690-336">説明</span><span class="sxs-lookup"><span data-stu-id="b7690-336">Description</span></span>
|:---------------------------------------------------------|:------------|:------------
| [<span data-ttu-id="b7690-337">アイテムを取得する</span><span class="sxs-lookup"><span data-stu-id="b7690-337">Get item</span></span>](../api/driveitem-get.md)                      | <span data-ttu-id="b7690-338">driveItem</span><span class="sxs-lookup"><span data-stu-id="b7690-338">driveItem</span></span> |<span data-ttu-id="b7690-339">ドライブ 内の DriveItem 用のメタデータを取得します。</span><span class="sxs-lookup"><span data-stu-id="b7690-339">Retrieve the metadata for a DriveItem in a Drive.</span></span>
| <span data-ttu-id="b7690-340">[分析を取得する][]</span><span class="sxs-lookup"><span data-stu-id="b7690-340">[Get analytics][]</span></span>                                        | <span data-ttu-id="b7690-341">[itemAnalytics][]</span><span class="sxs-lookup"><span data-stu-id="b7690-341">[itemAnalytics][]</span></span> | <span data-ttu-id="b7690-342">このリソースの分析を取得します。</span><span class="sxs-lookup"><span data-stu-id="b7690-342">Get analytics for this resource.</span></span> 
| <span data-ttu-id="b7690-343">[間隔ごとにアクティビティを取得する][]</span><span class="sxs-lookup"><span data-stu-id="b7690-343">[Get activities by interval][]</span></span>                           | <span data-ttu-id="b7690-344">[itemActivityStat][]</span><span class="sxs-lookup"><span data-stu-id="b7690-344">[itemActivityStat][]</span></span> | <span data-ttu-id="b7690-345">指定した時間間隔内に itemActivityStats のコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="b7690-345">Get a collection of itemActivityStats within the specified time interval.</span></span>
| [<span data-ttu-id="b7690-346">子を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="b7690-346">List children</span></span>](../api/driveitem-list-children.md)       | <span data-ttu-id="b7690-347">DriveItem のコレクション</span><span class="sxs-lookup"><span data-stu-id="b7690-347">collection of driveItem</span></span> | <span data-ttu-id="b7690-348">DriveItem の子リレーションシップで DriveItems のコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="b7690-348">Return a collection of DriveItems in the children relationship of a DriveItem.</span></span>
| [<span data-ttu-id="b7690-349">バージョンを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="b7690-349">List versions</span></span>](../api/driveitem-list-versions.md)       | <span data-ttu-id="b7690-350">[DriveItemVersion][] のコレクション</span><span class="sxs-lookup"><span data-stu-id="b7690-350">collection of [DriveItemVersion][]</span></span> | <span data-ttu-id="b7690-351">現在のユーザーのドライブ内のファイルのバージョンを取得します。</span><span class="sxs-lookup"><span data-stu-id="b7690-351">Retrieves the versions of a file in the current user's drive.</span></span>
| [<span data-ttu-id="b7690-352">アイテムを作成する</span><span class="sxs-lookup"><span data-stu-id="b7690-352">Create item</span></span>](../api/driveitem-post-children.md)         | <span data-ttu-id="b7690-353">driveItem</span><span class="sxs-lookup"><span data-stu-id="b7690-353">driveItem</span></span> | <span data-ttu-id="b7690-354">指定したドライブで driveItem を作成します。</span><span class="sxs-lookup"><span data-stu-id="b7690-354">Creates a driveItem in the specified drive.</span></span>
| [<span data-ttu-id="b7690-355">アイテムを更新する</span><span class="sxs-lookup"><span data-stu-id="b7690-355">Update item</span></span>](../api/driveitem-update.md)                | <span data-ttu-id="b7690-356">driveItem</span><span class="sxs-lookup"><span data-stu-id="b7690-356">driveItem</span></span> | <span data-ttu-id="b7690-357">ドライブで driveItem を更新します。</span><span class="sxs-lookup"><span data-stu-id="b7690-357">Updates a driveItem in the drive.</span></span>
| [<span data-ttu-id="b7690-358">コンテンツをアップロードする</span><span class="sxs-lookup"><span data-stu-id="b7690-358">Upload content</span></span>](../api/driveitem-put-content.md)        | <span data-ttu-id="b7690-359">driveItem</span><span class="sxs-lookup"><span data-stu-id="b7690-359">driveItem</span></span> | <span data-ttu-id="b7690-360">コンテンツを driveItem にアップロードします。</span><span class="sxs-lookup"><span data-stu-id="b7690-360">Uploads content to the driveItem.</span></span>
| [<span data-ttu-id="b7690-361">コンテンツをダウンロードする</span><span class="sxs-lookup"><span data-stu-id="b7690-361">Download content</span></span>](../api/driveitem-get-content.md)      | <span data-ttu-id="b7690-362">ダウンロード URL</span><span class="sxs-lookup"><span data-stu-id="b7690-362">download Url</span></span> | <span data-ttu-id="b7690-363">DriveItem のコンテンツをダウンロードします。</span><span class="sxs-lookup"><span data-stu-id="b7690-363">Downloads content of a driveItem.</span></span>
| <span data-ttu-id="b7690-364">[特定のファイル形式をダウンロードする][download-format]</span><span class="sxs-lookup"><span data-stu-id="b7690-364">[Download specific file format][download-format]</span></span>         | <span data-ttu-id="b7690-365">ダウンロード URL</span><span class="sxs-lookup"><span data-stu-id="b7690-365">download Url</span></span> | <span data-ttu-id="b7690-366">DriveItem のコンテンツを特定の形式でダウンロードします。</span><span class="sxs-lookup"><span data-stu-id="b7690-366">Downloads content of a driveItem with a specific format.</span></span>
| [<span data-ttu-id="b7690-367">アイテムを削除する</span><span class="sxs-lookup"><span data-stu-id="b7690-367">Delete item</span></span>](../api/driveitem-delete.md)                | <span data-ttu-id="b7690-368">コンテンツはありません</span><span class="sxs-lookup"><span data-stu-id="b7690-368">No Content</span></span> | <span data-ttu-id="b7690-369">DriveItem を削除します。</span><span class="sxs-lookup"><span data-stu-id="b7690-369">Deletes a driveItem.</span></span>
| [<span data-ttu-id="b7690-370">アイテムを移動する</span><span class="sxs-lookup"><span data-stu-id="b7690-370">Move item</span></span>](../api/driveitem-move.md)                    | <span data-ttu-id="b7690-371">driveItem</span><span class="sxs-lookup"><span data-stu-id="b7690-371">driveItem</span></span> | <span data-ttu-id="b7690-372">DriveItem を新しい親アイテムに移動します。</span><span class="sxs-lookup"><span data-stu-id="b7690-372">Move a DriveItem to a new parent item.</span></span>
| [<span data-ttu-id="b7690-373">アイテムをコピーする</span><span class="sxs-lookup"><span data-stu-id="b7690-373">Copy item</span></span>](../api/driveitem-copy.md)                    | <span data-ttu-id="b7690-374">コピーの[進行状況を監視する](/graph/long-running-actions-overview)方法についての詳細</span><span class="sxs-lookup"><span data-stu-id="b7690-374">details about how to [monitor the progress](/graph/long-running-actions-overview) of the copy</span></span> | <span data-ttu-id="b7690-375">DriveItem (すべての子を含む) のコピーを作成します。</span><span class="sxs-lookup"><span data-stu-id="b7690-375">Creates a copy of an driveItem (including any children).</span></span>
| [<span data-ttu-id="b7690-376">アイテムを検索する</span><span class="sxs-lookup"><span data-stu-id="b7690-376">Search items</span></span>](../api/driveitem-search.md)               | <span data-ttu-id="b7690-377">DriveItem のコレクション</span><span class="sxs-lookup"><span data-stu-id="b7690-377">collection of driveItem</span></span> | <span data-ttu-id="b7690-378">クエリと一致するアイテムを対象にアイテムの階層を検索します。</span><span class="sxs-lookup"><span data-stu-id="b7690-378">Search the hierarchy of items for items matching a query.</span></span>
| [<span data-ttu-id="b7690-379">ドライブ内の変更内容を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="b7690-379">List changes in a drive</span></span>](../api/driveitem-delta.md)     | <span data-ttu-id="b7690-380">差分リンク</span><span class="sxs-lookup"><span data-stu-id="b7690-380">delta link</span></span> | <span data-ttu-id="b7690-381">ドライブでのすべての変更を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="b7690-381">List any changes in the drive.</span></span>
| [<span data-ttu-id="b7690-382">サムネイルを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="b7690-382">List thumbnails</span></span>](../api/driveitem-list-thumbnails.md)   | <span data-ttu-id="b7690-383">DriveItem のコレクション</span><span class="sxs-lookup"><span data-stu-id="b7690-383">colletion of driveItem</span></span> | <span data-ttu-id="b7690-384">DriveItems とそれらのサムネイルを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="b7690-384">List driveItems with their thumbnails.</span></span> 
| [<span data-ttu-id="b7690-385">共有リンクを作成する</span><span class="sxs-lookup"><span data-stu-id="b7690-385">Create sharing link</span></span>](../api/driveitem-createlink.md)    | <span data-ttu-id="b7690-386">共有リンク</span><span class="sxs-lookup"><span data-stu-id="b7690-386">sharing link</span></span> | <span data-ttu-id="b7690-387">DriveItem を共有するためのリンクを作成します。</span><span class="sxs-lookup"><span data-stu-id="b7690-387">Create a link to share the driveItem.</span></span>
| [<span data-ttu-id="b7690-388">アクセス許可を追加する</span><span class="sxs-lookup"><span data-stu-id="b7690-388">Add permissions</span></span>](../api/driveitem-invite.md)            | <span data-ttu-id="b7690-389">[アクセス許可][]のコレクション</span><span class="sxs-lookup"><span data-stu-id="b7690-389">collection of [permission][]</span></span> | <span data-ttu-id="b7690-390">共有の招待をユーザーに送信します。</span><span class="sxs-lookup"><span data-stu-id="b7690-390">Sends a sharing ivite to a user.</span></span>
| [<span data-ttu-id="b7690-391">アクセス許可を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="b7690-391">List permissions</span></span>](../api/driveitem-list-permissions.md) | <span data-ttu-id="b7690-392">[アクセス許可][]のコレクション</span><span class="sxs-lookup"><span data-stu-id="b7690-392">collection of [permission][]</span></span> | <span data-ttu-id="b7690-393">DriveItem に対するアクセス許可のコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="b7690-393">Retrieves the collection of permissions on an driveItem.</span></span>
| [<span data-ttu-id="b7690-394">アクセス許可を削除する</span><span class="sxs-lookup"><span data-stu-id="b7690-394">Delete permission</span></span>](../api/permission-delete.md)         | <span data-ttu-id="b7690-395">コンテンツはありません</span><span class="sxs-lookup"><span data-stu-id="b7690-395">No Content</span></span> | <span data-ttu-id="b7690-396">DriveItem からアクセス許可を削除します。</span><span class="sxs-lookup"><span data-stu-id="b7690-396">Removes the permission from the driveItem.</span></span>
| <span data-ttu-id="b7690-397">[WebSocket チャネルを取得する][getWebSocket]</span><span class="sxs-lookup"><span data-stu-id="b7690-397">[Get WebSocket channel][getWebSocket]</span></span>                    | <span data-ttu-id="b7690-398">[subscription][]</span><span class="sxs-lookup"><span data-stu-id="b7690-398">[subscription][]</span></span> | <span data-ttu-id="b7690-399">Socket.io を使用して、ドライブのリアルタイムに近い変更通知を受信します。</span><span class="sxs-lookup"><span data-stu-id="b7690-399">Receives near-real-time change notifications for a drive using socket.io.</span></span>
| <span data-ttu-id="b7690-400">[アイテムをプレビューする][item-preview]</span><span class="sxs-lookup"><span data-stu-id="b7690-400">[Preview item][item-preview]</span></span>                             | <span data-ttu-id="b7690-401">JSON オブジェクト</span><span class="sxs-lookup"><span data-stu-id="b7690-401">json object</span></span> | <span data-ttu-id="b7690-402">一時的なプレビューを表示するために、アイテムの、有効期限が短い埋め込み可能な URL を取得します。</span><span class="sxs-lookup"><span data-stu-id="b7690-402">Obtain short-lived embeddable URLs for an item in order to render a temporary preview.</span></span>

[item-preview]: ../api/driveitem-preview.md
[分析を取得する]: ../api/itemanalytics-get.md
[Get analytics]: ../api/itemanalytics-get.md
[間隔によりアクティビティを取得する]: ../api/itemactivitystat-getactivitybyinterval.md
[Get activities by interval]: ../api/itemactivitystat-getactivitybyinterval.md

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

[DriveItemVersion]: driveitemversion.md
[permission]: permission.md
[subscription]: subscription.md
[itemActivityStat]: itemactivitystat.md

<!-- {
  "type": "#page.annotation",
  "description": "Item is the main data model in the OneDrive API. Everything is an item.",
  "keywords": "item,facet,resource",
  "section": "documentation",
  "tocPath": "Items",
  "tocBookmarks": { "Resources/Item": "#" }
} -->
