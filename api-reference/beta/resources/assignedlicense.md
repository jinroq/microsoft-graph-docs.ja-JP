---
title: assignedLicense リソースの種類
description: ユーザーに割り当てられているライセンスを表します。ユーザー エンティティの **assignedLicenses** プロパティは、**assignedLicense** のコレクションです。
localization_priority: Normal
ms.openlocfilehash: dfb93075fe62a0cfb479e12554e9078e876c4529
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27853784"
---
# <a name="assignedlicense-resource-type"></a><span data-ttu-id="91805-104">assignedLicense リソースの種類</span><span class="sxs-lookup"><span data-stu-id="91805-104">assignedLicense resource type</span></span>

> <span data-ttu-id="91805-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="91805-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="91805-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="91805-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="91805-p103">ユーザーに割り当てられているライセンスを表します。[ユーザー](user.md) エンティティの **assignedLicenses** プロパティは、**assignedLicense** のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="91805-p103">Represents a license assigned to a user. The **assignedLicenses** property of the [user](user.md) entity is a collection of **assignedLicense**.</span></span>

## <a name="properties"></a><span data-ttu-id="91805-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="91805-109">Properties</span></span>
| <span data-ttu-id="91805-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="91805-110">Property</span></span>     | <span data-ttu-id="91805-111">種類</span><span class="sxs-lookup"><span data-stu-id="91805-111">Type</span></span>   |<span data-ttu-id="91805-112">説明</span><span class="sxs-lookup"><span data-stu-id="91805-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="91805-113">disabledPlans</span><span class="sxs-lookup"><span data-stu-id="91805-113">disabledPlans</span></span>|<span data-ttu-id="91805-114">Guid コレクション</span><span class="sxs-lookup"><span data-stu-id="91805-114">Guid collection</span></span>|<span data-ttu-id="91805-115">無効になっているプランの一意識別子のコレクション。</span><span class="sxs-lookup"><span data-stu-id="91805-115">A collection of the unique identifiers for plans that have been disabled.</span></span>|
|<span data-ttu-id="91805-116">skuId</span><span class="sxs-lookup"><span data-stu-id="91805-116">skuId</span></span>|<span data-ttu-id="91805-117">Guid</span><span class="sxs-lookup"><span data-stu-id="91805-117">Guid</span></span>|<span data-ttu-id="91805-118">SKU の一意識別子。</span><span class="sxs-lookup"><span data-stu-id="91805-118">The unique identifier for the SKU.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="91805-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="91805-119">JSON representation</span></span>

<span data-ttu-id="91805-120">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="91805-120">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.assignedLicense"
}-->

```json
{
  "disabledPlans": ["guid"],
  "skuId": "guid"
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "assignedLicense resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
