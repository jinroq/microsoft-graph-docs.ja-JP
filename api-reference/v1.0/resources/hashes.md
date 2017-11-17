---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
ms.openlocfilehash: 9de6923146b915207fc771721d7aeb6767e9f99e
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/28/2017
---
# <a name="hashes-resource-type"></a><span data-ttu-id="d1584-101">ハッシュ リソースの種類</span><span class="sxs-lookup"><span data-stu-id="d1584-101">Hashes resource type</span></span>

<span data-ttu-id="d1584-102"> **ハッシュ** リソースは、利用可能なハッシュをアイテムの 1 つの構造にグループ化します。</span><span class="sxs-lookup"><span data-stu-id="d1584-102">The **Hashes** resource groups available hashes into a single structure for an item.</span></span>

<span data-ttu-id="d1584-103">**注:**すべてのサービスで、表示されているすべてのハッシュ プロパティに対して値が指定されているわけではありません。</span><span class="sxs-lookup"><span data-stu-id="d1584-103">**Note:** Not all services provide a value for all hash properties listed.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d1584-104">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d1584-104">JSON representation</span></span>

<span data-ttu-id="d1584-105">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="d1584-105">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="d1584-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d1584-106">Properties</span></span>

| <span data-ttu-id="d1584-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d1584-107">Property</span></span>         | <span data-ttu-id="d1584-108">型</span><span class="sxs-lookup"><span data-stu-id="d1584-108">Type</span></span>   | <span data-ttu-id="d1584-109">説明</span><span class="sxs-lookup"><span data-stu-id="d1584-109">Description</span></span>                                                       |
|:-----------------|:-------|:------------------------------------------------------------------|
| <span data-ttu-id="d1584-110">**sha1Hash**</span><span class="sxs-lookup"><span data-stu-id="d1584-110">**sha1Hash**</span></span>     | <span data-ttu-id="d1584-111">String</span><span class="sxs-lookup"><span data-stu-id="d1584-111">String</span></span> | <span data-ttu-id="d1584-p101">ファイルの内容の SHA1 ハッシュ (使用可能な場合)。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="d1584-p101">SHA1 hash for the contents of the file (if available). Read-only.</span></span> |
| <span data-ttu-id="d1584-114">**crc32Hash**</span><span class="sxs-lookup"><span data-stu-id="d1584-114">**crc32Hash**</span></span>    | <span data-ttu-id="d1584-115">String</span><span class="sxs-lookup"><span data-stu-id="d1584-115">String</span></span> | <span data-ttu-id="d1584-p102">ファイルの CRC32 の値 (使用可能な場合)。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="d1584-p102">The CRC32 value of the file (if available). Read-only.</span></span>            |
| <span data-ttu-id="d1584-118">**quickXorHash**</span><span class="sxs-lookup"><span data-stu-id="d1584-118">**quickXorHash**</span></span> | <span data-ttu-id="d1584-119">String</span><span class="sxs-lookup"><span data-stu-id="d1584-119">String</span></span> | <span data-ttu-id="d1584-p103">ファイルの内容が変更されているかどうかの判別に使用できるファイルの専用ハッシュ (使用可能な場合)。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="d1584-p103">A proprietary hash of the file that can be used to determine if the contents of the file have changed (if available). Read-only.</span></span> |

<span data-ttu-id="d1584-p104">**注:**ハッシュ値が使用可能ではない場合があります。その場合、アイテムのハッシュ値は、アイテムがダウンロードされた後に更新されます。</span><span class="sxs-lookup"><span data-stu-id="d1584-p104">**Note:** In some cases hash values may not be available. If this is the case, the hash values on an item will be updated after the item is downloaded.</span></span>

## <a name="remarks"></a><span data-ttu-id="d1584-124">注釈</span><span class="sxs-lookup"><span data-stu-id="d1584-124">Remarks</span></span>

<span data-ttu-id="d1584-125">OneDrive for Business および SharePoint Server 2016 では、**sha1Hash** と **crc32Hash** は利用できません。</span><span class="sxs-lookup"><span data-stu-id="d1584-125">In OneDrive for Business and SharePoint Server 2016, **sha1Hash** and **crc32Hash** are not available.</span></span>

<span data-ttu-id="d1584-126">OneDrive 個人用では、**quickXorHash** は利用できません。</span><span class="sxs-lookup"><span data-stu-id="d1584-126">In OneDrive Personal, **quickXorHash** is not available.</span></span>

<span data-ttu-id="d1584-127">ファイルに対する **quickXorHash** を計算する場合は、「[QuickXorHash スニペット](https://dev.onedrive.com/snippets/quickxorhash.htm)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d1584-127">To calculate **quickXorHash** for a file, refer to the [QuickXorHash snippet](https://dev.onedrive.com/snippets/quickxorhash.htm).</span></span>
<span data-ttu-id="d1584-128">DriveItem のファセットの詳細については、「[DriveItem](driveitem.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d1584-128">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>


<!-- {
  "type": "#page.annotation",
  "description": "The hashes facet provides hash identifiers for a file in OneDrive",
  "keywords": "hash,sha1,crc32,item,facet",
  "section": "documentation",
  "tocPath": "Facets/Hashes"
} -->
