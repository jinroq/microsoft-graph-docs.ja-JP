---
title: attendeeBase リソースの種類
description: 出席者の種類です。
localization_priority: Normal
ms.openlocfilehash: bce1550c107f2114d02744091b5863360ab0bcea
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29517457"
---
# <a name="attendeebase-resource-type"></a><span data-ttu-id="a8d22-103">attendeeBase リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a8d22-103">attendeeBase resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a8d22-104">出席者の種類です。</span><span class="sxs-lookup"><span data-stu-id="a8d22-104">The type of attendee.</span></span>

<span data-ttu-id="a8d22-105">[recipient](recipient.md) から派生します。</span><span class="sxs-lookup"><span data-stu-id="a8d22-105">Derived from [recipient](recipient.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="a8d22-106">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a8d22-106">JSON representation</span></span>

<span data-ttu-id="a8d22-107">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="a8d22-107">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
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
## <a name="properties"></a><span data-ttu-id="a8d22-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a8d22-108">Properties</span></span>
| <span data-ttu-id="a8d22-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a8d22-109">Property</span></span>     | <span data-ttu-id="a8d22-110">型</span><span class="sxs-lookup"><span data-stu-id="a8d22-110">Type</span></span>   |<span data-ttu-id="a8d22-111">説明</span><span class="sxs-lookup"><span data-stu-id="a8d22-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a8d22-112">type</span><span class="sxs-lookup"><span data-stu-id="a8d22-112">type</span></span>|<span data-ttu-id="a8d22-113">String</span><span class="sxs-lookup"><span data-stu-id="a8d22-113">String</span></span>| <span data-ttu-id="a8d22-p101">出席者の種類です。使用可能な値: `required`、`optional`、`resource`。現時点では、出席者が 1 人である場合、[findMeetingTimes](../api/user-findmeetingtimes.md) では常にその人は `Required` 型と見なされます。</span><span class="sxs-lookup"><span data-stu-id="a8d22-p101">The type of attendee. Possible values are: `required`, `optional`, `resource`. Currently if the attendee is a person, [findMeetingTimes](../api/user-findmeetingtimes.md) always considers the person is of the `Required` type.</span></span>|
|<span data-ttu-id="a8d22-117">emailAddress</span><span class="sxs-lookup"><span data-stu-id="a8d22-117">emailAddress</span></span>|[<span data-ttu-id="a8d22-118">emailAddress</span><span class="sxs-lookup"><span data-stu-id="a8d22-118">emailAddress</span></span>](emailaddress.md)|<span data-ttu-id="a8d22-119">参加者の名前と SMTP アドレスが含まれます。</span><span class="sxs-lookup"><span data-stu-id="a8d22-119">Includes the name and SMTP address of the attendee.</span></span>|

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
