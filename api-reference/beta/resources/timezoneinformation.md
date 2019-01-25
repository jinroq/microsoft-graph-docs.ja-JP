---
title: timeZoneInformation リソースの種類
description: タイム ゾーンを表します。 サポートされている形式は、Windows、およびインターネット割り当て番号機関 (IANA) はタイム ゾーン (Olson タイム ・ ゾーンとも呼ばれます)
localization_priority: Normal
ms.openlocfilehash: a63721de7ed4e8c3f3b74ce5954a88ee71a95414
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29526775"
---
# <a name="timezoneinformation-resource-type"></a><span data-ttu-id="75a63-104">timeZoneInformation リソースの種類</span><span class="sxs-lookup"><span data-stu-id="75a63-104">timeZoneInformation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="75a63-105">タイム ゾーンを表します。</span><span class="sxs-lookup"><span data-stu-id="75a63-105">Represents a time zone.</span></span> <span data-ttu-id="75a63-106">サポートされる形式は、Windows 形式です。現在既知の問題が解決されている場合は、[Internet Assigned Numbers Authority (IANA) タイム ゾーン](https://www.iana.org/time-zones) (Olson タイム ゾーンとも呼ばれる) 形式もサポートされます。</span><span class="sxs-lookup"><span data-stu-id="75a63-106">The supported format is Windows, and [Internet Assigned Numbers Authority (IANA) time zone](https://www.iana.org/time-zones) (also known as Olson time zone) format as well when the current known problem is fixed.</span></span>

## <a name="properties"></a><span data-ttu-id="75a63-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="75a63-107">Properties</span></span>
| <span data-ttu-id="75a63-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="75a63-108">Property</span></span>     | <span data-ttu-id="75a63-109">型</span><span class="sxs-lookup"><span data-stu-id="75a63-109">Type</span></span>   |<span data-ttu-id="75a63-110">説明</span><span class="sxs-lookup"><span data-stu-id="75a63-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="75a63-111">alias</span><span class="sxs-lookup"><span data-stu-id="75a63-111">alias</span></span>|<span data-ttu-id="75a63-112">string</span><span class="sxs-lookup"><span data-stu-id="75a63-112">string</span></span>|<span data-ttu-id="75a63-113">タイム ゾーンの識別子。</span><span class="sxs-lookup"><span data-stu-id="75a63-113">An identifier for the time zone.</span></span>|
|<span data-ttu-id="75a63-114">displayName</span><span class="sxs-lookup"><span data-stu-id="75a63-114">displayName</span></span>|<span data-ttu-id="75a63-115">string</span><span class="sxs-lookup"><span data-stu-id="75a63-115">string</span></span>|<span data-ttu-id="75a63-116">タイム ゾーンを表す表示文字列。</span><span class="sxs-lookup"><span data-stu-id="75a63-116">A display string that represents the time zone.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="75a63-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="75a63-117">JSON representation</span></span>

<span data-ttu-id="75a63-118">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="75a63-118">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.timeZoneInformation"
}-->

```json
{
  "alias": "string",
  "displayName": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "timeZoneInformation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/timezoneinformation.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
