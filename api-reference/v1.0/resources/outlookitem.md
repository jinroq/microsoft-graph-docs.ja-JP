---
title: outlookItem リソースの種類
description: 以下は、リソースの JSON 表記です
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 7b04d84019cbb38f78ef1df63e4e39480c4d949b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36035659"
---
# <a name="outlookitem-resource-type"></a><span data-ttu-id="63eb0-103">outlookItem リソースの種類</span><span class="sxs-lookup"><span data-stu-id="63eb0-103">outlookItem resource type</span></span>



## <a name="json-representation"></a><span data-ttu-id="63eb0-104">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="63eb0-104">JSON representation</span></span>

<span data-ttu-id="63eb0-105">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="63eb0-105">Here is a JSON representation of the resource</span></span>

<!--{
  "blockType": "resource",
  "abstract": true,
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
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
## <a name="properties"></a><span data-ttu-id="63eb0-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="63eb0-106">Properties</span></span>
| <span data-ttu-id="63eb0-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="63eb0-107">Property</span></span>     | <span data-ttu-id="63eb0-108">型</span><span class="sxs-lookup"><span data-stu-id="63eb0-108">Type</span></span>   |<span data-ttu-id="63eb0-109">説明</span><span class="sxs-lookup"><span data-stu-id="63eb0-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="63eb0-110">categories</span><span class="sxs-lookup"><span data-stu-id="63eb0-110">categories</span></span>|<span data-ttu-id="63eb0-111">String collection</span><span class="sxs-lookup"><span data-stu-id="63eb0-111">String collection</span></span>|<span data-ttu-id="63eb0-112">アイテムに関連付けられているカテゴリ</span><span class="sxs-lookup"><span data-stu-id="63eb0-112">The categories associated with the item</span></span>|
|<span data-ttu-id="63eb0-113">changeKey</span><span class="sxs-lookup"><span data-stu-id="63eb0-113">changeKey</span></span>|<span data-ttu-id="63eb0-114">String</span><span class="sxs-lookup"><span data-stu-id="63eb0-114">String</span></span>|<span data-ttu-id="63eb0-115">アイテムのバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="63eb0-115">Identifies the version of the item.</span></span> <span data-ttu-id="63eb0-116">項目が変更されるたびに、changeKey も変更されます。</span><span class="sxs-lookup"><span data-stu-id="63eb0-116">Every time the item is changed, changeKey changes as well.</span></span> <span data-ttu-id="63eb0-117">これにより、Exchange は正しいバージョンのオブジェクトに変更を適用できます。</span><span class="sxs-lookup"><span data-stu-id="63eb0-117">This allows Exchange to apply changes to the correct version of the object.</span></span> <span data-ttu-id="63eb0-118">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="63eb0-118">Read-only.</span></span>|
|<span data-ttu-id="63eb0-119">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="63eb0-119">createdDateTime</span></span>|<span data-ttu-id="63eb0-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="63eb0-120">DateTimeOffset</span></span>|<span data-ttu-id="63eb0-p102">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="63eb0-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="63eb0-123">id</span><span class="sxs-lookup"><span data-stu-id="63eb0-123">id</span></span>|<span data-ttu-id="63eb0-124">String</span><span class="sxs-lookup"><span data-stu-id="63eb0-124">String</span></span>| <span data-ttu-id="63eb0-125">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="63eb0-125">Read-only.</span></span>|
|<span data-ttu-id="63eb0-126">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="63eb0-126">lastModifiedDateTime</span></span>|<span data-ttu-id="63eb0-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="63eb0-127">DateTimeOffset</span></span>|<span data-ttu-id="63eb0-p103">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="63eb0-p103">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|

## <a name="relationships"></a><span data-ttu-id="63eb0-130">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="63eb0-130">Relationships</span></span>
<span data-ttu-id="63eb0-131">None</span><span class="sxs-lookup"><span data-stu-id="63eb0-131">None</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "outlookItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
