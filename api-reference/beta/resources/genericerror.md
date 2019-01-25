---
title: genericError リソースの種類
description: 汎用のエラーです。
localization_priority: Normal
ms.openlocfilehash: d3c7e9cd7ff7be635adfbf329170068cd944f0b2
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29524129"
---
# <a name="genericerror-resource-type"></a><span data-ttu-id="51d07-103">genericError リソースの種類</span><span class="sxs-lookup"><span data-stu-id="51d07-103">genericError resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="51d07-104">汎用のエラーです。</span><span class="sxs-lookup"><span data-stu-id="51d07-104">A general-purpose error.</span></span>

## <a name="properties"></a><span data-ttu-id="51d07-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="51d07-105">Properties</span></span>

| <span data-ttu-id="51d07-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="51d07-106">Property</span></span> | <span data-ttu-id="51d07-107">型</span><span class="sxs-lookup"><span data-stu-id="51d07-107">Type</span></span> | <span data-ttu-id="51d07-108">説明</span><span class="sxs-lookup"><span data-stu-id="51d07-108">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="51d07-109">message</span><span class="sxs-lookup"><span data-stu-id="51d07-109">message</span></span> | <span data-ttu-id="51d07-110">String</span><span class="sxs-lookup"><span data-stu-id="51d07-110">String</span></span> | <span data-ttu-id="51d07-111">エラー メッセージ。</span><span class="sxs-lookup"><span data-stu-id="51d07-111">The error message.</span></span> |
| <span data-ttu-id="51d07-112">code</span><span class="sxs-lookup"><span data-stu-id="51d07-112">code</span></span> | <span data-ttu-id="51d07-113">String</span><span class="sxs-lookup"><span data-stu-id="51d07-113">String</span></span> | <span data-ttu-id="51d07-114">エラー コード。</span><span class="sxs-lookup"><span data-stu-id="51d07-114">The error code.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="51d07-115">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="51d07-115">JSON representation</span></span>

<span data-ttu-id="51d07-116">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="51d07-116">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
  ],
  "@odata.type": "microsoft.graph.genericError"
}-->

```json
{
  "message": "String",
  "code": "String"
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/genericerror.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
