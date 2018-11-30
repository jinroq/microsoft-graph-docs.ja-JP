---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Hashes
ms.openlocfilehash: 2387af83450f667aa4732cc46d7d3cf2111579f0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27066773"
---
# <a name="hashes-resource-type"></a><span data-ttu-id="35233-102">Hashes リソース型</span><span class="sxs-lookup"><span data-stu-id="35233-102">Hashes resource type</span></span>

> <span data-ttu-id="35233-103">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="35233-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="35233-104">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="35233-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="35233-105"> *\*ハッシュ** リソースは、利用可能なハッシュをアイテムの 1 つの構造にグループ化します。</span><span class="sxs-lookup"><span data-stu-id="35233-105">The **Hashes** resource groups available hashes into a single structure for an item.</span></span>

<span data-ttu-id="35233-106">**注:** すべてのサービスで、表示されているすべてのハッシュ プロパティに対して値が指定されているわけではありません。</span><span class="sxs-lookup"><span data-stu-id="35233-106">**Note:** Not all services provide a value for all hash properties listed.</span></span>

## <a name="json-representation"></a><span data-ttu-id="35233-107">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="35233-107">JSON representation</span></span>

<span data-ttu-id="35233-108">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="35233-108">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="35233-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="35233-109">Properties</span></span>

| <span data-ttu-id="35233-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="35233-110">Property</span></span>         | <span data-ttu-id="35233-111">型</span><span class="sxs-lookup"><span data-stu-id="35233-111">Type</span></span>   | <span data-ttu-id="35233-112">説明</span><span class="sxs-lookup"><span data-stu-id="35233-112">Description</span></span>                                                       |
|:-----------------|:-------|:------------------------------------------------------------------|
| <span data-ttu-id="35233-113">**sha1Hash**</span><span class="sxs-lookup"><span data-stu-id="35233-113">**sha1Hash**</span></span>     | <span data-ttu-id="35233-114">String</span><span class="sxs-lookup"><span data-stu-id="35233-114">String</span></span> | <span data-ttu-id="35233-p102">ファイルの内容の SHA1 ハッシュ (使用可能な場合)。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="35233-p102">SHA1 hash for the contents of the file (if available). Read-only.</span></span> |
| <span data-ttu-id="35233-117">**crc32Hash**</span><span class="sxs-lookup"><span data-stu-id="35233-117">**crc32Hash**</span></span>    | <span data-ttu-id="35233-118">String</span><span class="sxs-lookup"><span data-stu-id="35233-118">String</span></span> | <span data-ttu-id="35233-p103">ファイルの CRC32 の値 (使用可能な場合)。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="35233-p103">The CRC32 value of the file (if available). Read-only.</span></span>            |
| <span data-ttu-id="35233-121">**quickXorHash**</span><span class="sxs-lookup"><span data-stu-id="35233-121">**quickXorHash**</span></span> | <span data-ttu-id="35233-122">String</span><span class="sxs-lookup"><span data-stu-id="35233-122">String</span></span> | <span data-ttu-id="35233-p104">ファイルの内容が変更されているかどうかの判別に使用できるファイルの専用ハッシュ (使用可能な場合)。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="35233-p104">A proprietary hash of the file that can be used to determine if the contents of the file have changed (if available). Read-only.</span></span> |

<span data-ttu-id="35233-p105">**注:** ハッシュ値が使用可能ではない場合があります。その場合、アイテムのハッシュ値は、アイテムがダウンロードされた後に更新されます。</span><span class="sxs-lookup"><span data-stu-id="35233-p105">**Note:** In some cases hash values may not be available. If this is the case, the hash values on an item will be updated after the item is downloaded.</span></span>

## <a name="remarks"></a><span data-ttu-id="35233-127">注釈</span><span class="sxs-lookup"><span data-stu-id="35233-127">Remarks</span></span>

<span data-ttu-id="35233-128">OneDrive for Business および SharePoint Server 2016 では、**sha1Hash** と **crc32Hash** は利用できません。</span><span class="sxs-lookup"><span data-stu-id="35233-128">In OneDrive for Business and SharePoint Server 2016, **sha1Hash** and **crc32Hash** are not available.</span></span>

<span data-ttu-id="35233-129">OneDrive 個人用では、**quickXorHash** は利用できません。</span><span class="sxs-lookup"><span data-stu-id="35233-129">In OneDrive Personal, **quickXorHash** is not available.</span></span>

<span data-ttu-id="35233-130">ファイルに対する **quickXorHash** を計算する場合は、[QuickXorHash スニペット](https://dev.onedrive.com/snippets/quickxorhash.htm)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="35233-130">To calculate **quickXorHash** for a file, refer to the [QuickXorHash snippet](https://dev.onedrive.com/snippets/quickxorhash.htm).</span></span>

<span data-ttu-id="35233-131">DriveItem のファセットの詳細については、「[DriveItem](driveitem.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="35233-131">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>


<!-- {
  "type": "#page.annotation",
  "description": "The hashes facet provides hash identifiers for a file in OneDrive",
  "keywords": "hash,sha1,crc32,item,facet",
  "section": "documentation",
  "tocPath": "Facets/Hashes"
} -->
