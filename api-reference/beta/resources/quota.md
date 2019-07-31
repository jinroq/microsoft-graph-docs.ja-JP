---
author: JeremyKelley
description: クォータリソースは、ドライブリソースの領域の制約に関する詳細を提供します。
ms.date: 09/10/2017
title: 領域
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 83e842872694a1f708bf37ab800fa73673255647
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36008797"
---
# <a name="quota-resource-type"></a><span data-ttu-id="4d979-103">クォータリソースの種類</span><span class="sxs-lookup"><span data-stu-id="4d979-103">quota resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4d979-104">**クォータ**リソースは、[ドライブ](drive.md)リソースの領域の制約に関する詳細を提供します。</span><span class="sxs-lookup"><span data-stu-id="4d979-104">The **quota** resource provides details about space constrains on a [drive](drive.md) resource.</span></span>

## <a name="json-representation"></a><span data-ttu-id="4d979-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="4d979-105">JSON representation</span></span>

<span data-ttu-id="4d979-106">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="4d979-106">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="4d979-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4d979-107">Properties</span></span>

| <span data-ttu-id="4d979-108">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="4d979-108">Property name</span></span> | <span data-ttu-id="4d979-109">種類</span><span class="sxs-lookup"><span data-stu-id="4d979-109">Type</span></span>   | <span data-ttu-id="4d979-110">説明</span><span class="sxs-lookup"><span data-stu-id="4d979-110">Description</span></span>                                                                 |
|:--------------|:-------|:----------------------------------------------------------------------------|
| <span data-ttu-id="4d979-111">total</span><span class="sxs-lookup"><span data-stu-id="4d979-111">total</span></span>         | <span data-ttu-id="4d979-112">Int64</span><span class="sxs-lookup"><span data-stu-id="4d979-112">Int64</span></span>  | <span data-ttu-id="4d979-p101">許可されている記憶域の合計 (バイト単位)。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="4d979-p101">Total allowed storage space, in bytes. Read-only.</span></span>                           |
| <span data-ttu-id="4d979-115">used</span><span class="sxs-lookup"><span data-stu-id="4d979-115">used</span></span>          | <span data-ttu-id="4d979-116">Int64</span><span class="sxs-lookup"><span data-stu-id="4d979-116">Int64</span></span>  | <span data-ttu-id="4d979-p102">使用領域の合計 (バイト単位)。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="4d979-p102">Total space used, in bytes. Read-only.</span></span>                                      |
| <span data-ttu-id="4d979-119">remaining</span><span class="sxs-lookup"><span data-stu-id="4d979-119">remaining</span></span>     | <span data-ttu-id="4d979-120">Int64</span><span class="sxs-lookup"><span data-stu-id="4d979-120">Int64</span></span>  | <span data-ttu-id="4d979-p103">クォータ制限に達するまでの残りの領域の合計 (バイト単位)。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="4d979-p103">Total space remaining before reaching the quota limit, in bytes. Read-only.</span></span> |
| <span data-ttu-id="4d979-123">deleted</span><span class="sxs-lookup"><span data-stu-id="4d979-123">deleted</span></span>       | <span data-ttu-id="4d979-124">Int64</span><span class="sxs-lookup"><span data-stu-id="4d979-124">Int64</span></span>  | <span data-ttu-id="4d979-p104">ごみ箱内のファイルによって消費されている領域の合計 (バイト単位)。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="4d979-p104">Total space consumed by files in the recycle bin, in bytes. Read-only.</span></span>      |
| <span data-ttu-id="4d979-127">state</span><span class="sxs-lookup"><span data-stu-id="4d979-127">state</span></span>         | <span data-ttu-id="4d979-128">string</span><span class="sxs-lookup"><span data-stu-id="4d979-128">string</span></span> | <span data-ttu-id="4d979-p105">記憶域の状態を示す列挙値。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="4d979-p105">Enumeration value that indicates the state of the storage space. Read-only.</span></span> |
| <span data-ttu-id="4d979-131">storagePlanInformation</span><span class="sxs-lookup"><span data-stu-id="4d979-131">storagePlanInformation</span></span>  | [<span data-ttu-id="4d979-132">storagePlanInformation</span><span class="sxs-lookup"><span data-stu-id="4d979-132">storagePlanInformation</span></span>](storageplaninformation.md) | <span data-ttu-id="4d979-133">ドライブの記憶域クォータプランに関する情報。</span><span class="sxs-lookup"><span data-stu-id="4d979-133">Information about the drive's storage quota plans.</span></span> <span data-ttu-id="4d979-134">個人用の OneDrive のみ</span><span class="sxs-lookup"><span data-stu-id="4d979-134">Only in Personal OneDrive.</span></span>|

### <a name="state-enumeration-values"></a><span data-ttu-id="4d979-135">状態列挙値</span><span class="sxs-lookup"><span data-stu-id="4d979-135">State enumeration values</span></span>

| <span data-ttu-id="4d979-136">値</span><span class="sxs-lookup"><span data-stu-id="4d979-136">Value</span></span>      | <span data-ttu-id="4d979-137">説明</span><span class="sxs-lookup"><span data-stu-id="4d979-137">Description</span></span>                                                                                                                                                                 |
|:-----------|:----------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| `normal`   | <span data-ttu-id="4d979-138">ドライブに十分なクォータが残っています。</span><span class="sxs-lookup"><span data-stu-id="4d979-138">The drive has plenty of remaining quota left.</span></span>                                                                                                                               |
| `nearing`  | <span data-ttu-id="4d979-139">残りのクォータは、クォータ領域の合計の 10% 未満です。</span><span class="sxs-lookup"><span data-stu-id="4d979-139">Remaining quota is less than 10% of total quota space.</span></span>                                                                                                                      |
| `critical` | <span data-ttu-id="4d979-140">残りのクォータは、クォータ領域の合計の 1% 未満です。</span><span class="sxs-lookup"><span data-stu-id="4d979-140">Remaining quota is less than 1% of total quota space.</span></span>                                                                                                                       |
| `exceeded` | <span data-ttu-id="4d979-p107">クォータ使用量が、クォータの合計を超えています。クォータの合計を下回るか、追加の記憶領域を購入するまで、新しいファイルまたはフォルダーをドライブに追加することはできません。</span><span class="sxs-lookup"><span data-stu-id="4d979-p107">The used quota has exceeded the total quota. New files or folders cannot be added to the drive until it is under the total quota amount or more storage space is purchased.</span></span> |

<!--
{
  "type": "#page.annotation",
  "description": "The quota facet provides information about how much space the OneDrive has available.",
  "keywords": "quota,available,remaining,used",
  "section": "documentation",
  "tocPath": "Facets/Quota",
  "suppressions": []
}
-->
