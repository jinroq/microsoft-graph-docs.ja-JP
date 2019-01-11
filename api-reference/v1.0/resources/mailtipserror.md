---
title: mailTipsError リソースの種類
description: 操作中に発生するエラーです。
localization_priority: Normal
ms.openlocfilehash: a4916bc34d7c76dc6c6592ee03e64b20a6485190
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27892094"
---
# <a name="mailtipserror-resource-type"></a><span data-ttu-id="f09ea-103">mailTipsError リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f09ea-103">mailTipsError resource type</span></span>

<span data-ttu-id="f09ea-104">操作中に発生するエラーです。</span><span class="sxs-lookup"><span data-stu-id="f09ea-104">An error that occurs during an action.</span></span>

## <a name="properties"></a><span data-ttu-id="f09ea-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f09ea-105">Properties</span></span>
| <span data-ttu-id="f09ea-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f09ea-106">Property</span></span>     | <span data-ttu-id="f09ea-107">種類</span><span class="sxs-lookup"><span data-stu-id="f09ea-107">Type</span></span>   |<span data-ttu-id="f09ea-108">説明</span><span class="sxs-lookup"><span data-stu-id="f09ea-108">Description</span></span>|
|:-----|:-----|:-----|
| <span data-ttu-id="f09ea-109">message</span><span class="sxs-lookup"><span data-stu-id="f09ea-109">message</span></span> | <span data-ttu-id="f09ea-110">String</span><span class="sxs-lookup"><span data-stu-id="f09ea-110">String</span></span> | <span data-ttu-id="f09ea-111">エラー メッセージ。</span><span class="sxs-lookup"><span data-stu-id="f09ea-111">The error message.</span></span> |
| <span data-ttu-id="f09ea-112">code</span><span class="sxs-lookup"><span data-stu-id="f09ea-112">code</span></span> | <span data-ttu-id="f09ea-113">String</span><span class="sxs-lookup"><span data-stu-id="f09ea-113">String</span></span> | <span data-ttu-id="f09ea-114">エラー コード。</span><span class="sxs-lookup"><span data-stu-id="f09ea-114">The error code.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="f09ea-115">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f09ea-115">JSON representation</span></span>

<span data-ttu-id="f09ea-116">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="f09ea-116">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.mailTipsError"
}-->

```json
{
  "message": "string",
  "code": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "mailTipsError resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
