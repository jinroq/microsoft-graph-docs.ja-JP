---
title: 電子メールリソースの種類
description: 以下は、リソースの JSON 表記です
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: cc1fc5bf69cb420b8cd0476a439123e90b236b48
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32542979"
---
# <a name="email-resource-type"></a><span data-ttu-id="77cb4-103">電子メールリソースの種類</span><span class="sxs-lookup"><span data-stu-id="77cb4-103">email resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="json-representation"></a><span data-ttu-id="77cb4-104">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="77cb4-104">JSON representation</span></span>

<span data-ttu-id="77cb4-105">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="77cb4-105">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.email"
}-->

```json
{
  "address": "string"
}

```
## <a name="properties"></a><span data-ttu-id="77cb4-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="77cb4-106">Properties</span></span>
| <span data-ttu-id="77cb4-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="77cb4-107">Property</span></span>     | <span data-ttu-id="77cb4-108">型</span><span class="sxs-lookup"><span data-stu-id="77cb4-108">Type</span></span>   |<span data-ttu-id="77cb4-109">説明</span><span class="sxs-lookup"><span data-stu-id="77cb4-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="77cb4-110">address</span><span class="sxs-lookup"><span data-stu-id="77cb4-110">address</span></span>|<span data-ttu-id="77cb4-111">String</span><span class="sxs-lookup"><span data-stu-id="77cb4-111">String</span></span>||

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "email resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/email.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
