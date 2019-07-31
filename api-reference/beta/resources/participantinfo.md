---
title: participantInfo リソースの種類
description: 参加者の id に関する追加のプロパティが含まれています
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: ad73ce0bbeaa02b0207f11bbd3f0004857d90506
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966226"
---
# <a name="participantinfo-resource-type"></a><span data-ttu-id="028d4-103">participantInfo リソースの種類</span><span class="sxs-lookup"><span data-stu-id="028d4-103">participantInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="028d4-104">参加者の id に関する追加のプロパティが含まれています</span><span class="sxs-lookup"><span data-stu-id="028d4-104">Contains additional properties about the participant identity</span></span>

## <a name="properties"></a><span data-ttu-id="028d4-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="028d4-105">Properties</span></span>

| <span data-ttu-id="028d4-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="028d4-106">Property</span></span>       | <span data-ttu-id="028d4-107">型</span><span class="sxs-lookup"><span data-stu-id="028d4-107">Type</span></span>                          | <span data-ttu-id="028d4-108">説明</span><span class="sxs-lookup"><span data-stu-id="028d4-108">Description</span></span>  |
|:---------------|:------------------------------|:-------------|
| <span data-ttu-id="028d4-109">独自性</span><span class="sxs-lookup"><span data-stu-id="028d4-109">identity</span></span>       | [<span data-ttu-id="028d4-110">identitySet</span><span class="sxs-lookup"><span data-stu-id="028d4-110">identitySet</span></span>](identityset.md) | <span data-ttu-id="028d4-111">この参加者に関連付けられている id[セット](identityset.md)。</span><span class="sxs-lookup"><span data-stu-id="028d4-111">The [identitySet](identityset.md) associated with this participant.</span></span> |
| <span data-ttu-id="028d4-112">languageId</span><span class="sxs-lookup"><span data-stu-id="028d4-112">languageId</span></span>     | <span data-ttu-id="028d4-113">String</span><span class="sxs-lookup"><span data-stu-id="028d4-113">String</span></span>                        | <span data-ttu-id="028d4-114">言語のカルチャ文字列。</span><span class="sxs-lookup"><span data-stu-id="028d4-114">The language culture string.</span></span> |
| <span data-ttu-id="028d4-115">エリア</span><span class="sxs-lookup"><span data-stu-id="028d4-115">region</span></span>         | <span data-ttu-id="028d4-116">String</span><span class="sxs-lookup"><span data-stu-id="028d4-116">String</span></span>                        | <span data-ttu-id="028d4-117">参加者の地域。</span><span class="sxs-lookup"><span data-stu-id="028d4-117">Region of the participant.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="028d4-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="028d4-118">JSON representation</span></span>

<span data-ttu-id="028d4-119">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="028d4-119">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "languageId", "region"
  ],
  "@odata.type": "microsoft.graph.participantInfo"
}-->
```json
{
  "identity": { "@odata.type": "#microsoft.graph.identitySet" },
  "languageId": "String",
  "region": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "participantInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
