---
title: outlookItem リソースの種類
description: 以下は、リソースの JSON 表記です
ms.openlocfilehash: 5f81598b62d2b47230f4a7ce16d17b8056bc9874
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27020996"
---
# <a name="outlookitem-resource-type"></a><span data-ttu-id="1cea6-103">outlookItem リソースの種類</span><span class="sxs-lookup"><span data-stu-id="1cea6-103">outlookItem resource type</span></span>



## <a name="json-representation"></a><span data-ttu-id="1cea6-104">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="1cea6-104">JSON representation</span></span>

<span data-ttu-id="1cea6-105">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="1cea6-105">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="1cea6-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1cea6-106">Properties</span></span>
| <span data-ttu-id="1cea6-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1cea6-107">Property</span></span>     | <span data-ttu-id="1cea6-108">型</span><span class="sxs-lookup"><span data-stu-id="1cea6-108">Type</span></span>   |<span data-ttu-id="1cea6-109">説明</span><span class="sxs-lookup"><span data-stu-id="1cea6-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1cea6-110">categories</span><span class="sxs-lookup"><span data-stu-id="1cea6-110">categories</span></span>|<span data-ttu-id="1cea6-111">String コレクション</span><span class="sxs-lookup"><span data-stu-id="1cea6-111">String collection</span></span>|<span data-ttu-id="1cea6-112">アイテムに関連付けられているカテゴリ</span><span class="sxs-lookup"><span data-stu-id="1cea6-112">The categories associated with the item</span></span>|
|<span data-ttu-id="1cea6-113">changeKey</span><span class="sxs-lookup"><span data-stu-id="1cea6-113">changeKey</span></span>|<span data-ttu-id="1cea6-114">String</span><span class="sxs-lookup"><span data-stu-id="1cea6-114">String</span></span>|<span data-ttu-id="1cea6-115">項目のバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="1cea6-115">Identifies the version of the item.</span></span> <span data-ttu-id="1cea6-116">たびにアイテムが変更されると、変更キーを同様に変更します。</span><span class="sxs-lookup"><span data-stu-id="1cea6-116">Every time the item is changed, changeKey changes as well.</span></span> <span data-ttu-id="1cea6-117">これにより、Exchange オブジェクトの適切なバージョンに変更を適用します。</span><span class="sxs-lookup"><span data-stu-id="1cea6-117">This allows Exchange to apply changes to the correct version of the object.</span></span> <span data-ttu-id="1cea6-118">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="1cea6-118">Read-only.</span></span>|
|<span data-ttu-id="1cea6-119">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1cea6-119">createdDateTime</span></span>|<span data-ttu-id="1cea6-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1cea6-120">DateTimeOffset</span></span>|<span data-ttu-id="1cea6-p102">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="1cea6-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="1cea6-123">id</span><span class="sxs-lookup"><span data-stu-id="1cea6-123">id</span></span>|<span data-ttu-id="1cea6-124">String</span><span class="sxs-lookup"><span data-stu-id="1cea6-124">String</span></span>| <span data-ttu-id="1cea6-125">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="1cea6-125">Read-only.</span></span>|
|<span data-ttu-id="1cea6-126">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1cea6-126">lastModifiedDateTime</span></span>|<span data-ttu-id="1cea6-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1cea6-127">DateTimeOffset</span></span>|<span data-ttu-id="1cea6-p103">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="1cea6-p103">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|

## <a name="relationships"></a><span data-ttu-id="1cea6-130">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="1cea6-130">Relationships</span></span>
<span data-ttu-id="1cea6-131">なし</span><span class="sxs-lookup"><span data-stu-id="1cea6-131">None</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "outlookItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
