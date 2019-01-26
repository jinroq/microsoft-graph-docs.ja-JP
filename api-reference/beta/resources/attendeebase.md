---
title: attendeeBase リソースの種類
description: 出席者の種類です。
localization_priority: Normal
ms.openlocfilehash: 6ec80f5505cb3dd742a2690ebb3cd5374635770d
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/26/2019
ms.locfileid: "29572739"
---
# <a name="attendeebase-resource-type"></a><span data-ttu-id="77715-103">attendeeBase リソースの種類</span><span class="sxs-lookup"><span data-stu-id="77715-103">attendeeBase resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="77715-104">出席者の種類です。</span><span class="sxs-lookup"><span data-stu-id="77715-104">The type of attendee.</span></span>

<span data-ttu-id="77715-105">[recipient](recipient.md) から派生します。</span><span class="sxs-lookup"><span data-stu-id="77715-105">Derived from [recipient](recipient.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="77715-106">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="77715-106">JSON representation</span></span>

<span data-ttu-id="77715-107">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="77715-107">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.recipient",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.attendeeBase"
}-->

```json
{
  "type": "String",
  "emailAddress": {"@odata.type": "microsoft.graph.emailAddress"}
}

```
## <a name="properties"></a><span data-ttu-id="77715-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="77715-108">Properties</span></span>
| <span data-ttu-id="77715-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="77715-109">Property</span></span>     | <span data-ttu-id="77715-110">型</span><span class="sxs-lookup"><span data-stu-id="77715-110">Type</span></span>   |<span data-ttu-id="77715-111">説明</span><span class="sxs-lookup"><span data-stu-id="77715-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="77715-112">type</span><span class="sxs-lookup"><span data-stu-id="77715-112">type</span></span>|<span data-ttu-id="77715-113">attendeeType</span><span class="sxs-lookup"><span data-stu-id="77715-113">attendeeType</span></span>| <span data-ttu-id="77715-114">出席者の種類です。</span><span class="sxs-lookup"><span data-stu-id="77715-114">The type of attendee.</span></span> <span data-ttu-id="77715-115">可能な値: `required`、 `optional`、 `resource`。</span><span class="sxs-lookup"><span data-stu-id="77715-115">The possible values are: `required`, `optional`, `resource`.</span></span> <span data-ttu-id="77715-116">現在、出席者が人間の場合は、 [findMeetingTimes](../api/user-findmeetingtimes.md)は一切の人では、`Required`型です。</span><span class="sxs-lookup"><span data-stu-id="77715-116">Currently if the attendee is a person, [findMeetingTimes](../api/user-findmeetingtimes.md) always considers the person is of the `Required` type.</span></span>|
|<span data-ttu-id="77715-117">emailAddress</span><span class="sxs-lookup"><span data-stu-id="77715-117">emailAddress</span></span>|[<span data-ttu-id="77715-118">emailAddress</span><span class="sxs-lookup"><span data-stu-id="77715-118">emailAddress</span></span>](emailaddress.md)|<span data-ttu-id="77715-119">参加者の名前と SMTP アドレスが含まれます。</span><span class="sxs-lookup"><span data-stu-id="77715-119">Includes the name and SMTP address of the attendee.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "attendeeBase resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/attendeebase.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
