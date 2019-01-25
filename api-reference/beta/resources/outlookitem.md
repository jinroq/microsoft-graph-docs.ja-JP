---
title: outlookItem リソースの種類
description: 以下は、リソースの JSON 表記です
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 8a44f9a2e568991c6803ebf72baf5f712f39ba64
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29528292"
---
# <a name="outlookitem-resource-type"></a><span data-ttu-id="c8e95-103">outlookItem リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c8e95-103">outlookItem resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="json-representation"></a><span data-ttu-id="c8e95-104">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c8e95-104">JSON representation</span></span>

<span data-ttu-id="c8e95-105">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="c8e95-105">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.outlookitem"
}-->

```json
{
  "categories": ["string"],
  "changeKey": "string",
  "createdDateTime": "String (timestamp)",
  "id": "string (identifier)",
  "lastModifiedDateTime": "String (timestamp)"
}

```
## <a name="properties"></a><span data-ttu-id="c8e95-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c8e95-106">Properties</span></span>
| <span data-ttu-id="c8e95-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c8e95-107">Property</span></span>     | <span data-ttu-id="c8e95-108">型</span><span class="sxs-lookup"><span data-stu-id="c8e95-108">Type</span></span>   |<span data-ttu-id="c8e95-109">説明</span><span class="sxs-lookup"><span data-stu-id="c8e95-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c8e95-110">categories</span><span class="sxs-lookup"><span data-stu-id="c8e95-110">categories</span></span>|<span data-ttu-id="c8e95-111">String コレクション</span><span class="sxs-lookup"><span data-stu-id="c8e95-111">String collection</span></span>||
|<span data-ttu-id="c8e95-112">changeKey</span><span class="sxs-lookup"><span data-stu-id="c8e95-112">changeKey</span></span>|<span data-ttu-id="c8e95-113">String</span><span class="sxs-lookup"><span data-stu-id="c8e95-113">String</span></span>||
|<span data-ttu-id="c8e95-114">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c8e95-114">createdDateTime</span></span>|<span data-ttu-id="c8e95-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c8e95-115">DateTimeOffset</span></span>|<span data-ttu-id="c8e95-p101">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="c8e95-p101">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="c8e95-118">id</span><span class="sxs-lookup"><span data-stu-id="c8e95-118">id</span></span>|<span data-ttu-id="c8e95-119">String</span><span class="sxs-lookup"><span data-stu-id="c8e95-119">String</span></span>| <span data-ttu-id="c8e95-120">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="c8e95-120">Read-only.</span></span>|
|<span data-ttu-id="c8e95-121">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c8e95-121">lastModifiedDateTime</span></span>|<span data-ttu-id="c8e95-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c8e95-122">DateTimeOffset</span></span>|<span data-ttu-id="c8e95-p102">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="c8e95-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|

## <a name="relationships"></a><span data-ttu-id="c8e95-125">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="c8e95-125">Relationships</span></span>
<span data-ttu-id="c8e95-126">なし</span><span class="sxs-lookup"><span data-stu-id="c8e95-126">None</span></span>


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "outlookItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/outlookitem.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
