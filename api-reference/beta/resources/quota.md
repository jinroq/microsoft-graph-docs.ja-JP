---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: クォータ
localization_priority: Normal
ms.openlocfilehash: 7cafff3162c7cdc4435df1cde522b42998398693
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/08/2019
ms.locfileid: "30480307"
---
# <a name="quota-resource-type"></a><span data-ttu-id="4c0df-102">クォータリソースの種類</span><span class="sxs-lookup"><span data-stu-id="4c0df-102">quota resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4c0df-103">**クォータ**リソースは、[ドライブ](drive.md)リソースの領域の制約に関する詳細を提供します。</span><span class="sxs-lookup"><span data-stu-id="4c0df-103">The **quota** resource provides details about space constrains on a [drive](drive.md) resource.</span></span>

## <a name="json-representation"></a><span data-ttu-id="4c0df-104">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="4c0df-104">JSON representation</span></span>

<span data-ttu-id="4c0df-105">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="4c0df-105">Here is a JSON representation of the resource.</span></span>

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
  "storagePlanInformation": {
    "upgradeAvailable": true
  },
  "total": 1024,
  "used": 1024
}
```

## <a name="properties"></a><span data-ttu-id="4c0df-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4c0df-106">Properties</span></span>

| <span data-ttu-id="4c0df-107">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="4c0df-107">Property name</span></span> | <span data-ttu-id="4c0df-108">種類</span><span class="sxs-lookup"><span data-stu-id="4c0df-108">Type</span></span>   | <span data-ttu-id="4c0df-109">説明</span><span class="sxs-lookup"><span data-stu-id="4c0df-109">Description</span></span>                                                                 |
|:--------------|:-------|:----------------------------------------------------------------------------|
| <span data-ttu-id="4c0df-110">total</span><span class="sxs-lookup"><span data-stu-id="4c0df-110">total</span></span>         | <span data-ttu-id="4c0df-111">Int64</span><span class="sxs-lookup"><span data-stu-id="4c0df-111">Int64</span></span>  | <span data-ttu-id="4c0df-p101">許可されている記憶域の合計 (バイト単位)。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="4c0df-p101">Total allowed storage space, in bytes. Read-only.</span></span>                           |
| <span data-ttu-id="4c0df-114">used</span><span class="sxs-lookup"><span data-stu-id="4c0df-114">used</span></span>          | <span data-ttu-id="4c0df-115">Int64</span><span class="sxs-lookup"><span data-stu-id="4c0df-115">Int64</span></span>  | <span data-ttu-id="4c0df-p102">使用領域の合計 (バイト単位)。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="4c0df-p102">Total space used, in bytes. Read-only.</span></span>                                      |
| <span data-ttu-id="4c0df-118">remaining</span><span class="sxs-lookup"><span data-stu-id="4c0df-118">remaining</span></span>     | <span data-ttu-id="4c0df-119">Int64</span><span class="sxs-lookup"><span data-stu-id="4c0df-119">Int64</span></span>  | <span data-ttu-id="4c0df-p103">クォータ制限に達するまでの残りの領域の合計 (バイト単位)。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="4c0df-p103">Total space remaining before reaching the quota limit, in bytes. Read-only.</span></span> |
| <span data-ttu-id="4c0df-122">deleted</span><span class="sxs-lookup"><span data-stu-id="4c0df-122">deleted</span></span>       | <span data-ttu-id="4c0df-123">Int64</span><span class="sxs-lookup"><span data-stu-id="4c0df-123">Int64</span></span>  | <span data-ttu-id="4c0df-p104">ごみ箱内のファイルによって消費されている領域の合計 (バイト単位)。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="4c0df-p104">Total space consumed by files in the recycle bin, in bytes. Read-only.</span></span>      |
| <span data-ttu-id="4c0df-126">state</span><span class="sxs-lookup"><span data-stu-id="4c0df-126">state</span></span>         | <span data-ttu-id="4c0df-127">string</span><span class="sxs-lookup"><span data-stu-id="4c0df-127">string</span></span> | <span data-ttu-id="4c0df-p105">記憶域の状態を示す列挙値。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="4c0df-p105">Enumeration value that indicates the state of the storage space. Read-only.</span></span> |
| <span data-ttu-id="4c0df-130">storagePlanInformation</span><span class="sxs-lookup"><span data-stu-id="4c0df-130">storagePlanInformation</span></span>  | [<span data-ttu-id="4c0df-131">storagePlanInformation</span><span class="sxs-lookup"><span data-stu-id="4c0df-131">storagePlanInformation</span></span>](storageplaninformation.md) | <span data-ttu-id="4c0df-132">ドライブの記憶域クォータプランに関する情報。</span><span class="sxs-lookup"><span data-stu-id="4c0df-132">Information about the drive's storage quota plans.</span></span> <span data-ttu-id="4c0df-133">個人用の OneDrive のみ</span><span class="sxs-lookup"><span data-stu-id="4c0df-133">Only in Personal OneDrive.</span></span>|

### <a name="state-enumeration-values"></a><span data-ttu-id="4c0df-134">状態列挙値</span><span class="sxs-lookup"><span data-stu-id="4c0df-134">State enumeration values</span></span>

| <span data-ttu-id="4c0df-135">値</span><span class="sxs-lookup"><span data-stu-id="4c0df-135">Value</span></span>      | <span data-ttu-id="4c0df-136">説明</span><span class="sxs-lookup"><span data-stu-id="4c0df-136">Description</span></span>                                                                                                                                                                 |
|:-----------|:----------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| `normal`   | <span data-ttu-id="4c0df-137">ドライブに十分なクォータが残っています。</span><span class="sxs-lookup"><span data-stu-id="4c0df-137">The drive has plenty of remaining quota left.</span></span>                                                                                                                               |
| `nearing`  | <span data-ttu-id="4c0df-138">残りのクォータは、クォータ領域の合計の 10% 未満です。</span><span class="sxs-lookup"><span data-stu-id="4c0df-138">Remaining quota is less than 10% of total quota space.</span></span>                                                                                                                      |
| `critical` | <span data-ttu-id="4c0df-139">残りのクォータは、クォータ領域の合計の 1% 未満です。</span><span class="sxs-lookup"><span data-stu-id="4c0df-139">Remaining quota is less than 1% of total quota space.</span></span>                                                                                                                       |
| `exceeded` | <span data-ttu-id="4c0df-p107">クォータ使用量が、クォータの合計を超えています。クォータの合計を下回るか、追加の記憶領域を購入するまで、新しいファイルまたはフォルダーをドライブに追加することはできません。</span><span class="sxs-lookup"><span data-stu-id="4c0df-p107">The used quota has exceeded the total quota. New files or folders cannot be added to the drive until it is under the total quota amount or more storage space is purchased.</span></span> |

<!--
{
  "type": "#page.annotation",
  "description": "The quota facet provides information about how much space the OneDrive has available.",
  "keywords": "quota,available,remaining,used",
  "section": "documentation",
  "tocPath": "Facets/Quota",
  "suppressions": [
    "Error: /api-reference/beta/resources/quota.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
