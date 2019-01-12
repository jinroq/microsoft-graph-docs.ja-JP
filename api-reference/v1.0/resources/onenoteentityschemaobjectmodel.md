---
title: onenoteEntitySchemaObjectModel リソース
description: これは、OneNote のエンティティの基本型です。
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: 168359bbdaa659db461aa33af96e402a4a81783d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27978712"
---
# <a name="onenoteentityschemaobjectmodel-resource"></a><span data-ttu-id="2762d-103">onenoteEntitySchemaObjectModel リソース</span><span class="sxs-lookup"><span data-stu-id="2762d-103">onenoteEntitySchemaObjectModel resource</span></span>

<span data-ttu-id="2762d-104">これは、OneNote のエンティティの基本型です。</span><span class="sxs-lookup"><span data-stu-id="2762d-104">This is a base type for OneNote entities.</span></span>

## <a name="json-representation"></a><span data-ttu-id="2762d-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="2762d-105">JSON representation</span></span>

<span data-ttu-id="2762d-106">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="2762d-106">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="2762d-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2762d-107">Properties</span></span>
| <span data-ttu-id="2762d-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2762d-108">Property</span></span>     | <span data-ttu-id="2762d-109">種類</span><span class="sxs-lookup"><span data-stu-id="2762d-109">Type</span></span>   |<span data-ttu-id="2762d-110">説明</span><span class="sxs-lookup"><span data-stu-id="2762d-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2762d-111">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2762d-111">createdDateTime</span></span>|<span data-ttu-id="2762d-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2762d-112">DateTimeOffset</span></span>|<span data-ttu-id="2762d-p101">ページが作成された日時。Timestamp は、ISO 8601 形式を使用した日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="2762d-p101">The date and time when the page was created. The timestamp represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|

<!-- uuid: bfb567de-2a2a-4b81-bf47-a55626a0c166
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "page resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
