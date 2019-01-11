---
title: provisionedPlan リソースの種類
description: ユーザー エンティティと組織エンティティの **provisionedPlans** プロパティは、**provisionedPlan** のコレクションです。
localization_priority: Normal
ms.openlocfilehash: 7bed57761777e637fdc2e567d10aa7f741a86663
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27837255"
---
# <a name="provisionedplan-resource-type"></a><span data-ttu-id="188b8-103">provisionedPlan リソースの種類</span><span class="sxs-lookup"><span data-stu-id="188b8-103">provisionedPlan resource type</span></span>

> <span data-ttu-id="188b8-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="188b8-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="188b8-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="188b8-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="188b8-106">[ユーザー](user.md) エンティティと[組織](organization.md)エンティティの **provisionedPlans** プロパティは、**provisionedPlan** のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="188b8-106">The **provisionedPlans** property of the [user](user.md) entity and the [organization](organization.md) entity is a collection of **provisionedPlan**.</span></span>


## <a name="properties"></a><span data-ttu-id="188b8-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="188b8-107">Properties</span></span>
| <span data-ttu-id="188b8-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="188b8-108">Property</span></span>     | <span data-ttu-id="188b8-109">種類</span><span class="sxs-lookup"><span data-stu-id="188b8-109">Type</span></span>   |<span data-ttu-id="188b8-110">説明</span><span class="sxs-lookup"><span data-stu-id="188b8-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="188b8-111">capabilityStatus</span><span class="sxs-lookup"><span data-stu-id="188b8-111">capabilityStatus</span></span>|<span data-ttu-id="188b8-112">String</span><span class="sxs-lookup"><span data-stu-id="188b8-112">String</span></span>|<span data-ttu-id="188b8-113">「有効」など。</span><span class="sxs-lookup"><span data-stu-id="188b8-113">For example, “Enabled”.</span></span>|
|<span data-ttu-id="188b8-114">provisioningStatus</span><span class="sxs-lookup"><span data-stu-id="188b8-114">provisioningStatus</span></span>|<span data-ttu-id="188b8-115">String</span><span class="sxs-lookup"><span data-stu-id="188b8-115">String</span></span>|<span data-ttu-id="188b8-116">「成功」など。</span><span class="sxs-lookup"><span data-stu-id="188b8-116">For example, “Success”.</span></span>|
|<span data-ttu-id="188b8-117">service</span><span class="sxs-lookup"><span data-stu-id="188b8-117">service</span></span>|<span data-ttu-id="188b8-118">String</span><span class="sxs-lookup"><span data-stu-id="188b8-118">String</span></span>|<span data-ttu-id="188b8-119">サービスの名前。「AccessControlS2S」など。</span><span class="sxs-lookup"><span data-stu-id="188b8-119">The name of the service; for example, “AccessControlS2S”</span></span>|

## <a name="json-representation"></a><span data-ttu-id="188b8-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="188b8-120">JSON representation</span></span>

<span data-ttu-id="188b8-121">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="188b8-121">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.provisionedplan"
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
<!-- {
  "type": "#page.annotation",
  "description": "provisionedPlan resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
