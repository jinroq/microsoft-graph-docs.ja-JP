---
title: onenoteEntityHierarchyModel リソース
description: これは、OneNote のエンティティの基本型です。
author: Jewan-microsoft
ms.openlocfilehash: a142e9206aefbb118f21b2f1a85d00cbc4a3a315
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27362021"
---
# <a name="onenoteentityhierarchymodel-resource"></a><span data-ttu-id="c328e-103">onenoteEntityHierarchyModel リソース</span><span class="sxs-lookup"><span data-stu-id="c328e-103">onenoteEntityHierarchyModel resource</span></span>

<span data-ttu-id="c328e-104">これは、OneNote のエンティティの基本型です。</span><span class="sxs-lookup"><span data-stu-id="c328e-104">This is a base type for OneNote entities.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c328e-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c328e-105">JSON representation</span></span>

<span data-ttu-id="c328e-106">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="c328e-106">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "abstract": true,
  "baseType": "microsoft.graph.onenoteEntitySchemaObjectModel",
  "optionalProperties": [
    "self"
  ],
  "@odata.type": "microsoft.graph.onenoteEntityHierarchyModel"
}-->

```json
{
  "displayName": "string",
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "lastModifiedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "lastModifiedDateTime": "String (timestamp)"
}

```
## <a name="properties"></a><span data-ttu-id="c328e-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c328e-107">Properties</span></span>
## <a name="properties"></a><span data-ttu-id="c328e-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c328e-108">Properties</span></span>
| <span data-ttu-id="c328e-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c328e-109">Property</span></span>     | <span data-ttu-id="c328e-110">種類</span><span class="sxs-lookup"><span data-stu-id="c328e-110">Type</span></span>   |<span data-ttu-id="c328e-111">説明</span><span class="sxs-lookup"><span data-stu-id="c328e-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c328e-112">displayName</span><span class="sxs-lookup"><span data-stu-id="c328e-112">displayName</span></span>|<span data-ttu-id="c328e-113">String</span><span class="sxs-lookup"><span data-stu-id="c328e-113">String</span></span>|<span data-ttu-id="c328e-114">ノートブックの名前。</span><span class="sxs-lookup"><span data-stu-id="c328e-114">The name of the notebook.</span></span>|
|<span data-ttu-id="c328e-115">createdBy</span><span class="sxs-lookup"><span data-stu-id="c328e-115">createdBy</span></span>|[<span data-ttu-id="c328e-116">identitySet</span><span class="sxs-lookup"><span data-stu-id="c328e-116">identitySet</span></span>](identityset.md)|<span data-ttu-id="c328e-p101">そのアイテムを作成したユーザーの ID、デバイス、アプリケーション。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="c328e-p101">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="c328e-119">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="c328e-119">lastModifiedBy</span></span>|[<span data-ttu-id="c328e-120">identitySet</span><span class="sxs-lookup"><span data-stu-id="c328e-120">identitySet</span></span>](identityset.md)|<span data-ttu-id="c328e-p102">そのアイテムを作成したユーザーの ID、デバイス、アプリケーション。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="c328e-p102">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="c328e-123">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c328e-123">lastModifiedDateTime</span></span>|<span data-ttu-id="c328e-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c328e-124">DateTimeOffset</span></span>|<span data-ttu-id="c328e-p103">ノートブックが最後に変更された日時。Timestamp は、ISO 8601 形式を使用した日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="c328e-p103">The date and time when the notebook was last modified. The timestamp represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|

<!-- uuid: 8b1af557-1a7c-4432-86eb-94989c2d4b54
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "page resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->