---
title: mentionsPreview リソースの種類
description: リソースインスタンス内のメンションオブジェクトに関する情報を表します。
localization_priority: Normal
author: simonhult
ms.prod: insights
ms.openlocfilehash: 516560d2a0a8e498c1a0b31a62d8ca4209724767
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33342290"
---
# <a name="mentionspreview-resource-type"></a><span data-ttu-id="341ee-103">mentionsPreview リソースの種類</span><span class="sxs-lookup"><span data-stu-id="341ee-103">mentionsPreview resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="341ee-104">リソースインスタンス内の[メンション](../resources/mention.md)オブジェクトに関する情報を表します。</span><span class="sxs-lookup"><span data-stu-id="341ee-104">Represents information about [mention](../resources/mention.md) objects in a resource instance.</span></span>

## <a name="properties"></a><span data-ttu-id="341ee-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="341ee-105">Properties</span></span>
| <span data-ttu-id="341ee-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="341ee-106">Property</span></span>     | <span data-ttu-id="341ee-107">型</span><span class="sxs-lookup"><span data-stu-id="341ee-107">Type</span></span>   |<span data-ttu-id="341ee-108">説明</span><span class="sxs-lookup"><span data-stu-id="341ee-108">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="341ee-109">説明</span><span class="sxs-lookup"><span data-stu-id="341ee-109">isMentioned</span></span> | <span data-ttu-id="341ee-110">Boolean</span><span class="sxs-lookup"><span data-stu-id="341ee-110">Boolean</span></span> | <span data-ttu-id="341ee-111">True の場合は、サインインしているユーザーが親リソースインスタンスで言及されます。</span><span class="sxs-lookup"><span data-stu-id="341ee-111">True if the signed-in user is mentioned in the parent resource instance.</span></span> <span data-ttu-id="341ee-112">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="341ee-112">Read-only.</span></span> <span data-ttu-id="341ee-113">フィルターをサポートします。</span><span class="sxs-lookup"><span data-stu-id="341ee-113">Supports filter.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="341ee-114">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="341ee-114">JSON representation</span></span>

<span data-ttu-id="341ee-115">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="341ee-115">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.mentionsPreview"
}-->

```json
{
  "isMentioned": "Boolean"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "mentionsPreview resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
