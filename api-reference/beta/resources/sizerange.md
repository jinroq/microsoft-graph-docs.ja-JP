---
title: sizeRange リソースの種類
description: '条件または例外を適用するために、受信メッセージに想定される最小サイズと最大サイズ (単位: キロバイト) を指定します。'
localization_priority: Normal
ms.openlocfilehash: ecf4a4349e7ee54b9f21fa27879834b45dc87491
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32583246"
---
# <a name="sizerange-resource-type"></a><span data-ttu-id="69c70-103">sizeRange リソースの種類</span><span class="sxs-lookup"><span data-stu-id="69c70-103">sizeRange resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="69c70-104">条件または例外を適用するために、受信メッセージに想定される最小サイズと最大サイズ (単位: キロバイト) を指定します。</span><span class="sxs-lookup"><span data-stu-id="69c70-104">Specifies the maximum and minimum sizes (in kilobytes) that an incoming message must have in order for a condition or exception to apply.</span></span>

## <a name="properties"></a><span data-ttu-id="69c70-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="69c70-105">Properties</span></span>
| <span data-ttu-id="69c70-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="69c70-106">Property</span></span>     | <span data-ttu-id="69c70-107">型</span><span class="sxs-lookup"><span data-stu-id="69c70-107">Type</span></span>   |<span data-ttu-id="69c70-108">説明</span><span class="sxs-lookup"><span data-stu-id="69c70-108">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="69c70-109">maximumSize</span><span class="sxs-lookup"><span data-stu-id="69c70-109">maximumSize</span></span> | <span data-ttu-id="69c70-110">Int32</span><span class="sxs-lookup"><span data-stu-id="69c70-110">Int32</span></span> | <span data-ttu-id="69c70-111">条件または例外を適用するために、受信メッセージに想定される最大サイズ (単位: キロバイト)。</span><span class="sxs-lookup"><span data-stu-id="69c70-111">The maximum size (in kilobytes) that an incoming message must have in order for a condition or exception to apply.</span></span> |
| <span data-ttu-id="69c70-112">minimumSize</span><span class="sxs-lookup"><span data-stu-id="69c70-112">minimumSize</span></span> | <span data-ttu-id="69c70-113">Int32</span><span class="sxs-lookup"><span data-stu-id="69c70-113">Int32</span></span> | <span data-ttu-id="69c70-114">条件または例外を適用するために、受信メッセージに想定される最小サイズ (単位: キロバイト)。</span><span class="sxs-lookup"><span data-stu-id="69c70-114">The minimum size (in kilobytes) that an incoming message must have in order for a condition or exception to apply.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="69c70-115">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="69c70-115">JSON representation</span></span>
<span data-ttu-id="69c70-116">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="69c70-116">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
   ],
  "@odata.type": "microsoft.graph.sizeRange"
}-->

```json
{
  "maximumSize": "Int32",
  "minimumSize": "Int32"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "sizeRange resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/sizerange.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
