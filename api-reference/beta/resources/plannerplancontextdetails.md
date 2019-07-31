---
title: プラン、Contextdetails リソースの種類
description: 「 **Plan The Contextdetails** resource」には、プランのコンテキストに関する追加情報が含まれています。
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 9d4bf7d0a5c2149f826097eedc350e81eb32bf70
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36009021"
---
# <a name="plannerplancontextdetails-resource-type"></a><span data-ttu-id="b5b93-103">プラン、Contextdetails リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b5b93-103">plannerPlanContextDetails resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b5b93-104">「 **Plan The Contextdetails** resource」には、プランの[コンテキスト](plannerplancontext.md)に関する追加情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="b5b93-104">The **plannerPlanContextDetails** resource contains additional information about a [plannerPlanContext](plannerplancontext.md).</span></span>

## <a name="properties"></a><span data-ttu-id="b5b93-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b5b93-105">Properties</span></span>
| <span data-ttu-id="b5b93-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b5b93-106">Property</span></span>     | <span data-ttu-id="b5b93-107">型</span><span class="sxs-lookup"><span data-stu-id="b5b93-107">Type</span></span>   |<span data-ttu-id="b5b93-108">説明</span><span class="sxs-lookup"><span data-stu-id="b5b93-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b5b93-109">url</span><span class="sxs-lookup"><span data-stu-id="b5b93-109">url</span></span>|<span data-ttu-id="b5b93-110">String</span><span class="sxs-lookup"><span data-stu-id="b5b93-110">String</span></span>|<span data-ttu-id="b5b93-111">関連する[プランのコンテキスト](plannerplancontext.md)によって表されるユーザーの作業の URL。</span><span class="sxs-lookup"><span data-stu-id="b5b93-111">URL of the user experience represented by the associated [plannerPlanContext](plannerplancontext.md).</span></span> |

## <a name="json-representation"></a><span data-ttu-id="b5b93-112">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b5b93-112">JSON representation</span></span>

<span data-ttu-id="b5b93-113">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="b5b93-113">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerPlanContextDetails"
}-->

```json
{
  "url": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "plannerPlanContextDetails resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
