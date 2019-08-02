---
title: onenoteEntitySchemaObjectModel リソース
description: これは、OneNote エンティティの基本型です。
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
doc_type: resourcePageType
ms.openlocfilehash: 4072a6d02ffb003731613c081effac50215f605a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36035813"
---
# <a name="onenoteentityschemaobjectmodel-resource"></a><span data-ttu-id="7010f-103">onenoteEntitySchemaObjectModel リソース</span><span class="sxs-lookup"><span data-stu-id="7010f-103">onenoteEntitySchemaObjectModel resource</span></span>

<span data-ttu-id="7010f-104">これは、OneNote エンティティの基本型です。</span><span class="sxs-lookup"><span data-stu-id="7010f-104">This is a base type for OneNote entities.</span></span>

## <a name="json-representation"></a><span data-ttu-id="7010f-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="7010f-105">JSON representation</span></span>

<span data-ttu-id="7010f-106">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="7010f-106">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "abstract": true,
  "baseType": "microsoft.graph.onenoteEntityBaseModel",
  "optionalProperties": [
    "self"
  ],
  "@odata.type": "microsoft.graph.onenoteEntitySchemaObjectModel"
}-->

```json
{
  "createdDateTime": "String (timestamp)"
}

```
## <a name="properties"></a><span data-ttu-id="7010f-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7010f-107">Properties</span></span>
| <span data-ttu-id="7010f-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7010f-108">Property</span></span>     | <span data-ttu-id="7010f-109">型</span><span class="sxs-lookup"><span data-stu-id="7010f-109">Type</span></span>   |<span data-ttu-id="7010f-110">説明</span><span class="sxs-lookup"><span data-stu-id="7010f-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7010f-111">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7010f-111">createdDateTime</span></span>|<span data-ttu-id="7010f-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7010f-112">DateTimeOffset</span></span>|<span data-ttu-id="7010f-113">ページが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="7010f-113">The date and time when the page was created.</span></span> <span data-ttu-id="7010f-114">Timestamp は、ISO 8601 形式を使用した日付と時刻の情報を表し、必ず UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="7010f-114">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="7010f-115">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="7010f-115">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="7010f-116">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="7010f-116">Read-only.</span></span>|

<!-- uuid: bfb567de-2a2a-4b81-bf47-a55626a0c166
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "page resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
