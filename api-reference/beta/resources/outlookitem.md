---
title: outlookItem リソースの種類
description: 以下は、リソースの JSON 表記です
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 8a44f9a2e568991c6803ebf72baf5f712f39ba64
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32568651"
---
# <a name="outlookitem-resource-type"></a><span data-ttu-id="936ed-103">outlookItem リソースの種類</span><span class="sxs-lookup"><span data-stu-id="936ed-103">outlookItem resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="json-representation"></a><span data-ttu-id="936ed-104">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="936ed-104">JSON representation</span></span>

<span data-ttu-id="936ed-105">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="936ed-105">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="936ed-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="936ed-106">Properties</span></span>
| <span data-ttu-id="936ed-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="936ed-107">Property</span></span>     | <span data-ttu-id="936ed-108">型</span><span class="sxs-lookup"><span data-stu-id="936ed-108">Type</span></span>   |<span data-ttu-id="936ed-109">説明</span><span class="sxs-lookup"><span data-stu-id="936ed-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="936ed-110">categories</span><span class="sxs-lookup"><span data-stu-id="936ed-110">categories</span></span>|<span data-ttu-id="936ed-111">String collection</span><span class="sxs-lookup"><span data-stu-id="936ed-111">String collection</span></span>||
|<span data-ttu-id="936ed-112">changeKey</span><span class="sxs-lookup"><span data-stu-id="936ed-112">changeKey</span></span>|<span data-ttu-id="936ed-113">String</span><span class="sxs-lookup"><span data-stu-id="936ed-113">String</span></span>||
|<span data-ttu-id="936ed-114">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="936ed-114">createdDateTime</span></span>|<span data-ttu-id="936ed-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="936ed-115">DateTimeOffset</span></span>|<span data-ttu-id="936ed-p101">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="936ed-p101">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="936ed-118">id</span><span class="sxs-lookup"><span data-stu-id="936ed-118">id</span></span>|<span data-ttu-id="936ed-119">String</span><span class="sxs-lookup"><span data-stu-id="936ed-119">String</span></span>| <span data-ttu-id="936ed-120">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="936ed-120">Read-only.</span></span>|
|<span data-ttu-id="936ed-121">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="936ed-121">lastModifiedDateTime</span></span>|<span data-ttu-id="936ed-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="936ed-122">DateTimeOffset</span></span>|<span data-ttu-id="936ed-p102">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="936ed-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|

## <a name="relationships"></a><span data-ttu-id="936ed-125">関係</span><span class="sxs-lookup"><span data-stu-id="936ed-125">Relationships</span></span>
<span data-ttu-id="936ed-126">なし</span><span class="sxs-lookup"><span data-stu-id="936ed-126">None</span></span>


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
