---
title: mailTipsError リソースの種類
description: 操作中に発生するエラーです。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 499949c5995025e9327e1f662365b0c5e43c80f4
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27934206"
---
# <a name="mailtipserror-resource-type"></a><span data-ttu-id="73c20-103">mailTipsError リソースの種類</span><span class="sxs-lookup"><span data-stu-id="73c20-103">mailTipsError resource type</span></span>

<span data-ttu-id="73c20-104">操作中に発生するエラーです。</span><span class="sxs-lookup"><span data-stu-id="73c20-104">An error that occurs during an action.</span></span>

## <a name="properties"></a><span data-ttu-id="73c20-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="73c20-105">Properties</span></span>
| <span data-ttu-id="73c20-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="73c20-106">Property</span></span>     | <span data-ttu-id="73c20-107">種類</span><span class="sxs-lookup"><span data-stu-id="73c20-107">Type</span></span>   |<span data-ttu-id="73c20-108">説明</span><span class="sxs-lookup"><span data-stu-id="73c20-108">Description</span></span>|
|:-----|:-----|:-----|
| <span data-ttu-id="73c20-109">message</span><span class="sxs-lookup"><span data-stu-id="73c20-109">message</span></span> | <span data-ttu-id="73c20-110">String</span><span class="sxs-lookup"><span data-stu-id="73c20-110">String</span></span> | <span data-ttu-id="73c20-111">エラー メッセージ。</span><span class="sxs-lookup"><span data-stu-id="73c20-111">The error message.</span></span> |
| <span data-ttu-id="73c20-112">code</span><span class="sxs-lookup"><span data-stu-id="73c20-112">code</span></span> | <span data-ttu-id="73c20-113">String</span><span class="sxs-lookup"><span data-stu-id="73c20-113">String</span></span> | <span data-ttu-id="73c20-114">エラー コード。</span><span class="sxs-lookup"><span data-stu-id="73c20-114">The error code.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="73c20-115">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="73c20-115">JSON representation</span></span>

<span data-ttu-id="73c20-116">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="73c20-116">Here is a JSON representation of the resource.</span></span>

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
