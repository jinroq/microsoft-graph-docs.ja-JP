---
title: attendeeAvailability リソースの種類
description: 出席者の空き時間。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 63014553824b833e2e4cdfb03485fcb7962c01a0
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32569362"
---
# <a name="attendeeavailability-resource-type"></a><span data-ttu-id="75a78-103">attendeeAvailability リソースの種類</span><span class="sxs-lookup"><span data-stu-id="75a78-103">attendeeAvailability resource type</span></span>

<span data-ttu-id="75a78-104">出席者の空き時間。</span><span class="sxs-lookup"><span data-stu-id="75a78-104">The availability of an attendee.</span></span>

## <a name="json-representation"></a><span data-ttu-id="75a78-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="75a78-105">JSON representation</span></span>

<span data-ttu-id="75a78-106">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="75a78-106">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.attendeeAvailability"
}-->

```json
{
  "attendee": {"@odata.type": "microsoft.graph.attendeeBase"},
  "availability": "String"
}

```
## <a name="properties"></a><span data-ttu-id="75a78-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="75a78-107">Properties</span></span>
| <span data-ttu-id="75a78-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="75a78-108">Property</span></span>     | <span data-ttu-id="75a78-109">型</span><span class="sxs-lookup"><span data-stu-id="75a78-109">Type</span></span>   |<span data-ttu-id="75a78-110">説明</span><span class="sxs-lookup"><span data-stu-id="75a78-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="75a78-111">attendee</span><span class="sxs-lookup"><span data-stu-id="75a78-111">attendee</span></span>|[<span data-ttu-id="75a78-112">attendeeBase</span><span class="sxs-lookup"><span data-stu-id="75a78-112">attendeeBase</span></span>](attendeebase.md)|<span data-ttu-id="75a78-113">出席者の電子メールアドレスと種類。個人またはリソースのいずれかを指定します。また、必要かどうかは、ユーザーの場合はオプションです。</span><span class="sxs-lookup"><span data-stu-id="75a78-113">The email address and type of attendee - whether it's a person or a resource, and whether required or optional if it's a person.</span></span>|
|<span data-ttu-id="75a78-114">availability</span><span class="sxs-lookup"><span data-stu-id="75a78-114">availability</span></span>|<span data-ttu-id="75a78-115">freeBusyStatus</span><span class="sxs-lookup"><span data-stu-id="75a78-115">freeBusyStatus</span></span>| <span data-ttu-id="75a78-116">出席者の空き時間の状態。</span><span class="sxs-lookup"><span data-stu-id="75a78-116">The availability status of the attendee.</span></span> <span data-ttu-id="75a78-117">使用可能な値は`free`、 `tentative`、 `busy` `oof` `workingElsewhere`、、、 `unknown`、です。</span><span class="sxs-lookup"><span data-stu-id="75a78-117">The possible values are: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "attendeeAvailability resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
