---
title: onenoteEntityBaseModel リソース
description: これは、OneNote エンティティの基本型です。
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: 53ed86ae22f3ac9fccdef98e56382cd9440e71e2
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32462614"
---
# <a name="onenoteentitybasemodel-resource"></a><span data-ttu-id="8df0c-103">onenoteEntityBaseModel リソース</span><span class="sxs-lookup"><span data-stu-id="8df0c-103">onenoteEntityBaseModel resource</span></span>

<span data-ttu-id="8df0c-104">これは、OneNote エンティティの基本型です。</span><span class="sxs-lookup"><span data-stu-id="8df0c-104">This is the base type for OneNote entities.</span></span>

## <a name="json-representation"></a><span data-ttu-id="8df0c-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="8df0c-105">JSON representation</span></span>

<span data-ttu-id="8df0c-106">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="8df0c-106">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "abstract": true,
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [
    "self"
  ],
  "@odata.type": "microsoft.graph.onenoteEntityBaseModel"
}-->

```json
{
  "self": "string"
}

```
## <a name="properties"></a><span data-ttu-id="8df0c-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8df0c-107">Properties</span></span>
| <span data-ttu-id="8df0c-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8df0c-108">Property</span></span>     | <span data-ttu-id="8df0c-109">型</span><span class="sxs-lookup"><span data-stu-id="8df0c-109">Type</span></span>   |<span data-ttu-id="8df0c-110">説明</span><span class="sxs-lookup"><span data-stu-id="8df0c-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8df0c-111">self</span><span class="sxs-lookup"><span data-stu-id="8df0c-111">self</span></span>|<span data-ttu-id="8df0c-112">String</span><span class="sxs-lookup"><span data-stu-id="8df0c-112">String</span></span>|<span data-ttu-id="8df0c-113">ページに関する詳細を取得できるエンドポイント。</span><span class="sxs-lookup"><span data-stu-id="8df0c-113">The endpoint where you can get details about the page.</span></span> <span data-ttu-id="8df0c-114">値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="8df0c-114">Read-only.</span></span>|

<!-- uuid: bfb567de-2a2a-4b81-bf47-a55626a0c166
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "page resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
