---
title: provisionedPlan リソースの種類
description: '**ユーザー** エンティティと組織エンティティの provisionedPlans プロパティは、**provisionedPlan** のコレクションです。'
localization_priority: Normal
ms.openlocfilehash: 1d6bec5cdcd4caaf8990caac6614f2fa589d4c4c
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33344031"
---
# <a name="provisionedplan-resource-type"></a><span data-ttu-id="8df2a-103">provisionedPlan リソースの種類</span><span class="sxs-lookup"><span data-stu-id="8df2a-103">provisionedPlan resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8df2a-104">**ユーザー** エンティティと[組織](user.md)エンティティの [provisionedPlans](organization.md) プロパティは、**provisionedPlan** のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="8df2a-104">The **provisionedPlans** property of the [user](user.md) entity and the [organization](organization.md) entity is a collection of **provisionedPlan**.</span></span>


## <a name="properties"></a><span data-ttu-id="8df2a-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8df2a-105">Properties</span></span>
| <span data-ttu-id="8df2a-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8df2a-106">Property</span></span>     | <span data-ttu-id="8df2a-107">型</span><span class="sxs-lookup"><span data-stu-id="8df2a-107">Type</span></span>   |<span data-ttu-id="8df2a-108">説明</span><span class="sxs-lookup"><span data-stu-id="8df2a-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8df2a-109">capabilityStatus</span><span class="sxs-lookup"><span data-stu-id="8df2a-109">capabilityStatus</span></span>|<span data-ttu-id="8df2a-110">String</span><span class="sxs-lookup"><span data-stu-id="8df2a-110">String</span></span>|<span data-ttu-id="8df2a-111">「有効」など。</span><span class="sxs-lookup"><span data-stu-id="8df2a-111">For example, “Enabled”.</span></span>|
|<span data-ttu-id="8df2a-112">プロビジョニング状態</span><span class="sxs-lookup"><span data-stu-id="8df2a-112">provisioningStatus</span></span>|<span data-ttu-id="8df2a-113">String</span><span class="sxs-lookup"><span data-stu-id="8df2a-113">String</span></span>|<span data-ttu-id="8df2a-114">「成功」など。</span><span class="sxs-lookup"><span data-stu-id="8df2a-114">For example, “Success”.</span></span>|
|<span data-ttu-id="8df2a-115">service</span><span class="sxs-lookup"><span data-stu-id="8df2a-115">service</span></span>|<span data-ttu-id="8df2a-116">String</span><span class="sxs-lookup"><span data-stu-id="8df2a-116">String</span></span>|<span data-ttu-id="8df2a-117">サービスの名前。「AccessControlS2S」など。</span><span class="sxs-lookup"><span data-stu-id="8df2a-117">The name of the service; for example, “AccessControlS2S”</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8df2a-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="8df2a-118">JSON representation</span></span>

<span data-ttu-id="8df2a-119">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="8df2a-119">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.provisionedPlan"
}-->

```json
{
  "capabilityStatus": "string",
  "provisioningStatus": "string",
  "service": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "provisionedPlan resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
