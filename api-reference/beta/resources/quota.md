---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Quota
ms.openlocfilehash: f4518021da8ad180b91472feb52199678c2edc83
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27072526"
---
# <a name="quota-resource-type"></a><span data-ttu-id="573b4-102">クォータのリソースの種類</span><span class="sxs-lookup"><span data-stu-id="573b4-102">quota resource type</span></span>

> <span data-ttu-id="573b4-103">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="573b4-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="573b4-104">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="573b4-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="573b4-105">**クォータ**のリソースでは、容量に関する詳細情報を[ドライブ](drive.md)リソースの制約を提供します。</span><span class="sxs-lookup"><span data-stu-id="573b4-105">The **quota** resource provides details about space constrains on a [drive](drive.md) resource.</span></span>

## <a name="json-representation"></a><span data-ttu-id="573b4-106">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="573b4-106">JSON representation</span></span>

<span data-ttu-id="573b4-107">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="573b4-107">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="573b4-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="573b4-108">Properties</span></span>

| <span data-ttu-id="573b4-109">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="573b4-109">Property name</span></span> | <span data-ttu-id="573b4-110">型</span><span class="sxs-lookup"><span data-stu-id="573b4-110">Type</span></span>   | <span data-ttu-id="573b4-111">説明</span><span class="sxs-lookup"><span data-stu-id="573b4-111">Description</span></span>                                                                 |
|:--------------|:-------|:----------------------------------------------------------------------------|
| <span data-ttu-id="573b4-112">total</span><span class="sxs-lookup"><span data-stu-id="573b4-112">total</span></span>         | <span data-ttu-id="573b4-113">Int64</span><span class="sxs-lookup"><span data-stu-id="573b4-113">Int64</span></span>  | <span data-ttu-id="573b4-p102">許可されている記憶域の合計 (バイト単位)。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="573b4-p102">Total allowed storage space, in bytes. Read-only.</span></span>                           |
| <span data-ttu-id="573b4-116">used</span><span class="sxs-lookup"><span data-stu-id="573b4-116">used</span></span>          | <span data-ttu-id="573b4-117">Int64</span><span class="sxs-lookup"><span data-stu-id="573b4-117">Int64</span></span>  | <span data-ttu-id="573b4-p103">使用領域の合計 (バイト単位)。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="573b4-p103">Total space used, in bytes. Read-only.</span></span>                                      |
| <span data-ttu-id="573b4-120">remaining</span><span class="sxs-lookup"><span data-stu-id="573b4-120">remaining</span></span>     | <span data-ttu-id="573b4-121">Int64</span><span class="sxs-lookup"><span data-stu-id="573b4-121">Int64</span></span>  | <span data-ttu-id="573b4-p104">クォータ制限に達するまでの残りの領域の合計 (バイト単位)。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="573b4-p104">Total space remaining before reaching the quota limit, in bytes. Read-only.</span></span> |
| <span data-ttu-id="573b4-124">deleted</span><span class="sxs-lookup"><span data-stu-id="573b4-124">deleted</span></span>       | <span data-ttu-id="573b4-125">Int64</span><span class="sxs-lookup"><span data-stu-id="573b4-125">Int64</span></span>  | <span data-ttu-id="573b4-p105">ごみ箱内のファイルによって消費されている領域の合計 (バイト単位)。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="573b4-p105">Total space consumed by files in the recycle bin, in bytes. Read-only.</span></span>      |
| <span data-ttu-id="573b4-128">state</span><span class="sxs-lookup"><span data-stu-id="573b4-128">state</span></span>         | <span data-ttu-id="573b4-129">文字列</span><span class="sxs-lookup"><span data-stu-id="573b4-129">string</span></span> | <span data-ttu-id="573b4-p106">記憶域の状態を示す列挙値。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="573b4-p106">Enumeration value that indicates the state of the storage space. Read-only.</span></span> |
| <span data-ttu-id="573b4-132">storagePlanInformation</span><span class="sxs-lookup"><span data-stu-id="573b4-132">storagePlanInformation</span></span>  | [<span data-ttu-id="573b4-133">storagePlanInformation</span><span class="sxs-lookup"><span data-stu-id="573b4-133">storagePlanInformation</span></span>](storageplaninformation.md) | <span data-ttu-id="573b4-134">ドライブの記憶域のクォータの計画について説明します。</span><span class="sxs-lookup"><span data-stu-id="573b4-134">Information about the drive's storage quota plans.</span></span> <span data-ttu-id="573b4-135">で個人の OneDrive です。</span><span class="sxs-lookup"><span data-stu-id="573b4-135">Only in Personal OneDrive.</span></span>|

### <a name="state-enumeration-values"></a><span data-ttu-id="573b4-136">状態の列挙値</span><span class="sxs-lookup"><span data-stu-id="573b4-136">State enumeration values</span></span>

| <span data-ttu-id="573b4-137">値</span><span class="sxs-lookup"><span data-stu-id="573b4-137">Value</span></span>      | <span data-ttu-id="573b4-138">説明</span><span class="sxs-lookup"><span data-stu-id="573b4-138">Description</span></span>                                                                                                                                                                 |
|:-----------|:----------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| `normal`   | <span data-ttu-id="573b4-139">ドライブに十分なクォータが残っています。</span><span class="sxs-lookup"><span data-stu-id="573b4-139">The drive has plenty of remaining quota left.</span></span>                                                                                                                               |
| `nearing`  | <span data-ttu-id="573b4-140">残りのクォータは、クォータ領域の合計の 10% 未満です。</span><span class="sxs-lookup"><span data-stu-id="573b4-140">Remaining quota is less than 10% of total quota space.</span></span>                                                                                                                      |
| `critical` | <span data-ttu-id="573b4-141">残りのクォータは、クォータ領域の合計の 1% 未満です。</span><span class="sxs-lookup"><span data-stu-id="573b4-141">Remaining quota is less than 1% of total quota space.</span></span>                                                                                                                       |
| `exceeded` | <span data-ttu-id="573b4-p108">クォータ使用量が、クォータの合計を超えています。クォータの合計を下回るか、追加の記憶領域を購入するまで、新しいファイルまたはフォルダーをドライブに追加することはできません。</span><span class="sxs-lookup"><span data-stu-id="573b4-p108">The used quota has exceeded the total quota. New files or folders cannot be added to the drive until it is under the total quota amount or more storage space is purchased.</span></span> |

<!-- {
  "type": "#page.annotation",
  "description": "The quota facet provides information about how much space the OneDrive has available.",
  "keywords": "quota,available,remaining,used",
  "section": "documentation",
  "tocPath": "Facets/Quota"
} -->
