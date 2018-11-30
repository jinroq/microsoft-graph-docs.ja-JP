---
title: mailTipsError リソースの種類
description: 操作中に発生するエラーです。
ms.openlocfilehash: 8604207844ade4e0c10981f30d03b33eacf4a0a2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27021769"
---
# <a name="mailtipserror-resource-type"></a><span data-ttu-id="18400-103">mailTipsError リソースの種類</span><span class="sxs-lookup"><span data-stu-id="18400-103">mailTipsError resource type</span></span>

<span data-ttu-id="18400-104">操作中に発生するエラーです。</span><span class="sxs-lookup"><span data-stu-id="18400-104">An error that occurs during an action.</span></span>

## <a name="properties"></a><span data-ttu-id="18400-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="18400-105">Properties</span></span>
| <span data-ttu-id="18400-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="18400-106">Property</span></span>     | <span data-ttu-id="18400-107">型</span><span class="sxs-lookup"><span data-stu-id="18400-107">Type</span></span>   |<span data-ttu-id="18400-108">説明</span><span class="sxs-lookup"><span data-stu-id="18400-108">Description</span></span>|
|:-----|:-----|:-----|
| <span data-ttu-id="18400-109">message</span><span class="sxs-lookup"><span data-stu-id="18400-109">message</span></span> | <span data-ttu-id="18400-110">String</span><span class="sxs-lookup"><span data-stu-id="18400-110">String</span></span> | <span data-ttu-id="18400-111">エラー メッセージ。</span><span class="sxs-lookup"><span data-stu-id="18400-111">The error message.</span></span> |
| <span data-ttu-id="18400-112">code</span><span class="sxs-lookup"><span data-stu-id="18400-112">code</span></span> | <span data-ttu-id="18400-113">String</span><span class="sxs-lookup"><span data-stu-id="18400-113">String</span></span> | <span data-ttu-id="18400-114">エラー コード。</span><span class="sxs-lookup"><span data-stu-id="18400-114">The error code.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="18400-115">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="18400-115">JSON representation</span></span>

<span data-ttu-id="18400-116">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="18400-116">Here is a JSON representation of the resource.</span></span>

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