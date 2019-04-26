---
title: attendeeAvailability リソースの種類
description: 出席者の空き時間。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 95896808f1a58eb77cafb8003ca5c7848d50bc08
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33339022"
---
# <a name="attendeeavailability-resource-type"></a><span data-ttu-id="99b0d-103">attendeeAvailability リソースの種類</span><span class="sxs-lookup"><span data-stu-id="99b0d-103">attendeeAvailability resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="99b0d-104">出席者の空き時間。</span><span class="sxs-lookup"><span data-stu-id="99b0d-104">The availability of an attendee.</span></span>

## <a name="json-representation"></a><span data-ttu-id="99b0d-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="99b0d-105">JSON representation</span></span>

<span data-ttu-id="99b0d-106">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="99b0d-106">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="99b0d-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="99b0d-107">Properties</span></span>
| <span data-ttu-id="99b0d-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="99b0d-108">Property</span></span>     | <span data-ttu-id="99b0d-109">型</span><span class="sxs-lookup"><span data-stu-id="99b0d-109">Type</span></span>   |<span data-ttu-id="99b0d-110">説明</span><span class="sxs-lookup"><span data-stu-id="99b0d-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="99b0d-111">attendee</span><span class="sxs-lookup"><span data-stu-id="99b0d-111">attendee</span></span>|[<span data-ttu-id="99b0d-112">attendeeBase</span><span class="sxs-lookup"><span data-stu-id="99b0d-112">attendeeBase</span></span>](attendeebase.md)|<span data-ttu-id="99b0d-113">出席者の電子メールアドレスと種類。個人またはリソースのいずれかを指定します。また、必要かどうかは、ユーザーの場合はオプションです。</span><span class="sxs-lookup"><span data-stu-id="99b0d-113">The email address and type of attendee - whether it's a person or a resource, and whether required or optional if it's a person.</span></span>|
|<span data-ttu-id="99b0d-114">availability</span><span class="sxs-lookup"><span data-stu-id="99b0d-114">availability</span></span>|<span data-ttu-id="99b0d-115">freeBusyStatus</span><span class="sxs-lookup"><span data-stu-id="99b0d-115">freeBusyStatus</span></span>| <span data-ttu-id="99b0d-p101">出席者の空き時間の状態。使用可能な値: `free`、`tentative`、`busy`、`oof`、`workingElsewhere`、`unknown`。</span><span class="sxs-lookup"><span data-stu-id="99b0d-p101">The availability status of the attendee. Possible values are: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span></span>|

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
