---
title: copystatusmodel リソースの種類
description: 以下は、リソースの JSON 表記です。
localization_priority: Normal
ms.openlocfilehash: bf1a88b74f38f21f89b089b31ea5b6e7b6af9f0b
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32535236"
---
# <a name="copystatusmodel-resource-type"></a><span data-ttu-id="3c308-103">copystatusmodel リソースの種類</span><span class="sxs-lookup"><span data-stu-id="3c308-103">copyStatusModel resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="json-representation"></a><span data-ttu-id="3c308-104">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="3c308-104">JSON representation</span></span>

<span data-ttu-id="3c308-105">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="3c308-105">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.copystatusmodel"
}-->

```json
{
  "createdDateTime": "String (timestamp)",
  "id": "string",
  "status": "string"
}

```
## <a name="properties"></a><span data-ttu-id="3c308-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3c308-106">Properties</span></span>
| <span data-ttu-id="3c308-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3c308-107">Property</span></span>     | <span data-ttu-id="3c308-108">型</span><span class="sxs-lookup"><span data-stu-id="3c308-108">Type</span></span>   |<span data-ttu-id="3c308-109">説明</span><span class="sxs-lookup"><span data-stu-id="3c308-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3c308-110">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3c308-110">createdDateTime</span></span>| <span data-ttu-id="3c308-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3c308-111">DateTimeOffset</span></span> ||
|<span data-ttu-id="3c308-112">id</span><span class="sxs-lookup"><span data-stu-id="3c308-112">id</span></span>|<span data-ttu-id="3c308-113">string</span><span class="sxs-lookup"><span data-stu-id="3c308-113">string</span></span>||
|<span data-ttu-id="3c308-114">status</span><span class="sxs-lookup"><span data-stu-id="3c308-114">status</span></span>|<span data-ttu-id="3c308-115">string</span><span class="sxs-lookup"><span data-stu-id="3c308-115">string</span></span>||

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "copyStatusModel resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/copystatusmodel.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
