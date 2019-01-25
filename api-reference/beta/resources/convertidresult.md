---
title: convertIdResult リソースの種類
description: TranslateExchangeIds 関数によって実行される ID 形式変換の結果です。
localization_priority: Normal
ms.openlocfilehash: db28172d009ee8a8a39b7e02733d893dc20a81e5
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29516526"
---
# <a name="convertidresult-resource-type"></a><span data-ttu-id="f6b62-103">convertIdResult リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f6b62-103">convertIdResult resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f6b62-104">[TranslateExchangeIds](../api/user-translateexchangeids.md)関数によって実行される ID 形式変換の結果です。</span><span class="sxs-lookup"><span data-stu-id="f6b62-104">The result of an ID format conversion performed by the [translateExchangeIds](../api/user-translateexchangeids.md) function.</span></span>

## <a name="properties"></a><span data-ttu-id="f6b62-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f6b62-105">Properties</span></span>

| <span data-ttu-id="f6b62-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f6b62-106">Property</span></span> | <span data-ttu-id="f6b62-107">型</span><span class="sxs-lookup"><span data-stu-id="f6b62-107">Type</span></span> | <span data-ttu-id="f6b62-108">説明</span><span class="sxs-lookup"><span data-stu-id="f6b62-108">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="f6b62-109">SourceId</span><span class="sxs-lookup"><span data-stu-id="f6b62-109">sourceId</span></span> | <span data-ttu-id="f6b62-110">String</span><span class="sxs-lookup"><span data-stu-id="f6b62-110">String</span></span> | <span data-ttu-id="f6b62-111">変換された識別子です。</span><span class="sxs-lookup"><span data-stu-id="f6b62-111">The identifier that was converted.</span></span> <span data-ttu-id="f6b62-112">この値は、元、変換されていない識別子です。</span><span class="sxs-lookup"><span data-stu-id="f6b62-112">This value is the original, un-converted identifier.</span></span> |
| <span data-ttu-id="f6b62-113">targetId</span><span class="sxs-lookup"><span data-stu-id="f6b62-113">targetId</span></span> | <span data-ttu-id="f6b62-114">String</span><span class="sxs-lookup"><span data-stu-id="f6b62-114">String</span></span> | <span data-ttu-id="f6b62-115">変換後の識別子です。</span><span class="sxs-lookup"><span data-stu-id="f6b62-115">The converted identifier.</span></span> <span data-ttu-id="f6b62-116">この値は、変換が失敗した場合ではありません。</span><span class="sxs-lookup"><span data-stu-id="f6b62-116">This value is not present if the conversion failed.</span></span> |
| <span data-ttu-id="f6b62-117">ErrorDetails</span><span class="sxs-lookup"><span data-stu-id="f6b62-117">errorDetails</span></span> | [<span data-ttu-id="f6b62-118">genericError</span><span class="sxs-lookup"><span data-stu-id="f6b62-118">genericError</span></span>](genericerror.md) | <span data-ttu-id="f6b62-119">変換エラーの原因を示すエラー オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="f6b62-119">An error object indicating the reason for the conversion failure.</span></span> <span data-ttu-id="f6b62-120">この値は、変換が成功した場合ではありません。</span><span class="sxs-lookup"><span data-stu-id="f6b62-120">This value is not present if the conversion succeeded.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="f6b62-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f6b62-121">JSON representation</span></span>

<span data-ttu-id="f6b62-122">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="f6b62-122">Here is a JSON representation of the resource.</span></span>

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
