---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: クォータ
localization_priority: Normal
ms.openlocfilehash: a9a5da54aeef3c9666c22c7a2f9bc0d92fc7a405
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/08/2019
ms.locfileid: "30481455"
---
# <a name="quota-resource-type"></a><span data-ttu-id="13c8b-102">クォータ リソースの種類</span><span class="sxs-lookup"><span data-stu-id="13c8b-102">Quota resource type</span></span>

<span data-ttu-id="13c8b-103">**クォータ** リソースは、[ドライブ](drive.md) リソースの領域の制約に関する詳細を提供します。</span><span class="sxs-lookup"><span data-stu-id="13c8b-103">The **quota** resource provides details about space constrains on a [Drive](drive.md) resource.</span></span>

## <a name="json-representation"></a><span data-ttu-id="13c8b-104">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="13c8b-104">JSON representation</span></span>

<span data-ttu-id="13c8b-105">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="13c8b-105">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@odata.type": "microsoft.graph.quota"
}-->

```json
{
  "deleted": 1024,
  "remaining": 1024,
  "state": "normal | nearing | critical | exceeded",
  "total": 1024,
  "used": 1024
}
```

## <a name="properties"></a><span data-ttu-id="13c8b-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="13c8b-106">Properties</span></span>

| <span data-ttu-id="13c8b-107">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="13c8b-107">Property name</span></span> | <span data-ttu-id="13c8b-108">種類</span><span class="sxs-lookup"><span data-stu-id="13c8b-108">Type</span></span>   | <span data-ttu-id="13c8b-109">説明</span><span class="sxs-lookup"><span data-stu-id="13c8b-109">Description</span></span>                                                                 |
|:--------------|:-------|:----------------------------------------------------------------------------|
| <span data-ttu-id="13c8b-110">total</span><span class="sxs-lookup"><span data-stu-id="13c8b-110">total</span></span>         | <span data-ttu-id="13c8b-111">Int64</span><span class="sxs-lookup"><span data-stu-id="13c8b-111">Int64</span></span>  | <span data-ttu-id="13c8b-p101">許可されている記憶域の合計 (バイト単位)。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="13c8b-p101">Total allowed storage space, in bytes. Read-only.</span></span>                           |
| <span data-ttu-id="13c8b-114">used</span><span class="sxs-lookup"><span data-stu-id="13c8b-114">used</span></span>          | <span data-ttu-id="13c8b-115">Int64</span><span class="sxs-lookup"><span data-stu-id="13c8b-115">Int64</span></span>  | <span data-ttu-id="13c8b-p102">使用領域の合計 (バイト単位)。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="13c8b-p102">Total space used, in bytes. Read-only.</span></span>                                      |
| <span data-ttu-id="13c8b-118">remaining</span><span class="sxs-lookup"><span data-stu-id="13c8b-118">remaining</span></span>     | <span data-ttu-id="13c8b-119">Int64</span><span class="sxs-lookup"><span data-stu-id="13c8b-119">Int64</span></span>  | <span data-ttu-id="13c8b-p103">クォータ制限に達するまでの残りの領域の合計 (バイト単位)。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="13c8b-p103">Total space remaining before reaching the quota limit, in bytes. Read-only.</span></span> |
| <span data-ttu-id="13c8b-122">deleted</span><span class="sxs-lookup"><span data-stu-id="13c8b-122">deleted</span></span>       | <span data-ttu-id="13c8b-123">Int64</span><span class="sxs-lookup"><span data-stu-id="13c8b-123">Int64</span></span>  | <span data-ttu-id="13c8b-p104">ごみ箱内のファイルによって消費されている領域の合計 (バイト単位)。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="13c8b-p104">Total space consumed by files in the recycle bin, in bytes. Read-only.</span></span>      |
| <span data-ttu-id="13c8b-126">state</span><span class="sxs-lookup"><span data-stu-id="13c8b-126">state</span></span>         | <span data-ttu-id="13c8b-127">string</span><span class="sxs-lookup"><span data-stu-id="13c8b-127">string</span></span> | <span data-ttu-id="13c8b-p105">記憶域の状態を示す列挙値。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="13c8b-p105">Enumeration value that indicates the state of the storage space. Read-only.</span></span> |

## <a name="state-enumeration"></a><span data-ttu-id="13c8b-130">状態の列挙値</span><span class="sxs-lookup"><span data-stu-id="13c8b-130">State Enumeration</span></span>

| <span data-ttu-id="13c8b-131">値</span><span class="sxs-lookup"><span data-stu-id="13c8b-131">Value</span></span>      | <span data-ttu-id="13c8b-132">説明</span><span class="sxs-lookup"><span data-stu-id="13c8b-132">Description</span></span>                                                                                                                                                                 |
|:-----------|:----------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| `normal`   | <span data-ttu-id="13c8b-133">ドライブに十分なクォータが残っています。</span><span class="sxs-lookup"><span data-stu-id="13c8b-133">The drive has plenty of remaining quota left.</span></span>                                                                                                                               |
| `nearing`  | <span data-ttu-id="13c8b-134">残りのクォータは、クォータ領域の合計の 10% 未満です。</span><span class="sxs-lookup"><span data-stu-id="13c8b-134">Remaining quota is less than 10% of total quota space.</span></span>                                                                                                                      |
| `critical` | <span data-ttu-id="13c8b-135">残りのクォータは、クォータ領域の合計の 1% 未満です。</span><span class="sxs-lookup"><span data-stu-id="13c8b-135">Remaining quota is less than 1% of total quota space.</span></span>                                                                                                                       |
| `exceeded` | <span data-ttu-id="13c8b-p106">クォータ使用量が、クォータの合計を超えています。クォータの合計を下回るか、追加の記憶領域を購入するまで、新しいファイルまたはフォルダーをドライブに追加することはできません。</span><span class="sxs-lookup"><span data-stu-id="13c8b-p106">The used quota has exceeded the total quota. New files or folders cannot be added to the drive until it is under the total quota amount or more storage space is purchased.</span></span> |

<!-- {
  "type": "#page.annotation",
  "description": "The quota facet provides information about how much space the OneDrive has available.",
  "keywords": "quota,available,remaining,used",
  "section": "documentation",
  "suppressions": [
    "Warning: /api-reference/v1.0/resources/quota.md:
      Found potential enums in resource example that weren't defined in a table:(normal, nearing,critical,exceeded) are in resource, but () are in table"
  ],
  "tocPath": "Facets/Quota"
} -->
