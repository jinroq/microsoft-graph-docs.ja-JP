---
title: attendeeBase リソースの種類
description: 出席者の種類です。
localization_priority: Normal
ms.openlocfilehash: d009ef6a58c63017addf8b8a1bdecc1974abbff3
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32569355"
---
# <a name="attendeebase-resource-type"></a><span data-ttu-id="f37c8-103">attendeeBase リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f37c8-103">attendeeBase resource type</span></span>

<span data-ttu-id="f37c8-104">出席者の種類です。</span><span class="sxs-lookup"><span data-stu-id="f37c8-104">The type of attendee.</span></span>

<span data-ttu-id="f37c8-105">[recipient](recipient.md) から派生します。</span><span class="sxs-lookup"><span data-stu-id="f37c8-105">Derived from [recipient](recipient.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="f37c8-106">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f37c8-106">JSON representation</span></span>

<span data-ttu-id="f37c8-107">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="f37c8-107">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="f37c8-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f37c8-108">Properties</span></span>
| <span data-ttu-id="f37c8-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f37c8-109">Property</span></span>     | <span data-ttu-id="f37c8-110">型</span><span class="sxs-lookup"><span data-stu-id="f37c8-110">Type</span></span>   |<span data-ttu-id="f37c8-111">説明</span><span class="sxs-lookup"><span data-stu-id="f37c8-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f37c8-112">type</span><span class="sxs-lookup"><span data-stu-id="f37c8-112">type</span></span>|<span data-ttu-id="f37c8-113">attendeeType</span><span class="sxs-lookup"><span data-stu-id="f37c8-113">attendeeType</span></span>| <span data-ttu-id="f37c8-114">出席者の種類です。</span><span class="sxs-lookup"><span data-stu-id="f37c8-114">The type of attendee.</span></span> <span data-ttu-id="f37c8-115">使用可能な値: `required`、`optional`、`resource`。</span><span class="sxs-lookup"><span data-stu-id="f37c8-115">The possible values are: `required`, `optional`, `resource`.</span></span> <span data-ttu-id="f37c8-116">現時点では、出席者が 1 人である場合、[findMeetingTimes](../api/user-findmeetingtimes.md) では常にその人は `Required` 型と見なされます。</span><span class="sxs-lookup"><span data-stu-id="f37c8-116">Currently if the attendee is a person, [findMeetingTimes](../api/user-findmeetingtimes.md) always considers the person is of the `Required` type.</span></span>|
|<span data-ttu-id="f37c8-117">emailAddress</span><span class="sxs-lookup"><span data-stu-id="f37c8-117">emailAddress</span></span>|[<span data-ttu-id="f37c8-118">emailAddress</span><span class="sxs-lookup"><span data-stu-id="f37c8-118">emailAddress</span></span>](emailaddress.md)|<span data-ttu-id="f37c8-119">参加者の名前と SMTP アドレスが含まれます。</span><span class="sxs-lookup"><span data-stu-id="f37c8-119">Includes the name and SMTP address of the attendee.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "attendeeBase resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
