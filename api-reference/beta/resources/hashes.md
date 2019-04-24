---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: 方向性
localization_priority: Normal
ms.openlocfilehash: be7d3b27b1ef22976dc93ea5aecbc2a64031e8b4
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32506350"
---
# <a name="hashes-resource-type"></a><span data-ttu-id="d717b-102">Hashes リソース型</span><span class="sxs-lookup"><span data-stu-id="d717b-102">Hashes resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d717b-103"> *\*ハッシュ** リソースは、利用可能なハッシュをアイテムの 1 つの構造にグループ化します。</span><span class="sxs-lookup"><span data-stu-id="d717b-103">The **Hashes** resource groups available hashes into a single structure for an item.</span></span>

<span data-ttu-id="d717b-104">**注:** すべてのサービスで、表示されているすべてのハッシュ プロパティに対して値が指定されているわけではありません。</span><span class="sxs-lookup"><span data-stu-id="d717b-104">**Note:** Not all services provide a value for all hash properties listed.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d717b-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d717b-105">JSON representation</span></span>

<span data-ttu-id="d717b-106">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="d717b-106">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ "sha1Hash", "crc32Hash", "quickXorHash" ],
  "@odata.type": "microsoft.graph.hashes"
}-->

```json
{
  "crc32Hash": "string (hex)",
  "sha1Hash": "string (hex)",
  "quickXorHash": "string (base64)"
}
```

## <a name="properties"></a><span data-ttu-id="d717b-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d717b-107">Properties</span></span>

| <span data-ttu-id="d717b-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d717b-108">Property</span></span>         | <span data-ttu-id="d717b-109">型</span><span class="sxs-lookup"><span data-stu-id="d717b-109">Type</span></span>   | <span data-ttu-id="d717b-110">説明</span><span class="sxs-lookup"><span data-stu-id="d717b-110">Description</span></span>                                                       |
|:-----------------|:-------|:------------------------------------------------------------------|
| <span data-ttu-id="d717b-111">**sha1Hash**</span><span class="sxs-lookup"><span data-stu-id="d717b-111">**sha1Hash**</span></span>     | <span data-ttu-id="d717b-112">String</span><span class="sxs-lookup"><span data-stu-id="d717b-112">String</span></span> | <span data-ttu-id="d717b-p101">ファイルの内容の SHA1 ハッシュ (使用可能な場合)。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="d717b-p101">SHA1 hash for the contents of the file (if available). Read-only.</span></span> |
| <span data-ttu-id="d717b-115">**crc32Hash**</span><span class="sxs-lookup"><span data-stu-id="d717b-115">**crc32Hash**</span></span>    | <span data-ttu-id="d717b-116">String</span><span class="sxs-lookup"><span data-stu-id="d717b-116">String</span></span> | <span data-ttu-id="d717b-p102">ファイルの CRC32 の値 (使用可能な場合)。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="d717b-p102">The CRC32 value of the file (if available). Read-only.</span></span>            |
| <span data-ttu-id="d717b-119">**quickXorHash**</span><span class="sxs-lookup"><span data-stu-id="d717b-119">**quickXorHash**</span></span> | <span data-ttu-id="d717b-120">String</span><span class="sxs-lookup"><span data-stu-id="d717b-120">String</span></span> | <span data-ttu-id="d717b-p103">ファイルの内容が変更されているかどうかの判別に使用できるファイルの専用ハッシュ (使用可能な場合)。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="d717b-p103">A proprietary hash of the file that can be used to determine if the contents of the file have changed (if available). Read-only.</span></span> |

<span data-ttu-id="d717b-p104">**注:** ハッシュ値が使用可能ではない場合があります。その場合、アイテムのハッシュ値は、アイテムがダウンロードされた後に更新されます。</span><span class="sxs-lookup"><span data-stu-id="d717b-p104">**Note:** In some cases hash values may not be available. If this is the case, the hash values on an item will be updated after the item is downloaded.</span></span>

## <a name="remarks"></a><span data-ttu-id="d717b-125">備考</span><span class="sxs-lookup"><span data-stu-id="d717b-125">Remarks</span></span>

<span data-ttu-id="d717b-126">OneDrive for Business および SharePoint Server 2016 では、**sha1Hash** と **crc32Hash** は利用できません。</span><span class="sxs-lookup"><span data-stu-id="d717b-126">In OneDrive for Business and SharePoint Server 2016, **sha1Hash** and **crc32Hash** are not available.</span></span>

<span data-ttu-id="d717b-127">OneDrive 個人用では、**quickXorHash** は利用できません。</span><span class="sxs-lookup"><span data-stu-id="d717b-127">In OneDrive Personal, **quickXorHash** is not available.</span></span>

<span data-ttu-id="d717b-128">ファイルに対する **quickXorHash** を計算する場合は、[QuickXorHash スニペット](https://dev.onedrive.com/snippets/quickxorhash.htm)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d717b-128">To calculate **quickXorHash** for a file, refer to the [QuickXorHash snippet](https://dev.onedrive.com/snippets/quickxorhash.htm).</span></span>

<span data-ttu-id="d717b-129">DriveItem のファセットの詳細については、「[DriveItem](driveitem.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d717b-129">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>


<!--
{
  "type": "#page.annotation",
  "description": "The hashes facet provides hash identifiers for a file in OneDrive",
  "keywords": "hash,sha1,crc32,item,facet",
  "section": "documentation",
  "tocPath": "Facets/Hashes",
  "suppressions": [
    "Error: /api-reference/beta/resources/hashes.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
