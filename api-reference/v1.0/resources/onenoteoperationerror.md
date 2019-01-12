---
title: onenoteOperationError リソースの種類
description: 失敗した OneNote 操作によるエラー。
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: 3291f70e8cc18ee532f636feb1de9e8bb5751e02
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27932463"
---
# <a name="onenoteoperationerror-resource-type"></a><span data-ttu-id="8e111-103">onenoteOperationError リソースの種類</span><span class="sxs-lookup"><span data-stu-id="8e111-103">onenoteOperationError resource type</span></span>

<span data-ttu-id="8e111-104">失敗した OneNote 操作によるエラー。</span><span class="sxs-lookup"><span data-stu-id="8e111-104">An error from a failed OneNote operation.</span></span>

## <a name="json-representation"></a><span data-ttu-id="8e111-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="8e111-105">JSON representation</span></span>

<span data-ttu-id="8e111-106">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="8e111-106">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="8e111-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8e111-107">Properties</span></span>
| <span data-ttu-id="8e111-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8e111-108">Property</span></span>     | <span data-ttu-id="8e111-109">種類</span><span class="sxs-lookup"><span data-stu-id="8e111-109">Type</span></span>   |<span data-ttu-id="8e111-110">説明</span><span class="sxs-lookup"><span data-stu-id="8e111-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8e111-111">code</span><span class="sxs-lookup"><span data-stu-id="8e111-111">code</span></span>|<span data-ttu-id="8e111-112">文字列</span><span class="sxs-lookup"><span data-stu-id="8e111-112">string</span></span>|<span data-ttu-id="8e111-113">エラー コード。</span><span class="sxs-lookup"><span data-stu-id="8e111-113">The error code.</span></span>|
|<span data-ttu-id="8e111-114">message</span><span class="sxs-lookup"><span data-stu-id="8e111-114">message</span></span>|<span data-ttu-id="8e111-115">文字列</span><span class="sxs-lookup"><span data-stu-id="8e111-115">string</span></span>|<span data-ttu-id="8e111-116">エラー メッセージ。</span><span class="sxs-lookup"><span data-stu-id="8e111-116">The error message.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onenoteOperationError resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
