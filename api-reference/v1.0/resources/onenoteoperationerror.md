---
title: onenoteOperationError リソースの種類
description: 失敗した OneNote 操作によるエラー。
author: Jewan-microsoft
ms.openlocfilehash: e31d47f9351a050eef134cde2f6a6a8bbdf526d7
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27320693"
---
# <a name="onenoteoperationerror-resource-type"></a><span data-ttu-id="fc2cf-103">onenoteOperationError リソースの種類</span><span class="sxs-lookup"><span data-stu-id="fc2cf-103">onenoteOperationError resource type</span></span>

<span data-ttu-id="fc2cf-104">失敗した OneNote 操作によるエラー。</span><span class="sxs-lookup"><span data-stu-id="fc2cf-104">An error from a failed OneNote operation.</span></span>

## <a name="json-representation"></a><span data-ttu-id="fc2cf-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="fc2cf-105">JSON representation</span></span>

<span data-ttu-id="fc2cf-106">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="fc2cf-106">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onenoteOperationError"
}-->

```json
{
  "code": "string",
  "message": "string"
}

```
## <a name="properties"></a><span data-ttu-id="fc2cf-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fc2cf-107">Properties</span></span>
| <span data-ttu-id="fc2cf-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fc2cf-108">Property</span></span>     | <span data-ttu-id="fc2cf-109">種類</span><span class="sxs-lookup"><span data-stu-id="fc2cf-109">Type</span></span>   |<span data-ttu-id="fc2cf-110">説明</span><span class="sxs-lookup"><span data-stu-id="fc2cf-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fc2cf-111">code</span><span class="sxs-lookup"><span data-stu-id="fc2cf-111">code</span></span>|<span data-ttu-id="fc2cf-112">文字列</span><span class="sxs-lookup"><span data-stu-id="fc2cf-112">string</span></span>|<span data-ttu-id="fc2cf-113">エラー コード。</span><span class="sxs-lookup"><span data-stu-id="fc2cf-113">The error code.</span></span>|
|<span data-ttu-id="fc2cf-114">message</span><span class="sxs-lookup"><span data-stu-id="fc2cf-114">message</span></span>|<span data-ttu-id="fc2cf-115">string</span><span class="sxs-lookup"><span data-stu-id="fc2cf-115">string</span></span>|<span data-ttu-id="fc2cf-116">エラー メッセージ。</span><span class="sxs-lookup"><span data-stu-id="fc2cf-116">The error message.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onenoteOperationError resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
