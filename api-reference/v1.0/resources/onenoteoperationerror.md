---
title: onenoteOperationError リソースの種類
description: 失敗した OneNote 操作によるエラー。
author: Jewan-microsoft
localization_priority: Normal
ms.openlocfilehash: df0bfd768d26c751a303f42e1f1123b863388faa
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27837339"
---
# <a name="onenoteoperationerror-resource-type"></a><span data-ttu-id="40389-103">onenoteOperationError リソースの種類</span><span class="sxs-lookup"><span data-stu-id="40389-103">onenoteOperationError resource type</span></span>

<span data-ttu-id="40389-104">失敗した OneNote 操作によるエラー。</span><span class="sxs-lookup"><span data-stu-id="40389-104">An error from a failed OneNote operation.</span></span>

## <a name="json-representation"></a><span data-ttu-id="40389-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="40389-105">JSON representation</span></span>

<span data-ttu-id="40389-106">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="40389-106">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="40389-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="40389-107">Properties</span></span>
| <span data-ttu-id="40389-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="40389-108">Property</span></span>     | <span data-ttu-id="40389-109">種類</span><span class="sxs-lookup"><span data-stu-id="40389-109">Type</span></span>   |<span data-ttu-id="40389-110">説明</span><span class="sxs-lookup"><span data-stu-id="40389-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="40389-111">code</span><span class="sxs-lookup"><span data-stu-id="40389-111">code</span></span>|<span data-ttu-id="40389-112">文字列</span><span class="sxs-lookup"><span data-stu-id="40389-112">string</span></span>|<span data-ttu-id="40389-113">エラー コード。</span><span class="sxs-lookup"><span data-stu-id="40389-113">The error code.</span></span>|
|<span data-ttu-id="40389-114">message</span><span class="sxs-lookup"><span data-stu-id="40389-114">message</span></span>|<span data-ttu-id="40389-115">文字列</span><span class="sxs-lookup"><span data-stu-id="40389-115">string</span></span>|<span data-ttu-id="40389-116">エラー メッセージ。</span><span class="sxs-lookup"><span data-stu-id="40389-116">The error message.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onenoteOperationError resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
