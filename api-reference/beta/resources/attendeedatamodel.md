---
title: attendeeDataModel リソースの種類
description: 出席者の種類です。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: e8659b88cae8b9d2a94177593da40b61363fa23b
ms.sourcegitcommit: 539ed08adf3b7ad3253c98636d4ab303ce00176e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/15/2019
ms.locfileid: "30057405"
---
# <a name="attendeedatamodel-resource-type"></a><span data-ttu-id="426de-103">attendeeDataModel リソースの種類</span><span class="sxs-lookup"><span data-stu-id="426de-103">attendeeDataModel resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="426de-104">会議に含まれている個人またはリソースを表します。</span><span class="sxs-lookup"><span data-stu-id="426de-104">Represents a person or resource who is being included in a meeting.</span></span>

## <a name="json-representation"></a><span data-ttu-id="426de-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="426de-105">JSON representation</span></span>

<span data-ttu-id="426de-106">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="426de-106">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "type"
  ],
  "@odata.type": "microsoft.graph.attendeeDataModel"
}-->

```json
{
  "type": "String",
  "emailAddress": {"@odata.type": "microsoft.graph.emailAddress"}
}

```
## <a name="properties"></a><span data-ttu-id="426de-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="426de-107">Properties</span></span>
| <span data-ttu-id="426de-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="426de-108">Property</span></span>     | <span data-ttu-id="426de-109">型</span><span class="sxs-lookup"><span data-stu-id="426de-109">Type</span></span>   |<span data-ttu-id="426de-110">説明</span><span class="sxs-lookup"><span data-stu-id="426de-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="426de-111">type</span><span class="sxs-lookup"><span data-stu-id="426de-111">type</span></span>|<span data-ttu-id="426de-112">attendeeType</span><span class="sxs-lookup"><span data-stu-id="426de-112">attendeeType</span></span>| <span data-ttu-id="426de-113">出席者の種類です。</span><span class="sxs-lookup"><span data-stu-id="426de-113">The type of attendee.</span></span> <span data-ttu-id="426de-114">使用可能な値は`required`、 `optional`、 `resource`、です。</span><span class="sxs-lookup"><span data-stu-id="426de-114">The possible values are: `required`, `optional`, `resource`.</span></span> <span data-ttu-id="426de-115">現時点では、参加者が人物の場合、 [findの会議時間](../api/user-findmeetingtimes.md)は常にその`required`人物の種類を考慮します。</span><span class="sxs-lookup"><span data-stu-id="426de-115">Currently if the attendee is a person, [findMeetingTimes](../api/user-findmeetingtimes.md) always considers the person is of the `required` type.</span></span>|
|<span data-ttu-id="426de-116">emailAddress</span><span class="sxs-lookup"><span data-stu-id="426de-116">emailAddress</span></span>|[<span data-ttu-id="426de-117">emailAddress</span><span class="sxs-lookup"><span data-stu-id="426de-117">emailAddress</span></span>](emailaddress.md)|<span data-ttu-id="426de-118">参加者の名前と SMTP アドレスが含まれます。</span><span class="sxs-lookup"><span data-stu-id="426de-118">Includes the name and SMTP address of the attendee.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "attendeeDataModel resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/attendeedatamodel.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->