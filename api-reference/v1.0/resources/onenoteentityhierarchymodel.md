---
title: onenoteEntityHierarchyModel リソース
description: これは、OneNote エンティティの基本型です。
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: a25e50f6929ae6b13bbe59839f035d2e4a31a6fb
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32462621"
---
# <a name="onenoteentityhierarchymodel-resource"></a><span data-ttu-id="e4352-103">onenoteEntityHierarchyModel リソース</span><span class="sxs-lookup"><span data-stu-id="e4352-103">onenoteEntityHierarchyModel resource</span></span>

<span data-ttu-id="e4352-104">これは、OneNote エンティティの基本型です。</span><span class="sxs-lookup"><span data-stu-id="e4352-104">This is a base type for OneNote entities.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e4352-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e4352-105">JSON representation</span></span>

<span data-ttu-id="e4352-106">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="e4352-106">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="e4352-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e4352-107">Properties</span></span>
## <a name="properties"></a><span data-ttu-id="e4352-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e4352-108">Properties</span></span>
| <span data-ttu-id="e4352-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e4352-109">Property</span></span>     | <span data-ttu-id="e4352-110">型</span><span class="sxs-lookup"><span data-stu-id="e4352-110">Type</span></span>   |<span data-ttu-id="e4352-111">説明</span><span class="sxs-lookup"><span data-stu-id="e4352-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e4352-112">displayName</span><span class="sxs-lookup"><span data-stu-id="e4352-112">displayName</span></span>|<span data-ttu-id="e4352-113">String</span><span class="sxs-lookup"><span data-stu-id="e4352-113">String</span></span>|<span data-ttu-id="e4352-114">ノートブックの名前。</span><span class="sxs-lookup"><span data-stu-id="e4352-114">The name of the notebook.</span></span>|
|<span data-ttu-id="e4352-115">createdBy</span><span class="sxs-lookup"><span data-stu-id="e4352-115">createdBy</span></span>|[<span data-ttu-id="e4352-116">identitySet</span><span class="sxs-lookup"><span data-stu-id="e4352-116">identitySet</span></span>](identityset.md)|<span data-ttu-id="e4352-p101">そのアイテムを作成したユーザーの ID、デバイス、アプリケーション。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="e4352-p101">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="e4352-119">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="e4352-119">lastModifiedBy</span></span>|[<span data-ttu-id="e4352-120">identitySet</span><span class="sxs-lookup"><span data-stu-id="e4352-120">identitySet</span></span>](identityset.md)|<span data-ttu-id="e4352-p102">そのアイテムを作成したユーザーの ID、デバイス、アプリケーション。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="e4352-p102">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="e4352-123">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e4352-123">lastModifiedDateTime</span></span>|<span data-ttu-id="e4352-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e4352-124">DateTimeOffset</span></span>|<span data-ttu-id="e4352-125">ノートブックが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="e4352-125">The date and time when the notebook was last modified.</span></span> <span data-ttu-id="e4352-126">Timestamp は、ISO 8601 形式を使用した日付と時刻の情報を表し、必ず UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="e4352-126">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="e4352-127">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="e4352-127">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="e4352-128">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="e4352-128">Read-only.</span></span>|

<!-- uuid: 8b1af557-1a7c-4432-86eb-94989c2d4b54
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "page resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
