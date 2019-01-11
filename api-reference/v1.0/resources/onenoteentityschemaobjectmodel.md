---
title: onenoteEntitySchemaObjectModel リソース
description: これは、OneNote のエンティティの基本型です。
author: Jewan-microsoft
localization_priority: Normal
ms.openlocfilehash: 9ecdb17d48f8c8682af5970ea468fb2ad0118bbb
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27843884"
---
# <a name="onenoteentityschemaobjectmodel-resource"></a><span data-ttu-id="89867-103">onenoteEntitySchemaObjectModel リソース</span><span class="sxs-lookup"><span data-stu-id="89867-103">onenoteEntitySchemaObjectModel resource</span></span>

<span data-ttu-id="89867-104">これは、OneNote のエンティティの基本型です。</span><span class="sxs-lookup"><span data-stu-id="89867-104">This is a base type for OneNote entities.</span></span>

## <a name="json-representation"></a><span data-ttu-id="89867-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="89867-105">JSON representation</span></span>

<span data-ttu-id="89867-106">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="89867-106">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="89867-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="89867-107">Properties</span></span>
| <span data-ttu-id="89867-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="89867-108">Property</span></span>     | <span data-ttu-id="89867-109">種類</span><span class="sxs-lookup"><span data-stu-id="89867-109">Type</span></span>   |<span data-ttu-id="89867-110">説明</span><span class="sxs-lookup"><span data-stu-id="89867-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="89867-111">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="89867-111">createdDateTime</span></span>|<span data-ttu-id="89867-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="89867-112">DateTimeOffset</span></span>|<span data-ttu-id="89867-p101">ページが作成された日時。Timestamp は、ISO 8601 形式を使用した日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="89867-p101">The date and time when the page was created. The timestamp represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|

<!-- uuid: bfb567de-2a2a-4b81-bf47-a55626a0c166
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "page resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
