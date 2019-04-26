---
title: attendeeBase リソースの種類
description: 出席者の種類です。
localization_priority: Normal
ms.openlocfilehash: a0095a2076cd09bee2d4b934bac29cd030924ec1
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33328581"
---
# <a name="attendeebase-resource-type"></a><span data-ttu-id="c9880-103">attendeeBase リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c9880-103">attendeeBase resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c9880-104">出席者の種類です。</span><span class="sxs-lookup"><span data-stu-id="c9880-104">The type of attendee.</span></span>

<span data-ttu-id="c9880-105">[recipient](recipient.md) から派生します。</span><span class="sxs-lookup"><span data-stu-id="c9880-105">Derived from [recipient](recipient.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="c9880-106">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c9880-106">JSON representation</span></span>

<span data-ttu-id="c9880-107">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="c9880-107">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="c9880-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c9880-108">Properties</span></span>
| <span data-ttu-id="c9880-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c9880-109">Property</span></span>     | <span data-ttu-id="c9880-110">型</span><span class="sxs-lookup"><span data-stu-id="c9880-110">Type</span></span>   |<span data-ttu-id="c9880-111">説明</span><span class="sxs-lookup"><span data-stu-id="c9880-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c9880-112">type</span><span class="sxs-lookup"><span data-stu-id="c9880-112">type</span></span>|<span data-ttu-id="c9880-113">String</span><span class="sxs-lookup"><span data-stu-id="c9880-113">String</span></span>| <span data-ttu-id="c9880-p101">出席者の種類です。使用可能な値: `required`、`optional`、`resource`。現時点では、出席者が 1 人である場合、[findMeetingTimes](../api/user-findmeetingtimes.md) では常にその人は `Required` 型と見なされます。</span><span class="sxs-lookup"><span data-stu-id="c9880-p101">The type of attendee. Possible values are: `required`, `optional`, `resource`. Currently if the attendee is a person, [findMeetingTimes](../api/user-findmeetingtimes.md) always considers the person is of the `Required` type.</span></span>|
|<span data-ttu-id="c9880-117">emailAddress</span><span class="sxs-lookup"><span data-stu-id="c9880-117">emailAddress</span></span>|[<span data-ttu-id="c9880-118">emailAddress</span><span class="sxs-lookup"><span data-stu-id="c9880-118">emailAddress</span></span>](emailaddress.md)|<span data-ttu-id="c9880-119">参加者の名前と SMTP アドレスが含まれます。</span><span class="sxs-lookup"><span data-stu-id="c9880-119">Includes the name and SMTP address of the attendee.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "attendeeBase resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
