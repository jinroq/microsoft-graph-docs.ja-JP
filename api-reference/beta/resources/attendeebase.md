---
title: attendeeBase リソースの種類
description: 出席者の種類です。
ms.openlocfilehash: 2d7d3889cd65886eba4cf9356862417928ed3296
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27066476"
---
# <a name="attendeebase-resource-type"></a><span data-ttu-id="b23cd-103">attendeeBase リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b23cd-103">attendeeBase resource type</span></span>

> <span data-ttu-id="b23cd-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="b23cd-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b23cd-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b23cd-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b23cd-106">出席者の種類です。</span><span class="sxs-lookup"><span data-stu-id="b23cd-106">The type of attendee.</span></span>

<span data-ttu-id="b23cd-107">[recipient](recipient.md) から派生します。</span><span class="sxs-lookup"><span data-stu-id="b23cd-107">Derived from [recipient](recipient.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="b23cd-108">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b23cd-108">JSON representation</span></span>

<span data-ttu-id="b23cd-109">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="b23cd-109">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="b23cd-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b23cd-110">Properties</span></span>
| <span data-ttu-id="b23cd-111">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b23cd-111">Property</span></span>     | <span data-ttu-id="b23cd-112">型</span><span class="sxs-lookup"><span data-stu-id="b23cd-112">Type</span></span>   |<span data-ttu-id="b23cd-113">説明</span><span class="sxs-lookup"><span data-stu-id="b23cd-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b23cd-114">type</span><span class="sxs-lookup"><span data-stu-id="b23cd-114">type</span></span>|<span data-ttu-id="b23cd-115">String</span><span class="sxs-lookup"><span data-stu-id="b23cd-115">String</span></span>| <span data-ttu-id="b23cd-p102">出席者の種類です。使用可能な値: `required`、`optional`、`resource`。現時点では、出席者が 1 人である場合、[findMeetingTimes](../api/user-findmeetingtimes.md) では常にその人は `Required` 型と見なされます。</span><span class="sxs-lookup"><span data-stu-id="b23cd-p102">The type of attendee. Possible values are: `required`, `optional`, `resource`. Currently if the attendee is a person, [findMeetingTimes](../api/user-findmeetingtimes.md) always considers the person is of the `Required` type.</span></span>|
|<span data-ttu-id="b23cd-119">emailAddress</span><span class="sxs-lookup"><span data-stu-id="b23cd-119">emailAddress</span></span>|[<span data-ttu-id="b23cd-120">emailAddress</span><span class="sxs-lookup"><span data-stu-id="b23cd-120">emailAddress</span></span>](emailaddress.md)|<span data-ttu-id="b23cd-121">参加者の名前と SMTP アドレスが含まれます。</span><span class="sxs-lookup"><span data-stu-id="b23cd-121">Includes the name and SMTP address of the attendee.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "attendeeBase resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->