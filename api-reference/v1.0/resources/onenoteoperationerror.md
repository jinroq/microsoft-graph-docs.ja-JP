---
title: onenoteOperationError リソースの種類
description: 失敗した OneNote 操作のエラー。
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
doc_type: resourcePageType
ms.openlocfilehash: 95eda3299b62a1ebe49b2520206265cc14c3ac57
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36035771"
---
# <a name="onenoteoperationerror-resource-type"></a><span data-ttu-id="5fd84-103">onenoteOperationError リソースの種類</span><span class="sxs-lookup"><span data-stu-id="5fd84-103">onenoteOperationError resource type</span></span>

<span data-ttu-id="5fd84-104">失敗した OneNote 操作のエラー。</span><span class="sxs-lookup"><span data-stu-id="5fd84-104">An error from a failed OneNote operation.</span></span>

## <a name="json-representation"></a><span data-ttu-id="5fd84-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="5fd84-105">JSON representation</span></span>

<span data-ttu-id="5fd84-106">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="5fd84-106">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="5fd84-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5fd84-107">Properties</span></span>
| <span data-ttu-id="5fd84-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5fd84-108">Property</span></span>     | <span data-ttu-id="5fd84-109">型</span><span class="sxs-lookup"><span data-stu-id="5fd84-109">Type</span></span>   |<span data-ttu-id="5fd84-110">説明</span><span class="sxs-lookup"><span data-stu-id="5fd84-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5fd84-111">code</span><span class="sxs-lookup"><span data-stu-id="5fd84-111">code</span></span>|<span data-ttu-id="5fd84-112">string</span><span class="sxs-lookup"><span data-stu-id="5fd84-112">string</span></span>|<span data-ttu-id="5fd84-113">エラーコード。</span><span class="sxs-lookup"><span data-stu-id="5fd84-113">The error code.</span></span>|
|<span data-ttu-id="5fd84-114">message</span><span class="sxs-lookup"><span data-stu-id="5fd84-114">message</span></span>|<span data-ttu-id="5fd84-115">string</span><span class="sxs-lookup"><span data-stu-id="5fd84-115">string</span></span>|<span data-ttu-id="5fd84-116">エラー メッセージ。</span><span class="sxs-lookup"><span data-stu-id="5fd84-116">The error message.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onenoteOperationError resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
