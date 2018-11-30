---
title: attendeeBase リソースの種類
description: 出席者の種類です。
ms.openlocfilehash: 6995ac94a600a60313ef26208b441c6ef6fdf001
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27022828"
---
# <a name="attendeebase-resource-type"></a><span data-ttu-id="3e1ec-103">attendeeBase リソースの種類</span><span class="sxs-lookup"><span data-stu-id="3e1ec-103">attendeeBase resource type</span></span>

<span data-ttu-id="3e1ec-104">出席者の種類です。</span><span class="sxs-lookup"><span data-stu-id="3e1ec-104">The type of attendee.</span></span>

<span data-ttu-id="3e1ec-105">[recipient](recipient.md) から派生します。</span><span class="sxs-lookup"><span data-stu-id="3e1ec-105">Derived from [recipient](recipient.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="3e1ec-106">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="3e1ec-106">JSON representation</span></span>

<span data-ttu-id="3e1ec-107">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="3e1ec-107">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="3e1ec-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3e1ec-108">Properties</span></span>
| <span data-ttu-id="3e1ec-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3e1ec-109">Property</span></span>     | <span data-ttu-id="3e1ec-110">型</span><span class="sxs-lookup"><span data-stu-id="3e1ec-110">Type</span></span>   |<span data-ttu-id="3e1ec-111">説明</span><span class="sxs-lookup"><span data-stu-id="3e1ec-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3e1ec-112">type</span><span class="sxs-lookup"><span data-stu-id="3e1ec-112">type</span></span>|<span data-ttu-id="3e1ec-113">attendeeType</span><span class="sxs-lookup"><span data-stu-id="3e1ec-113">attendeeType</span></span>| <span data-ttu-id="3e1ec-114">出席者の種類です。</span><span class="sxs-lookup"><span data-stu-id="3e1ec-114">The type of attendee.</span></span> <span data-ttu-id="3e1ec-115">可能な値: `required`、 `optional`、 `resource`。</span><span class="sxs-lookup"><span data-stu-id="3e1ec-115">The possible values are: `required`, `optional`, `resource`.</span></span> <span data-ttu-id="3e1ec-116">現在、出席者が人間の場合は、 [findMeetingTimes](../api/user-findmeetingtimes.md)は一切の人では、`Required`型です。</span><span class="sxs-lookup"><span data-stu-id="3e1ec-116">Currently if the attendee is a person, [findMeetingTimes](../api/user-findmeetingtimes.md) always considers the person is of the `Required` type.</span></span>|
|<span data-ttu-id="3e1ec-117">emailAddress</span><span class="sxs-lookup"><span data-stu-id="3e1ec-117">emailAddress</span></span>|[<span data-ttu-id="3e1ec-118">emailAddress</span><span class="sxs-lookup"><span data-stu-id="3e1ec-118">emailAddress</span></span>](emailaddress.md)|<span data-ttu-id="3e1ec-119">参加者の名前と SMTP アドレスが含まれます。</span><span class="sxs-lookup"><span data-stu-id="3e1ec-119">Includes the name and SMTP address of the attendee.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "attendeeBase resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
