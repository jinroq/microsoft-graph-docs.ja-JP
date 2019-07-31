---
title: attendeeAvailability リソースの種類
description: 出席者の空き時間。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 8e9a9eb91ccfc70e771357abf3b91d6a23dbd367
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36013256"
---
# <a name="attendeeavailability-resource-type"></a><span data-ttu-id="2d7b7-103">attendeeAvailability リソースの種類</span><span class="sxs-lookup"><span data-stu-id="2d7b7-103">attendeeAvailability resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2d7b7-104">出席者の空き時間。</span><span class="sxs-lookup"><span data-stu-id="2d7b7-104">The availability of an attendee.</span></span>

## <a name="json-representation"></a><span data-ttu-id="2d7b7-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="2d7b7-105">JSON representation</span></span>

<span data-ttu-id="2d7b7-106">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="2d7b7-106">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="2d7b7-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2d7b7-107">Properties</span></span>
| <span data-ttu-id="2d7b7-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2d7b7-108">Property</span></span>     | <span data-ttu-id="2d7b7-109">型</span><span class="sxs-lookup"><span data-stu-id="2d7b7-109">Type</span></span>   |<span data-ttu-id="2d7b7-110">説明</span><span class="sxs-lookup"><span data-stu-id="2d7b7-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2d7b7-111">attendee</span><span class="sxs-lookup"><span data-stu-id="2d7b7-111">attendee</span></span>|[<span data-ttu-id="2d7b7-112">attendeeBase</span><span class="sxs-lookup"><span data-stu-id="2d7b7-112">attendeeBase</span></span>](attendeebase.md)|<span data-ttu-id="2d7b7-113">出席者の電子メールアドレスと種類。個人またはリソースのいずれかを指定します。また、必要かどうかは、ユーザーの場合はオプションです。</span><span class="sxs-lookup"><span data-stu-id="2d7b7-113">The email address and type of attendee - whether it's a person or a resource, and whether required or optional if it's a person.</span></span>|
|<span data-ttu-id="2d7b7-114">availability</span><span class="sxs-lookup"><span data-stu-id="2d7b7-114">availability</span></span>|<span data-ttu-id="2d7b7-115">freeBusyStatus</span><span class="sxs-lookup"><span data-stu-id="2d7b7-115">freeBusyStatus</span></span>| <span data-ttu-id="2d7b7-p101">出席者の空き時間の状態。使用可能な値: `free`、`tentative`、`busy`、`oof`、`workingElsewhere`、`unknown`。</span><span class="sxs-lookup"><span data-stu-id="2d7b7-p101">The availability status of the attendee. Possible values are: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "attendeeAvailability resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
