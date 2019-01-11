---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
localization_priority: Normal
ms.openlocfilehash: 3ed0023e80457598bd80b068156b60a5ace4984b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27830486"
---
# <a name="hashes-resource-type"></a><span data-ttu-id="43ddd-101">ハッシュ リソースの種類</span><span class="sxs-lookup"><span data-stu-id="43ddd-101">Hashes resource type</span></span>

<span data-ttu-id="43ddd-102"> *\*ハッシュ** リソースは、利用可能なハッシュをアイテムの 1 つの構造にグループ化します。</span><span class="sxs-lookup"><span data-stu-id="43ddd-102">The **Hashes** resource groups available hashes into a single structure for an item.</span></span>

<span data-ttu-id="43ddd-103">**注:** すべてのサービスで、表示されているすべてのハッシュ プロパティに対して値が指定されているわけではありません。</span><span class="sxs-lookup"><span data-stu-id="43ddd-103">**Note:** Not all services provide a value for all hash properties listed.</span></span>

## <a name="json-representation"></a><span data-ttu-id="43ddd-104">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="43ddd-104">JSON representation</span></span>

<span data-ttu-id="43ddd-105">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="43ddd-105">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="43ddd-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="43ddd-106">Properties</span></span>

| <span data-ttu-id="43ddd-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="43ddd-107">Property</span></span>         | <span data-ttu-id="43ddd-108">種類</span><span class="sxs-lookup"><span data-stu-id="43ddd-108">Type</span></span>   | <span data-ttu-id="43ddd-109">説明</span><span class="sxs-lookup"><span data-stu-id="43ddd-109">Description</span></span>                                                       |
|:-----------------|:-------|:------------------------------------------------------------------|
| <span data-ttu-id="43ddd-110">**sha1Hash**</span><span class="sxs-lookup"><span data-stu-id="43ddd-110">**sha1Hash**</span></span>     | <span data-ttu-id="43ddd-111">String</span><span class="sxs-lookup"><span data-stu-id="43ddd-111">String</span></span> | <span data-ttu-id="43ddd-p101">ファイルの内容の SHA1 ハッシュ (使用可能な場合)。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="43ddd-p101">SHA1 hash for the contents of the file (if available). Read-only.</span></span> |
| <span data-ttu-id="43ddd-114">**crc32Hash**</span><span class="sxs-lookup"><span data-stu-id="43ddd-114">**crc32Hash**</span></span>    | <span data-ttu-id="43ddd-115">String</span><span class="sxs-lookup"><span data-stu-id="43ddd-115">String</span></span> | <span data-ttu-id="43ddd-116">リトルエンディアン (ある場合) 内のファイルの CRC32 の値です。</span><span class="sxs-lookup"><span data-stu-id="43ddd-116">The CRC32 value of the file in little endian (if available).</span></span> <span data-ttu-id="43ddd-117">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="43ddd-117">Read-only.</span></span>            |
| <span data-ttu-id="43ddd-118">**quickXorHash**</span><span class="sxs-lookup"><span data-stu-id="43ddd-118">**quickXorHash**</span></span> | <span data-ttu-id="43ddd-119">String</span><span class="sxs-lookup"><span data-stu-id="43ddd-119">String</span></span> | <span data-ttu-id="43ddd-p103">ファイルの内容が変更されているかどうかの判別に使用できるファイルの専用ハッシュ (使用可能な場合)。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="43ddd-p103">A proprietary hash of the file that can be used to determine if the contents of the file have changed (if available). Read-only.</span></span> |

<span data-ttu-id="43ddd-p104">**注:** ハッシュ値が使用可能ではない場合があります。その場合、アイテムのハッシュ値は、アイテムがダウンロードされた後に更新されます。</span><span class="sxs-lookup"><span data-stu-id="43ddd-p104">**Note:** In some cases hash values may not be available. If this is the case, the hash values on an item will be updated after the item is downloaded.</span></span>

## <a name="remarks"></a><span data-ttu-id="43ddd-124">注釈</span><span class="sxs-lookup"><span data-stu-id="43ddd-124">Remarks</span></span>

<span data-ttu-id="43ddd-125">OneDrive for Business および SharePoint Server 2016 では、**sha1Hash** と **crc32Hash** は利用できません。</span><span class="sxs-lookup"><span data-stu-id="43ddd-125">In OneDrive for Business and SharePoint Server 2016, **sha1Hash** and **crc32Hash** are not available.</span></span>

<span data-ttu-id="43ddd-126">OneDrive 個人用では、**quickXorHash** は利用できません。</span><span class="sxs-lookup"><span data-stu-id="43ddd-126">In OneDrive Personal, **quickXorHash** is not available.</span></span>

<span data-ttu-id="43ddd-127">ファイルに対する **quickXorHash** を計算する場合は、[QuickXorHash スニペット](https://dev.onedrive.com/snippets/quickxorhash.htm)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="43ddd-127">To calculate **quickXorHash** for a file, refer to the [QuickXorHash snippet](https://dev.onedrive.com/snippets/quickxorhash.htm).</span></span>
<span data-ttu-id="43ddd-128">DriveItem のファセットの詳細については、「[DriveItem](driveitem.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="43ddd-128">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>


<!-- {
  "type": "#page.annotation",
  "description": "The hashes facet provides hash identifiers for a file in OneDrive",
  "keywords": "hash,sha1,crc32,item,facet",
  "section": "documentation",
  "tocPath": "Facets/Hashes"
} -->
