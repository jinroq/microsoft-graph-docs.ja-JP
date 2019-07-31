---
author: JeremyKelley
description: ハッシュ リソースは、利用可能なハッシュをアイテムの 1 つの構造にグループ化します。
ms.date: 09/10/2017
title: 方向性
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: e2e61e6fbc5e6ff92c91eb2ffd408e6d4c7c41c0
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36006396"
---
# <a name="hashes-resource-type"></a><span data-ttu-id="100b7-103">Hashes リソース型</span><span class="sxs-lookup"><span data-stu-id="100b7-103">Hashes resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="100b7-104"> **ハッシュ** リソースは、利用可能なハッシュをアイテムの 1 つの構造にグループ化します。</span><span class="sxs-lookup"><span data-stu-id="100b7-104">The **Hashes** resource groups available hashes into a single structure for an item.</span></span>

<span data-ttu-id="100b7-105">**注:** すべてのサービスで、表示されているすべてのハッシュ プロパティに対して値が指定されているわけではありません。</span><span class="sxs-lookup"><span data-stu-id="100b7-105">**Note:** Not all services provide a value for all hash properties listed.</span></span>

## <a name="json-representation"></a><span data-ttu-id="100b7-106">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="100b7-106">JSON representation</span></span>

<span data-ttu-id="100b7-107">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="100b7-107">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="100b7-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="100b7-108">Properties</span></span>

| <span data-ttu-id="100b7-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="100b7-109">Property</span></span>         | <span data-ttu-id="100b7-110">型</span><span class="sxs-lookup"><span data-stu-id="100b7-110">Type</span></span>   | <span data-ttu-id="100b7-111">説明</span><span class="sxs-lookup"><span data-stu-id="100b7-111">Description</span></span>                                                       |
|:-----------------|:-------|:------------------------------------------------------------------|
| <span data-ttu-id="100b7-112">**sha1Hash**</span><span class="sxs-lookup"><span data-stu-id="100b7-112">**sha1Hash**</span></span>     | <span data-ttu-id="100b7-113">String</span><span class="sxs-lookup"><span data-stu-id="100b7-113">String</span></span> | <span data-ttu-id="100b7-p101">ファイルの内容の SHA1 ハッシュ (使用可能な場合)。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="100b7-p101">SHA1 hash for the contents of the file (if available). Read-only.</span></span> |
| <span data-ttu-id="100b7-116">**crc32Hash**</span><span class="sxs-lookup"><span data-stu-id="100b7-116">**crc32Hash**</span></span>    | <span data-ttu-id="100b7-117">String</span><span class="sxs-lookup"><span data-stu-id="100b7-117">String</span></span> | <span data-ttu-id="100b7-p102">ファイルの CRC32 の値 (使用可能な場合)。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="100b7-p102">The CRC32 value of the file (if available). Read-only.</span></span>            |
| <span data-ttu-id="100b7-120">**quickXorHash**</span><span class="sxs-lookup"><span data-stu-id="100b7-120">**quickXorHash**</span></span> | <span data-ttu-id="100b7-121">String</span><span class="sxs-lookup"><span data-stu-id="100b7-121">String</span></span> | <span data-ttu-id="100b7-p103">ファイルの内容が変更されているかどうかの判別に使用できるファイルの専用ハッシュ (使用可能な場合)。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="100b7-p103">A proprietary hash of the file that can be used to determine if the contents of the file have changed (if available). Read-only.</span></span> |

<span data-ttu-id="100b7-p104">**注:** ハッシュ値が使用可能ではない場合があります。その場合、アイテムのハッシュ値は、アイテムがダウンロードされた後に更新されます。</span><span class="sxs-lookup"><span data-stu-id="100b7-p104">**Note:** In some cases hash values may not be available. If this is the case, the hash values on an item will be updated after the item is downloaded.</span></span>

## <a name="remarks"></a><span data-ttu-id="100b7-126">備考</span><span class="sxs-lookup"><span data-stu-id="100b7-126">Remarks</span></span>

<span data-ttu-id="100b7-127">OneDrive for Business および SharePoint Server 2016 では、**sha1Hash** と **crc32Hash** は利用できません。</span><span class="sxs-lookup"><span data-stu-id="100b7-127">In OneDrive for Business and SharePoint Server 2016, **sha1Hash** and **crc32Hash** are not available.</span></span>

<span data-ttu-id="100b7-128">OneDrive 個人用では、**quickXorHash** は利用できません。</span><span class="sxs-lookup"><span data-stu-id="100b7-128">In OneDrive Personal, **quickXorHash** is not available.</span></span>

<span data-ttu-id="100b7-129">ファイルに対する **quickXorHash** を計算する場合は、[QuickXorHash スニペット](https://dev.onedrive.com/snippets/quickxorhash.htm)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="100b7-129">To calculate **quickXorHash** for a file, refer to the [QuickXorHash snippet](https://dev.onedrive.com/snippets/quickxorhash.htm).</span></span>

<span data-ttu-id="100b7-130">DriveItem のファセットの詳細については、「[DriveItem](driveitem.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="100b7-130">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>


<!--
{
  "type": "#page.annotation",
  "description": "The hashes facet provides hash identifiers for a file in OneDrive",
  "keywords": "hash,sha1,crc32,item,facet",
  "section": "documentation",
  "tocPath": "Facets/Hashes",
  "suppressions": []
}
-->
