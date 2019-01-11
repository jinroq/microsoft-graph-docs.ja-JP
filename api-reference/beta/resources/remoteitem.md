---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: RemoteItem
localization_priority: Normal
ms.openlocfilehash: 122e13513db1a59e23a41cadd16e61996e6a6c04
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27843191"
---
# <a name="remoteitem-resource-type"></a><span data-ttu-id="3c2d3-102">RemoteItem リソースの種類</span><span class="sxs-lookup"><span data-stu-id="3c2d3-102">RemoteItem resource type</span></span>

> <span data-ttu-id="3c2d3-103">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="3c2d3-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3c2d3-104">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3c2d3-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3c2d3-p102">**remoteItem** リソースは、[**driveItem**](driveitem.md) が別のドライブに存在するアイテムを参照することを示します。このリソースは、ソース ドライブとターゲット項目の固有 ID を提供します。</span><span class="sxs-lookup"><span data-stu-id="3c2d3-p102">The **remoteItem** resource indicates that a [**driveItem**](driveitem.md) references an item that exists in another drive. This resource provides the unique IDs of the source drive and target item.</span></span>

<span data-ttu-id="3c2d3-107">非 null の **remoteItem** ファセットを持つ [**DriveItems**](driveitem.md)は、共有された、ユーザーの OneDrive に追加された、あるいは異質な項目のコレクション (検索結果など) から返される項目上にあるリソースです。</span><span class="sxs-lookup"><span data-stu-id="3c2d3-107">[**DriveItems**](driveitem.md) with a non-null **remoteItem** facet are resources that are shared, added to the user's OneDrive, or on items returned from hetrogenous collections of items (like search results).</span></span>

<span data-ttu-id="3c2d3-108">**注:** 同じドライブにあるフォルダーとは異なり、リモート アイテムに移動された **driveItem** では、`id` 値が変更された可能性があります。</span><span class="sxs-lookup"><span data-stu-id="3c2d3-108">**Note:** Unlike with folders in the same drive, a **driveItem** moved into a remote item may have its `id` value changed.</span></span>

## <a name="json-representation"></a><span data-ttu-id="3c2d3-109">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="3c2d3-109">JSON representation</span></span>

<!-- { "blockType": "resource", 
       "@odata.type": "microsoft.graph.remoteItem", 
       "optionalProperties": ["name", "fileSystemInfo", "file", "folder"] } -->

```json
{
  "id": "string",
  "createdBy": { "@odata.type": "microsoft.graph.identitySet" },
  "createdDateTime": "timestamp",
  "file": { "@odata.type": "microsoft.graph.file" },
  "fileSystemInfo": { "@odata.type": "microsoft.graph.fileSystemInfo" },
  "folder": { "@odata.type": "microsoft.graph.folder" },
  "lastModifiedBy": { "@odata.type": "microsoft.graph.identitySet" },
  "lastModifiedDateTime": "timestamp",
  "name": "string",
  "package": { "@odata.type": "microsoft.graph.package" },
  "parentReference": { "@odata.type": "microsoft.graph.itemReference" },
  "shared": { "@odata.type": "microsoft.graph.shared" },
  "sharepointIds": { "@odata.type": "microsoft.graph.sharepointIds" },
  "size": 1024,
  "webDavUrl": "url",
  "webUrl": "url"
}
```

## <a name="properties"></a><span data-ttu-id="3c2d3-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3c2d3-110">Properties</span></span>

| <span data-ttu-id="3c2d3-111">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="3c2d3-111">Property name</span></span>        | <span data-ttu-id="3c2d3-112">Type</span><span class="sxs-lookup"><span data-stu-id="3c2d3-112">Type</span></span>                                | <span data-ttu-id="3c2d3-113">説明</span><span class="sxs-lookup"><span data-stu-id="3c2d3-113">Description</span></span>                                                                                                                                                       |
| :------------------- | :---------------------------------- | :---------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="3c2d3-114">createdBy</span><span class="sxs-lookup"><span data-stu-id="3c2d3-114">createdBy</span></span>            | [<span data-ttu-id="3c2d3-115">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="3c2d3-115">IdentitySet</span></span>](identityset.md)       | <span data-ttu-id="3c2d3-p103">その項目を作成したユーザー、デバイス、およびアプリケーションの ID。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="3c2d3-p103">Identity of the user, device, and application which created the item. Read-only.</span></span>                                                                                  |
| <span data-ttu-id="3c2d3-118">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3c2d3-118">createdDateTime</span></span>      | <span data-ttu-id="3c2d3-119">Timestamp</span><span class="sxs-lookup"><span data-stu-id="3c2d3-119">Timestamp</span></span>                           | <span data-ttu-id="3c2d3-p104">項目作成の日付と時刻。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="3c2d3-p104">Date and time of item creation. Read-only.</span></span>                                                                                                                        |
| <span data-ttu-id="3c2d3-122">file</span><span class="sxs-lookup"><span data-stu-id="3c2d3-122">file</span></span>                 | [<span data-ttu-id="3c2d3-123">File</span><span class="sxs-lookup"><span data-stu-id="3c2d3-123">File</span></span>](file.md)                     | <span data-ttu-id="3c2d3-p105">リモート項目がファイルであることを示します。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="3c2d3-p105">Indicates that the remote item is a file. Read-only.</span></span>                                                                                                              |
| <span data-ttu-id="3c2d3-126">fileSystemInfo</span><span class="sxs-lookup"><span data-stu-id="3c2d3-126">fileSystemInfo</span></span>       | [<span data-ttu-id="3c2d3-127">FileSystemInfo</span><span class="sxs-lookup"><span data-stu-id="3c2d3-127">FileSystemInfo</span></span>](filesysteminfo.md) | <span data-ttu-id="3c2d3-p106">ローカル ファイル システムからのリモート項目についての情報。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="3c2d3-p106">Information about the remote item from the local file system. Read-only.</span></span>                                                                                          |
| <span data-ttu-id="3c2d3-130">folder</span><span class="sxs-lookup"><span data-stu-id="3c2d3-130">folder</span></span>               | [<span data-ttu-id="3c2d3-131">Folder</span><span class="sxs-lookup"><span data-stu-id="3c2d3-131">Folder</span></span>](folder.md)                 | <span data-ttu-id="3c2d3-p107">リモート項目がフォルダーであることを示します。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="3c2d3-p107">Indicates that the remote item is a folder. Read-only.</span></span>                                                                                                            |
| <span data-ttu-id="3c2d3-134">id</span><span class="sxs-lookup"><span data-stu-id="3c2d3-134">id</span></span>                   | <span data-ttu-id="3c2d3-135">String</span><span class="sxs-lookup"><span data-stu-id="3c2d3-135">String</span></span>                              | <span data-ttu-id="3c2d3-p108">ドライブ内のリモート項目の固有識別子です。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="3c2d3-p108">Unique identifier for the remote item in its drive. Read-only.</span></span>                                                                                                    |
| <span data-ttu-id="3c2d3-138">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="3c2d3-138">lastModifiedBy</span></span>       | [<span data-ttu-id="3c2d3-139">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="3c2d3-139">IdentitySet</span></span>](identityset.md)       | <span data-ttu-id="3c2d3-p109">アイテムを最終更新したユーザーの ID、デバイス、アプリケーション。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="3c2d3-p109">Identity of the user, device, and application which last modified the item. Read-only.</span></span>                                                                            |
| <span data-ttu-id="3c2d3-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3c2d3-142">lastModifiedDateTime</span></span> | <span data-ttu-id="3c2d3-143">Timestamp</span><span class="sxs-lookup"><span data-stu-id="3c2d3-143">Timestamp</span></span>                           | <span data-ttu-id="3c2d3-p110">アイテムが最後に変更された日時。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="3c2d3-p110">Date and time the item was last modified. Read-only.</span></span>                                                                                                              |
| <span data-ttu-id="3c2d3-146">name</span><span class="sxs-lookup"><span data-stu-id="3c2d3-146">name</span></span>                 | <span data-ttu-id="3c2d3-147">String</span><span class="sxs-lookup"><span data-stu-id="3c2d3-147">String</span></span>                              | <span data-ttu-id="3c2d3-p111">省略可能。リモート項目のファイル名です。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="3c2d3-p111">Optional. Filename of the remote item. Read-only.</span></span>                                                                                                                 |
| <span data-ttu-id="3c2d3-151">package</span><span class="sxs-lookup"><span data-stu-id="3c2d3-151">package</span></span>              | [<span data-ttu-id="3c2d3-152">Package</span><span class="sxs-lookup"><span data-stu-id="3c2d3-152">Package</span></span>](package.md)               | <span data-ttu-id="3c2d3-p112">存在する場合、この項目がフォルダーやファイルではなくパッケージであることを示します。パッケージは、一部のコンテキストでのファイルのように、他のコンテキストではフォルダーのように扱われます。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="3c2d3-p112">If present, indicates that this item is a package instead of a folder or file. Packages are treated like files in some contexts and folders in others. Read-only.</span></span> |
| <span data-ttu-id="3c2d3-156">parentReference</span><span class="sxs-lookup"><span data-stu-id="3c2d3-156">parentReference</span></span>      | [<span data-ttu-id="3c2d3-157">ItemReference</span><span class="sxs-lookup"><span data-stu-id="3c2d3-157">ItemReference</span></span>](itemreference.md)   | <span data-ttu-id="3c2d3-p113">リモート項目の親のプロパティです。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="3c2d3-p113">Properties of the parent of the remote item. Read-only.</span></span>                                                                                                           |
| <span data-ttu-id="3c2d3-160">shared</span><span class="sxs-lookup"><span data-stu-id="3c2d3-160">shared</span></span>               | [<span data-ttu-id="3c2d3-161">shared</span><span class="sxs-lookup"><span data-stu-id="3c2d3-161">shared</span></span>](shared.md)                 | <span data-ttu-id="3c2d3-p114">アイテムが他のユーザーと共有されていることを示し、アイテムの共有状態に関する情報を提供します。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="3c2d3-p114">Indicates that the item has been shared with others and provides information about the shared state of the item. Read-only.</span></span>                                       |
| <span data-ttu-id="3c2d3-164">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="3c2d3-164">sharepointIds</span></span>        | [<span data-ttu-id="3c2d3-165">SharepointIds</span><span class="sxs-lookup"><span data-stu-id="3c2d3-165">SharepointIds</span></span>](sharepointids.md)   | <span data-ttu-id="3c2d3-p115">OneDrive for Business と SharePoint 間の相互運用を、項目識別子の完全なセットと共に提供します。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="3c2d3-p115">Provides interop between items in OneDrive for Business and SharePoint with the full set of item identifiers. Read-only.</span></span>                                          |
| <span data-ttu-id="3c2d3-168">size</span><span class="sxs-lookup"><span data-stu-id="3c2d3-168">size</span></span>                 | <span data-ttu-id="3c2d3-169">Int64</span><span class="sxs-lookup"><span data-stu-id="3c2d3-169">Int64</span></span>                               | <span data-ttu-id="3c2d3-p116">リモート項目のサイズです。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="3c2d3-p116">Size of the remote item. Read-only.</span></span>                                                                                                                               |
| <span data-ttu-id="3c2d3-172">webDavUrl</span><span class="sxs-lookup"><span data-stu-id="3c2d3-172">webDavUrl</span></span>            | <span data-ttu-id="3c2d3-173">Url</span><span class="sxs-lookup"><span data-stu-id="3c2d3-173">Url</span></span>                                 | <span data-ttu-id="3c2d3-174">項目の、DAV 互換性のある URL です。</span><span class="sxs-lookup"><span data-stu-id="3c2d3-174">DAV compatible URL for the item.</span></span>                                                                                                                                  |
| <span data-ttu-id="3c2d3-175">webUrl</span><span class="sxs-lookup"><span data-stu-id="3c2d3-175">webUrl</span></span>               | <span data-ttu-id="3c2d3-176">Url</span><span class="sxs-lookup"><span data-stu-id="3c2d3-176">Url</span></span>                                 | <span data-ttu-id="3c2d3-p117">ブラウザーでリソースを表示するための URL。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="3c2d3-p117">URL that displays the resource in the browser. Read-only.</span></span>                                                                                                         |

## <a name="remarks"></a><span data-ttu-id="3c2d3-179">備考</span><span class="sxs-lookup"><span data-stu-id="3c2d3-179">Remarks</span></span>

<span data-ttu-id="3c2d3-180">**driveItem** のファセットに関する詳細については、「[driveItem](driveitem.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3c2d3-180">For more information about the facets on a **driveItem**, see [driveItem](driveitem.md).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The quota facet provides information about how much space the OneDrive has available.",
  "keywords": "quota,available,remaining,used",
  "section": "documentation",
  "tocPath": "Facets/RemoteItem"
} -->
