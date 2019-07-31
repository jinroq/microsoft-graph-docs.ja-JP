---
author: JeremyKelley
description: remoteItem リソースは、driveItem が別のドライブに存在するアイテムを参照することを示します。
ms.date: 09/10/2017
title: RemoteItem
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 05da43fb3d7b1e2adec01f707eeed61df4623f04
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36008706"
---
# <a name="remoteitem-resource-type"></a><span data-ttu-id="66099-103">RemoteItem リソースの種類</span><span class="sxs-lookup"><span data-stu-id="66099-103">RemoteItem resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="66099-104">**remoteItem** リソースは、[**driveItem**](driveitem.md) が別のドライブに存在するアイテムを参照することを示します。</span><span class="sxs-lookup"><span data-stu-id="66099-104">The **remoteItem** resource indicates that a [**driveItem**](driveitem.md) references an item that exists in another drive.</span></span>
<span data-ttu-id="66099-105">このリソースは、ソース ドライブとターゲット項目の固有 ID を提供します。</span><span class="sxs-lookup"><span data-stu-id="66099-105">This resource provides the unique IDs of the source drive and target item.</span></span>

<span data-ttu-id="66099-106">非 null の **remoteItem** ファセットを持つ [**DriveItems**](driveitem.md)は、共有された、ユーザーの OneDrive に追加された、あるいは異質な項目のコレクション (検索結果など) から返される項目上にあるリソースです。</span><span class="sxs-lookup"><span data-stu-id="66099-106">[**DriveItems**](driveitem.md) with a non-null **remoteItem** facet are resources that are shared, added to the user's OneDrive, or on items returned from hetrogenous collections of items (like search results).</span></span>

<span data-ttu-id="66099-107">**注:** 同じドライブにあるフォルダーとは異なり、リモート アイテムに移動された **driveItem** では、`id` 値が変更された可能性があります。</span><span class="sxs-lookup"><span data-stu-id="66099-107">**Note:** Unlike with folders in the same drive, a **driveItem** moved into a remote item may have its `id` value changed.</span></span>

## <a name="json-representation"></a><span data-ttu-id="66099-108">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="66099-108">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="66099-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="66099-109">Properties</span></span>

| <span data-ttu-id="66099-110">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="66099-110">Property name</span></span>        | <span data-ttu-id="66099-111">種類</span><span class="sxs-lookup"><span data-stu-id="66099-111">Type</span></span>                                | <span data-ttu-id="66099-112">説明</span><span class="sxs-lookup"><span data-stu-id="66099-112">Description</span></span>                                                                                                                                                       |
| :------------------- | :---------------------------------- | :---------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="66099-113">createdBy</span><span class="sxs-lookup"><span data-stu-id="66099-113">createdBy</span></span>            | [<span data-ttu-id="66099-114">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="66099-114">IdentitySet</span></span>](identityset.md)       | <span data-ttu-id="66099-p102">そのアイテムを作成したユーザーの ID、デバイス、アプリケーション。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="66099-p102">Identity of the user, device, and application which created the item. Read-only.</span></span>                                                                                  |
| <span data-ttu-id="66099-117">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="66099-117">createdDateTime</span></span>      | <span data-ttu-id="66099-118">Timestamp</span><span class="sxs-lookup"><span data-stu-id="66099-118">Timestamp</span></span>                           | <span data-ttu-id="66099-p103">項目作成の日付と時刻。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="66099-p103">Date and time of item creation. Read-only.</span></span>                                                                                                                        |
| <span data-ttu-id="66099-121">file</span><span class="sxs-lookup"><span data-stu-id="66099-121">file</span></span>                 | [<span data-ttu-id="66099-122">File</span><span class="sxs-lookup"><span data-stu-id="66099-122">File</span></span>](file.md)                     | <span data-ttu-id="66099-p104">リモート項目がファイルであることを示します。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="66099-p104">Indicates that the remote item is a file. Read-only.</span></span>                                                                                                              |
| <span data-ttu-id="66099-125">fileSystemInfo</span><span class="sxs-lookup"><span data-stu-id="66099-125">fileSystemInfo</span></span>       | [<span data-ttu-id="66099-126">FileSystemInfo</span><span class="sxs-lookup"><span data-stu-id="66099-126">FileSystemInfo</span></span>](filesysteminfo.md) | <span data-ttu-id="66099-p105">ローカル ファイル システムからのリモート項目についての情報。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="66099-p105">Information about the remote item from the local file system. Read-only.</span></span>                                                                                          |
| <span data-ttu-id="66099-129">folder</span><span class="sxs-lookup"><span data-stu-id="66099-129">folder</span></span>               | [<span data-ttu-id="66099-130">Folder</span><span class="sxs-lookup"><span data-stu-id="66099-130">Folder</span></span>](folder.md)                 | <span data-ttu-id="66099-p106">リモート項目がフォルダーであることを示します。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="66099-p106">Indicates that the remote item is a folder. Read-only.</span></span>                                                                                                            |
| <span data-ttu-id="66099-133">id</span><span class="sxs-lookup"><span data-stu-id="66099-133">id</span></span>                   | <span data-ttu-id="66099-134">文字列</span><span class="sxs-lookup"><span data-stu-id="66099-134">String</span></span>                              | <span data-ttu-id="66099-p107">ドライブ内のリモート項目の固有識別子です。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="66099-p107">Unique identifier for the remote item in its drive. Read-only.</span></span>                                                                                                    |
| <span data-ttu-id="66099-137">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="66099-137">lastModifiedBy</span></span>       | [<span data-ttu-id="66099-138">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="66099-138">IdentitySet</span></span>](identityset.md)       | <span data-ttu-id="66099-p108">アイテムを最終更新したユーザーの ID、デバイス、アプリケーション。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="66099-p108">Identity of the user, device, and application which last modified the item. Read-only.</span></span>                                                                            |
| <span data-ttu-id="66099-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="66099-141">lastModifiedDateTime</span></span> | <span data-ttu-id="66099-142">Timestamp</span><span class="sxs-lookup"><span data-stu-id="66099-142">Timestamp</span></span>                           | <span data-ttu-id="66099-p109">アイテムが最後に変更された日時。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="66099-p109">Date and time the item was last modified. Read-only.</span></span>                                                                                                              |
| <span data-ttu-id="66099-145">name</span><span class="sxs-lookup"><span data-stu-id="66099-145">name</span></span>                 | <span data-ttu-id="66099-146">String</span><span class="sxs-lookup"><span data-stu-id="66099-146">String</span></span>                              | <span data-ttu-id="66099-p110">省略可能。リモート項目のファイル名です。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="66099-p110">Optional. Filename of the remote item. Read-only.</span></span>                                                                                                                 |
| <span data-ttu-id="66099-150">package</span><span class="sxs-lookup"><span data-stu-id="66099-150">package</span></span>              | [<span data-ttu-id="66099-151">Package</span><span class="sxs-lookup"><span data-stu-id="66099-151">Package</span></span>](package.md)               | <span data-ttu-id="66099-p111">これがある場合、アイテムはフォルダーやファイルではなく、パッケージです。パッケージは、コンテキスト次第で、ファイルとして、あるいはフォルダーとして扱われます。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="66099-p111">If present, indicates that this item is a package instead of a folder or file. Packages are treated like files in some contexts and folders in others. Read-only.</span></span> |
| <span data-ttu-id="66099-155">parentReference</span><span class="sxs-lookup"><span data-stu-id="66099-155">parentReference</span></span>      | [<span data-ttu-id="66099-156">ItemReference</span><span class="sxs-lookup"><span data-stu-id="66099-156">ItemReference</span></span>](itemreference.md)   | <span data-ttu-id="66099-p112">リモート項目の親のプロパティです。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="66099-p112">Properties of the parent of the remote item. Read-only.</span></span>                                                                                                           |
| <span data-ttu-id="66099-159">共有</span><span class="sxs-lookup"><span data-stu-id="66099-159">shared</span></span>               | [<span data-ttu-id="66099-160">shared</span><span class="sxs-lookup"><span data-stu-id="66099-160">shared</span></span>](shared.md)                 | <span data-ttu-id="66099-p113">アイテムが他のユーザーと共有されていることを示し、アイテムの共有状態に関する情報を提供します。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="66099-p113">Indicates that the item has been shared with others and provides information about the shared state of the item. Read-only.</span></span>                                       |
| <span data-ttu-id="66099-163">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="66099-163">sharepointIds</span></span>        | [<span data-ttu-id="66099-164">SharepointIds</span><span class="sxs-lookup"><span data-stu-id="66099-164">SharepointIds</span></span>](sharepointids.md)   | <span data-ttu-id="66099-p114">OneDrive for Business と SharePoint 間の相互運用を、項目識別子の完全なセットと共に提供します。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="66099-p114">Provides interop between items in OneDrive for Business and SharePoint with the full set of item identifiers. Read-only.</span></span>                                          |
| <span data-ttu-id="66099-167">size</span><span class="sxs-lookup"><span data-stu-id="66099-167">size</span></span>                 | <span data-ttu-id="66099-168">Int64</span><span class="sxs-lookup"><span data-stu-id="66099-168">Int64</span></span>                               | <span data-ttu-id="66099-p115">リモート項目のサイズです。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="66099-p115">Size of the remote item. Read-only.</span></span>                                                                                                                               |
| <span data-ttu-id="66099-171">webDavUrl</span><span class="sxs-lookup"><span data-stu-id="66099-171">webDavUrl</span></span>            | <span data-ttu-id="66099-172">Url</span><span class="sxs-lookup"><span data-stu-id="66099-172">Url</span></span>                                 | <span data-ttu-id="66099-173">項目の、DAV 互換性のある URL です。</span><span class="sxs-lookup"><span data-stu-id="66099-173">DAV compatible URL for the item.</span></span>                                                                                                                                  |
| <span data-ttu-id="66099-174">webUrl</span><span class="sxs-lookup"><span data-stu-id="66099-174">webUrl</span></span>               | <span data-ttu-id="66099-175">URL</span><span class="sxs-lookup"><span data-stu-id="66099-175">Url</span></span>                                 | <span data-ttu-id="66099-p116">ブラウザーでリソースを表示するための URL。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="66099-p116">URL that displays the resource in the browser. Read-only.</span></span>                                                                                                         |

## <a name="remarks"></a><span data-ttu-id="66099-178">備考</span><span class="sxs-lookup"><span data-stu-id="66099-178">Remarks</span></span>

<span data-ttu-id="66099-179">**driveItem** のファセットに関する詳細については、「[driveItem](driveitem.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="66099-179">For more information about the facets on a **driveItem**, see [driveItem](driveitem.md).</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "The quota facet provides information about how much space the OneDrive has available.",
  "keywords": "quota,available,remaining,used",
  "section": "documentation",
  "tocPath": "Facets/RemoteItem",
  "suppressions": []
}
-->
