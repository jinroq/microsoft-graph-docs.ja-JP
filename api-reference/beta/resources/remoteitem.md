---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: RemoteItem
localization_priority: Normal
ms.openlocfilehash: 13eb7ff286467a7acfef85f58ea59763a13d9801
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29514335"
---
# <a name="remoteitem-resource-type"></a><span data-ttu-id="f5616-102">RemoteItem リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f5616-102">RemoteItem resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f5616-p101">remoteItem リソースは、driveItem が別のドライブに存在するアイテムを参照することを示します。このリソースは、ソース ドライブとターゲット項目の固有 ID を提供します。</span><span class="sxs-lookup"><span data-stu-id="f5616-p101">The **remoteItem** resource indicates that a [**driveItem**](driveitem.md) references an item that exists in another drive. This resource provides the unique IDs of the source drive and target item.</span></span>

<span data-ttu-id="f5616-105">非 null の **remoteItem** ファセットを持つ [**DriveItems**](driveitem.md)は、共有された、ユーザーの OneDrive に追加された、あるいは異質な項目のコレクション (検索結果など) から返される項目上にあるリソースです。</span><span class="sxs-lookup"><span data-stu-id="f5616-105">[**DriveItems**](driveitem.md) with a non-null **remoteItem** facet are resources that are shared, added to the user's OneDrive, or on items returned from hetrogenous collections of items (like search results).</span></span>

<span data-ttu-id="f5616-106">**注:** 同じドライブにあるフォルダーとは異なり、リモート アイテムに移動された **driveItem** では、`id` 値が変更された可能性があります。</span><span class="sxs-lookup"><span data-stu-id="f5616-106">**Note:** Unlike with folders in the same drive, a **driveItem** moved into a remote item may have its `id` value changed.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f5616-107">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f5616-107">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="f5616-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f5616-108">Properties</span></span>

| <span data-ttu-id="f5616-109">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="f5616-109">Property name</span></span>        | <span data-ttu-id="f5616-110">種類</span><span class="sxs-lookup"><span data-stu-id="f5616-110">Type</span></span>                                | <span data-ttu-id="f5616-111">説明</span><span class="sxs-lookup"><span data-stu-id="f5616-111">Description</span></span>                                                                                                                                                       |
| :------------------- | :---------------------------------- | :---------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="f5616-112">createdBy</span><span class="sxs-lookup"><span data-stu-id="f5616-112">createdBy</span></span>            | [<span data-ttu-id="f5616-113">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="f5616-113">IdentitySet</span></span>](identityset.md)       | <span data-ttu-id="f5616-p102">その項目を作成したユーザー、デバイス、およびアプリケーションの ID。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="f5616-p102">Identity of the user, device, and application which created the item. Read-only.</span></span>                                                                                  |
| <span data-ttu-id="f5616-116">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f5616-116">createdDateTime</span></span>      | <span data-ttu-id="f5616-117">Timestamp</span><span class="sxs-lookup"><span data-stu-id="f5616-117">Timestamp</span></span>                           | <span data-ttu-id="f5616-p103">項目作成の日付と時刻。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="f5616-p103">Date and time of item creation. Read-only.</span></span>                                                                                                                        |
| <span data-ttu-id="f5616-120">file</span><span class="sxs-lookup"><span data-stu-id="f5616-120">file</span></span>                 | [<span data-ttu-id="f5616-121">File</span><span class="sxs-lookup"><span data-stu-id="f5616-121">File</span></span>](file.md)                     | <span data-ttu-id="f5616-p104">リモート項目がファイルであることを示します。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="f5616-p104">Indicates that the remote item is a file. Read-only.</span></span>                                                                                                              |
| <span data-ttu-id="f5616-124">fileSystemInfo</span><span class="sxs-lookup"><span data-stu-id="f5616-124">fileSystemInfo</span></span>       | [<span data-ttu-id="f5616-125">FileSystemInfo</span><span class="sxs-lookup"><span data-stu-id="f5616-125">FileSystemInfo</span></span>](filesysteminfo.md) | <span data-ttu-id="f5616-p105">ローカル ファイル システムからのリモート項目についての情報。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="f5616-p105">Information about the remote item from the local file system. Read-only.</span></span>                                                                                          |
| <span data-ttu-id="f5616-128">folder</span><span class="sxs-lookup"><span data-stu-id="f5616-128">folder</span></span>               | [<span data-ttu-id="f5616-129">Folder</span><span class="sxs-lookup"><span data-stu-id="f5616-129">Folder</span></span>](folder.md)                 | <span data-ttu-id="f5616-p106">リモート項目がフォルダーであることを示します。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="f5616-p106">Indicates that the remote item is a folder. Read-only.</span></span>                                                                                                            |
| <span data-ttu-id="f5616-132">id</span><span class="sxs-lookup"><span data-stu-id="f5616-132">id</span></span>                   | <span data-ttu-id="f5616-133">String</span><span class="sxs-lookup"><span data-stu-id="f5616-133">String</span></span>                              | <span data-ttu-id="f5616-p107">ドライブ内のリモート項目の固有識別子です。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="f5616-p107">Unique identifier for the remote item in its drive. Read-only.</span></span>                                                                                                    |
| <span data-ttu-id="f5616-136">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="f5616-136">lastModifiedBy</span></span>       | [<span data-ttu-id="f5616-137">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="f5616-137">IdentitySet</span></span>](identityset.md)       | <span data-ttu-id="f5616-p108">最後にその項目を修正したユーザー、デバイス、およびアプリケーションの ID。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="f5616-p108">Identity of the user, device, and application which last modified the item. Read-only.</span></span>                                                                            |
| <span data-ttu-id="f5616-140">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f5616-140">lastModifiedDateTime</span></span> | <span data-ttu-id="f5616-141">Timestamp</span><span class="sxs-lookup"><span data-stu-id="f5616-141">Timestamp</span></span>                           | <span data-ttu-id="f5616-p109">アイテムが最後に変更された日時。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="f5616-p109">Date and time the item was last modified. Read-only.</span></span>                                                                                                              |
| <span data-ttu-id="f5616-144">name</span><span class="sxs-lookup"><span data-stu-id="f5616-144">name</span></span>                 | <span data-ttu-id="f5616-145">String</span><span class="sxs-lookup"><span data-stu-id="f5616-145">String</span></span>                              | <span data-ttu-id="f5616-p110">省略可能。リモート項目のファイル名です。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="f5616-p110">Optional. Filename of the remote item. Read-only.</span></span>                                                                                                                 |
| <span data-ttu-id="f5616-149">package</span><span class="sxs-lookup"><span data-stu-id="f5616-149">package</span></span>              | [<span data-ttu-id="f5616-150">Package</span><span class="sxs-lookup"><span data-stu-id="f5616-150">Package</span></span>](package.md)               | <span data-ttu-id="f5616-p111">存在する場合、この項目がフォルダーやファイルではなくパッケージであることを示します。パッケージは、一部のコンテキストでのファイルのように、他のコンテキストではフォルダーのように扱われます。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="f5616-p111">If present, indicates that this item is a package instead of a folder or file. Packages are treated like files in some contexts and folders in others. Read-only.</span></span> |
| <span data-ttu-id="f5616-154">parentReference</span><span class="sxs-lookup"><span data-stu-id="f5616-154">parentReference</span></span>      | [<span data-ttu-id="f5616-155">ItemReference</span><span class="sxs-lookup"><span data-stu-id="f5616-155">ItemReference</span></span>](itemreference.md)   | <span data-ttu-id="f5616-p112">リモート項目の親のプロパティです。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="f5616-p112">Properties of the parent of the remote item. Read-only.</span></span>                                                                                                           |
| <span data-ttu-id="f5616-158">shared</span><span class="sxs-lookup"><span data-stu-id="f5616-158">shared</span></span>               | [<span data-ttu-id="f5616-159">shared</span><span class="sxs-lookup"><span data-stu-id="f5616-159">shared</span></span>](shared.md)                 | <span data-ttu-id="f5616-p113">アイテムが他のユーザーと共有されていることを示し、アイテムの共有状態に関する情報を提供します。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="f5616-p113">Indicates that the item has been shared with others and provides information about the shared state of the item. Read-only.</span></span>                                       |
| <span data-ttu-id="f5616-162">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="f5616-162">sharepointIds</span></span>        | [<span data-ttu-id="f5616-163">SharepointIds</span><span class="sxs-lookup"><span data-stu-id="f5616-163">SharepointIds</span></span>](sharepointids.md)   | <span data-ttu-id="f5616-p114">OneDrive for Business と SharePoint 間の相互運用を、項目識別子の完全なセットと共に提供します。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="f5616-p114">Provides interop between items in OneDrive for Business and SharePoint with the full set of item identifiers. Read-only.</span></span>                                          |
| <span data-ttu-id="f5616-166">size</span><span class="sxs-lookup"><span data-stu-id="f5616-166">size</span></span>                 | <span data-ttu-id="f5616-167">Int64</span><span class="sxs-lookup"><span data-stu-id="f5616-167">Int64</span></span>                               | <span data-ttu-id="f5616-p115">リモート項目のサイズです。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="f5616-p115">Size of the remote item. Read-only.</span></span>                                                                                                                               |
| <span data-ttu-id="f5616-170">webDavUrl</span><span class="sxs-lookup"><span data-stu-id="f5616-170">webDavUrl</span></span>            | <span data-ttu-id="f5616-171">Url</span><span class="sxs-lookup"><span data-stu-id="f5616-171">Url</span></span>                                 | <span data-ttu-id="f5616-172">項目の、DAV 互換性のある URL です。</span><span class="sxs-lookup"><span data-stu-id="f5616-172">DAV compatible URL for the item.</span></span>                                                                                                                                  |
| <span data-ttu-id="f5616-173">webUrl</span><span class="sxs-lookup"><span data-stu-id="f5616-173">webUrl</span></span>               | <span data-ttu-id="f5616-174">URL</span><span class="sxs-lookup"><span data-stu-id="f5616-174">Url</span></span>                                 | <span data-ttu-id="f5616-p116">ブラウザーでリソースを表示するための URL。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="f5616-p116">URL that displays the resource in the browser. Read-only.</span></span>                                                                                                         |

## <a name="remarks"></a><span data-ttu-id="f5616-177">備考</span><span class="sxs-lookup"><span data-stu-id="f5616-177">Remarks</span></span>

<span data-ttu-id="f5616-178">**driveItem** のファセットに関する詳細については、「[driveItem](driveitem.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f5616-178">For more information about the facets on a **driveItem**, see [driveItem](driveitem.md).</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "The quota facet provides information about how much space the OneDrive has available.",
  "keywords": "quota,available,remaining,used",
  "section": "documentation",
  "tocPath": "Facets/RemoteItem",
  "suppressions": [
    "Error: /api-reference/beta/resources/remoteitem.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
