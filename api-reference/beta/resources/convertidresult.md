---
title: convertIdResult リソースの種類
description: translateExchangeIds 関数によって実行される ID 形式変換の結果。
localization_priority: Normal
ms.openlocfilehash: db28172d009ee8a8a39b7e02733d893dc20a81e5
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32535392"
---
# <a name="convertidresult-resource-type"></a><span data-ttu-id="15e7d-103">convertIdResult リソースの種類</span><span class="sxs-lookup"><span data-stu-id="15e7d-103">convertIdResult resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="15e7d-104">[translateExchangeIds](../api/user-translateexchangeids.md)関数によって実行される ID 形式変換の結果。</span><span class="sxs-lookup"><span data-stu-id="15e7d-104">The result of an ID format conversion performed by the [translateExchangeIds](../api/user-translateexchangeids.md) function.</span></span>

## <a name="properties"></a><span data-ttu-id="15e7d-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="15e7d-105">Properties</span></span>

| <span data-ttu-id="15e7d-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="15e7d-106">Property</span></span> | <span data-ttu-id="15e7d-107">型</span><span class="sxs-lookup"><span data-stu-id="15e7d-107">Type</span></span> | <span data-ttu-id="15e7d-108">説明</span><span class="sxs-lookup"><span data-stu-id="15e7d-108">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="15e7d-109">sourceId</span><span class="sxs-lookup"><span data-stu-id="15e7d-109">sourceId</span></span> | <span data-ttu-id="15e7d-110">String</span><span class="sxs-lookup"><span data-stu-id="15e7d-110">String</span></span> | <span data-ttu-id="15e7d-111">変換された識別子。</span><span class="sxs-lookup"><span data-stu-id="15e7d-111">The identifier that was converted.</span></span> <span data-ttu-id="15e7d-112">この値は、元の、変換されていない識別子です。</span><span class="sxs-lookup"><span data-stu-id="15e7d-112">This value is the original, un-converted identifier.</span></span> |
| <span data-ttu-id="15e7d-113">targetId</span><span class="sxs-lookup"><span data-stu-id="15e7d-113">targetId</span></span> | <span data-ttu-id="15e7d-114">String</span><span class="sxs-lookup"><span data-stu-id="15e7d-114">String</span></span> | <span data-ttu-id="15e7d-115">変換された識別子。</span><span class="sxs-lookup"><span data-stu-id="15e7d-115">The converted identifier.</span></span> <span data-ttu-id="15e7d-116">変換が失敗した場合、この値は表示されません。</span><span class="sxs-lookup"><span data-stu-id="15e7d-116">This value is not present if the conversion failed.</span></span> |
| <span data-ttu-id="15e7d-117">errorDetails</span><span class="sxs-lookup"><span data-stu-id="15e7d-117">errorDetails</span></span> | [<span data-ttu-id="15e7d-118">genericerror</span><span class="sxs-lookup"><span data-stu-id="15e7d-118">genericError</span></span>](genericerror.md) | <span data-ttu-id="15e7d-119">変換エラーの理由を示す error オブジェクト。</span><span class="sxs-lookup"><span data-stu-id="15e7d-119">An error object indicating the reason for the conversion failure.</span></span> <span data-ttu-id="15e7d-120">この値は、変換に成功した場合は表示されません。</span><span class="sxs-lookup"><span data-stu-id="15e7d-120">This value is not present if the conversion succeeded.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="15e7d-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="15e7d-121">JSON representation</span></span>

<span data-ttu-id="15e7d-122">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="15e7d-122">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "targetId",
    "errorDetails"
  ],
  "@odata.type": "microsoft.graph.convertIdResult"
}-->

```json
{
  "sourceId": "String",
  "targetId": "String",
  "errorDetails": {
    "@odata.type": "microsoft.graph.genericError"
  }
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/convertidresult.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
