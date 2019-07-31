---
title: attendeeBase リソースの種類
description: 出席者の種類です。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: dfa873daf5b3c5a47e10ab480292ffb11b656b01
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35974299"
---
# <a name="attendeebase-resource-type"></a><span data-ttu-id="0a09f-103">attendeeBase リソースの種類</span><span class="sxs-lookup"><span data-stu-id="0a09f-103">attendeeBase resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0a09f-104">出席者の種類です。</span><span class="sxs-lookup"><span data-stu-id="0a09f-104">The type of attendee.</span></span>

<span data-ttu-id="0a09f-105">[recipient](recipient.md) から派生します。</span><span class="sxs-lookup"><span data-stu-id="0a09f-105">Derived from [recipient](recipient.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="0a09f-106">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0a09f-106">JSON representation</span></span>

<span data-ttu-id="0a09f-107">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="0a09f-107">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="0a09f-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0a09f-108">Properties</span></span>
| <span data-ttu-id="0a09f-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0a09f-109">Property</span></span>     | <span data-ttu-id="0a09f-110">型</span><span class="sxs-lookup"><span data-stu-id="0a09f-110">Type</span></span>   |<span data-ttu-id="0a09f-111">説明</span><span class="sxs-lookup"><span data-stu-id="0a09f-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0a09f-112">type</span><span class="sxs-lookup"><span data-stu-id="0a09f-112">type</span></span>|<span data-ttu-id="0a09f-113">String</span><span class="sxs-lookup"><span data-stu-id="0a09f-113">String</span></span>| <span data-ttu-id="0a09f-p101">出席者の種類です。使用可能な値: `required`、`optional`、`resource`。現時点では、出席者が 1 人である場合、[findMeetingTimes](../api/user-findmeetingtimes.md) では常にその人は `Required` 型と見なされます。</span><span class="sxs-lookup"><span data-stu-id="0a09f-p101">The type of attendee. Possible values are: `required`, `optional`, `resource`. Currently if the attendee is a person, [findMeetingTimes](../api/user-findmeetingtimes.md) always considers the person is of the `Required` type.</span></span>|
|<span data-ttu-id="0a09f-117">emailAddress</span><span class="sxs-lookup"><span data-stu-id="0a09f-117">emailAddress</span></span>|[<span data-ttu-id="0a09f-118">emailAddress</span><span class="sxs-lookup"><span data-stu-id="0a09f-118">emailAddress</span></span>](emailaddress.md)|<span data-ttu-id="0a09f-119">参加者の名前と SMTP アドレスが含まれます。</span><span class="sxs-lookup"><span data-stu-id="0a09f-119">Includes the name and SMTP address of the attendee.</span></span>|

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
