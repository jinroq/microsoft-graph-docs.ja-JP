---
title: updateWindow リソースの種類
description: updateWindow リソースの種類。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 57fb977dd853261300ed09dd8d9b3c343f62bea0
ms.sourcegitcommit: 8844023e15b7649a5c03603aee243acf85930ef2
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/24/2019
ms.locfileid: "35840955"
---
# <a name="updatewindow-resource-type"></a><span data-ttu-id="e4e9a-103">updateWindow リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e4e9a-103">updateWindow resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e4e9a-104">[エージェント](onpremisesagent.md)が更新を受信できる時間枠を表します。</span><span class="sxs-lookup"><span data-stu-id="e4e9a-104">Represents time window during which [agents](onpremisesagent.md) can receive updates.</span></span>

## <a name="properties"></a><span data-ttu-id="e4e9a-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e4e9a-105">Properties</span></span>

| <span data-ttu-id="e4e9a-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e4e9a-106">Property</span></span>     | <span data-ttu-id="e4e9a-107">型</span><span class="sxs-lookup"><span data-stu-id="e4e9a-107">Type</span></span>        | <span data-ttu-id="e4e9a-108">説明</span><span class="sxs-lookup"><span data-stu-id="e4e9a-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="e4e9a-109">updateWindowEndTime</span><span class="sxs-lookup"><span data-stu-id="e4e9a-109">updateWindowEndTime</span></span>|<span data-ttu-id="e4e9a-110">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="e4e9a-110">TimeOfDay</span></span>|<span data-ttu-id="e4e9a-111">エージェントが更新を受信できる時間枠の終わり</span><span class="sxs-lookup"><span data-stu-id="e4e9a-111">End of a time window during which agents can receive updates</span></span>|
|<span data-ttu-id="e4e9a-112">updateWindowStartTime</span><span class="sxs-lookup"><span data-stu-id="e4e9a-112">updateWindowStartTime</span></span>|<span data-ttu-id="e4e9a-113">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="e4e9a-113">TimeOfDay</span></span>|<span data-ttu-id="e4e9a-114">エージェントが更新プログラムを受信できる時間枠の開始</span><span class="sxs-lookup"><span data-stu-id="e4e9a-114">Start of a time window during which agents can receive updates</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e4e9a-115">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e4e9a-115">JSON representation</span></span>

<span data-ttu-id="e4e9a-116">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e4e9a-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.updateWindow",
  "baseType": null
}-->

```json
{
  "updateWindowEndTime": "String (timestamp)",
  "updateWindowStartTime": "String (timestamp)"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "updateWindow resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
