---
title: outlookItem リソースの種類
description: 以下は、リソースの JSON 表記です
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 77741fa05f356418e688cdc4a45c5a4750604c3c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36009280"
---
# <a name="outlookitem-resource-type"></a><span data-ttu-id="1d26a-103">outlookItem リソースの種類</span><span class="sxs-lookup"><span data-stu-id="1d26a-103">outlookItem resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="json-representation"></a><span data-ttu-id="1d26a-104">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="1d26a-104">JSON representation</span></span>

<span data-ttu-id="1d26a-105">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="1d26a-105">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.outlookItem"
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
## <a name="properties"></a><span data-ttu-id="1d26a-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1d26a-106">Properties</span></span>
| <span data-ttu-id="1d26a-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1d26a-107">Property</span></span>     | <span data-ttu-id="1d26a-108">型</span><span class="sxs-lookup"><span data-stu-id="1d26a-108">Type</span></span>   |<span data-ttu-id="1d26a-109">説明</span><span class="sxs-lookup"><span data-stu-id="1d26a-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1d26a-110">categories</span><span class="sxs-lookup"><span data-stu-id="1d26a-110">categories</span></span>|<span data-ttu-id="1d26a-111">String collection</span><span class="sxs-lookup"><span data-stu-id="1d26a-111">String collection</span></span>||
|<span data-ttu-id="1d26a-112">changeKey</span><span class="sxs-lookup"><span data-stu-id="1d26a-112">changeKey</span></span>|<span data-ttu-id="1d26a-113">String</span><span class="sxs-lookup"><span data-stu-id="1d26a-113">String</span></span>||
|<span data-ttu-id="1d26a-114">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1d26a-114">createdDateTime</span></span>|<span data-ttu-id="1d26a-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1d26a-115">DateTimeOffset</span></span>|<span data-ttu-id="1d26a-p101">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="1d26a-p101">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="1d26a-118">id</span><span class="sxs-lookup"><span data-stu-id="1d26a-118">id</span></span>|<span data-ttu-id="1d26a-119">String</span><span class="sxs-lookup"><span data-stu-id="1d26a-119">String</span></span>| <span data-ttu-id="1d26a-120">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="1d26a-120">Read-only.</span></span>|
|<span data-ttu-id="1d26a-121">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1d26a-121">lastModifiedDateTime</span></span>|<span data-ttu-id="1d26a-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1d26a-122">DateTimeOffset</span></span>|<span data-ttu-id="1d26a-p102">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="1d26a-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|

## <a name="relationships"></a><span data-ttu-id="1d26a-125">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="1d26a-125">Relationships</span></span>
<span data-ttu-id="1d26a-126">None</span><span class="sxs-lookup"><span data-stu-id="1d26a-126">None</span></span>


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "outlookItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
