---
title: genericerror リソースの種類
description: 汎用エラー。
localization_priority: Normal
ms.openlocfilehash: d3c7e9cd7ff7be635adfbf329170068cd944f0b2
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32547499"
---
# <a name="genericerror-resource-type"></a><span data-ttu-id="79ed8-103">genericerror リソースの種類</span><span class="sxs-lookup"><span data-stu-id="79ed8-103">genericError resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="79ed8-104">汎用エラー。</span><span class="sxs-lookup"><span data-stu-id="79ed8-104">A general-purpose error.</span></span>

## <a name="properties"></a><span data-ttu-id="79ed8-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="79ed8-105">Properties</span></span>

| <span data-ttu-id="79ed8-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="79ed8-106">Property</span></span> | <span data-ttu-id="79ed8-107">型</span><span class="sxs-lookup"><span data-stu-id="79ed8-107">Type</span></span> | <span data-ttu-id="79ed8-108">説明</span><span class="sxs-lookup"><span data-stu-id="79ed8-108">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="79ed8-109">メッセージ​​</span><span class="sxs-lookup"><span data-stu-id="79ed8-109">message</span></span> | <span data-ttu-id="79ed8-110">String</span><span class="sxs-lookup"><span data-stu-id="79ed8-110">String</span></span> | <span data-ttu-id="79ed8-111">エラー メッセージ。</span><span class="sxs-lookup"><span data-stu-id="79ed8-111">The error message.</span></span> |
| <span data-ttu-id="79ed8-112">code</span><span class="sxs-lookup"><span data-stu-id="79ed8-112">code</span></span> | <span data-ttu-id="79ed8-113">String</span><span class="sxs-lookup"><span data-stu-id="79ed8-113">String</span></span> | <span data-ttu-id="79ed8-114">エラーコード。</span><span class="sxs-lookup"><span data-stu-id="79ed8-114">The error code.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="79ed8-115">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="79ed8-115">JSON representation</span></span>

<span data-ttu-id="79ed8-116">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="79ed8-116">Here is a JSON representation of the resource.</span></span>

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
