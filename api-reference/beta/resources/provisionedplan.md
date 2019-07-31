---
title: provisionedPlan リソースの種類
description: '**ユーザー** エンティティと組織エンティティの provisionedPlans プロパティは、**provisionedPlan** のコレクションです。'
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 76c29a74d54ca6e02febe8c83c80072bf158aa6b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965556"
---
# <a name="provisionedplan-resource-type"></a><span data-ttu-id="203b8-103">provisionedPlan リソースの種類</span><span class="sxs-lookup"><span data-stu-id="203b8-103">provisionedPlan resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="203b8-104">**ユーザー** エンティティと[組織](user.md)エンティティの [provisionedPlans](organization.md) プロパティは、**provisionedPlan** のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="203b8-104">The **provisionedPlans** property of the [user](user.md) entity and the [organization](organization.md) entity is a collection of **provisionedPlan**.</span></span>


## <a name="properties"></a><span data-ttu-id="203b8-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="203b8-105">Properties</span></span>
| <span data-ttu-id="203b8-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="203b8-106">Property</span></span>     | <span data-ttu-id="203b8-107">型</span><span class="sxs-lookup"><span data-stu-id="203b8-107">Type</span></span>   |<span data-ttu-id="203b8-108">説明</span><span class="sxs-lookup"><span data-stu-id="203b8-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="203b8-109">capabilityStatus</span><span class="sxs-lookup"><span data-stu-id="203b8-109">capabilityStatus</span></span>|<span data-ttu-id="203b8-110">String</span><span class="sxs-lookup"><span data-stu-id="203b8-110">String</span></span>|<span data-ttu-id="203b8-111">「有効」など。</span><span class="sxs-lookup"><span data-stu-id="203b8-111">For example, “Enabled”.</span></span>|
|<span data-ttu-id="203b8-112">プロビジョニング状態</span><span class="sxs-lookup"><span data-stu-id="203b8-112">provisioningStatus</span></span>|<span data-ttu-id="203b8-113">String</span><span class="sxs-lookup"><span data-stu-id="203b8-113">String</span></span>|<span data-ttu-id="203b8-114">「成功」など。</span><span class="sxs-lookup"><span data-stu-id="203b8-114">For example, “Success”.</span></span>|
|<span data-ttu-id="203b8-115">service</span><span class="sxs-lookup"><span data-stu-id="203b8-115">service</span></span>|<span data-ttu-id="203b8-116">String</span><span class="sxs-lookup"><span data-stu-id="203b8-116">String</span></span>|<span data-ttu-id="203b8-117">サービスの名前。「AccessControlS2S」など。</span><span class="sxs-lookup"><span data-stu-id="203b8-117">The name of the service; for example, “AccessControlS2S”</span></span>|

## <a name="json-representation"></a><span data-ttu-id="203b8-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="203b8-118">JSON representation</span></span>

<span data-ttu-id="203b8-119">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="203b8-119">Here is a JSON representation of the resource</span></span>

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
