---
title: mailTipsError リソースの種類
description: アクション中に発生するエラー。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: fd5df6f723ad41f7e6c2074f278cd5f59a902bf6
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36036317"
---
# <a name="mailtipserror-resource-type"></a><span data-ttu-id="060d8-103">mailTipsError リソースの種類</span><span class="sxs-lookup"><span data-stu-id="060d8-103">mailTipsError resource type</span></span>

<span data-ttu-id="060d8-104">アクション中に発生するエラー。</span><span class="sxs-lookup"><span data-stu-id="060d8-104">An error that occurs during an action.</span></span>

## <a name="properties"></a><span data-ttu-id="060d8-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="060d8-105">Properties</span></span>
| <span data-ttu-id="060d8-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="060d8-106">Property</span></span>     | <span data-ttu-id="060d8-107">型</span><span class="sxs-lookup"><span data-stu-id="060d8-107">Type</span></span>   |<span data-ttu-id="060d8-108">説明</span><span class="sxs-lookup"><span data-stu-id="060d8-108">Description</span></span>|
|:-----|:-----|:-----|
| <span data-ttu-id="060d8-109">メッセージ​​</span><span class="sxs-lookup"><span data-stu-id="060d8-109">message</span></span> | <span data-ttu-id="060d8-110">String</span><span class="sxs-lookup"><span data-stu-id="060d8-110">String</span></span> | <span data-ttu-id="060d8-111">エラー メッセージ。</span><span class="sxs-lookup"><span data-stu-id="060d8-111">The error message.</span></span> |
| <span data-ttu-id="060d8-112">code</span><span class="sxs-lookup"><span data-stu-id="060d8-112">code</span></span> | <span data-ttu-id="060d8-113">String</span><span class="sxs-lookup"><span data-stu-id="060d8-113">String</span></span> | <span data-ttu-id="060d8-114">エラーコード。</span><span class="sxs-lookup"><span data-stu-id="060d8-114">The error code.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="060d8-115">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="060d8-115">JSON representation</span></span>

<span data-ttu-id="060d8-116">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="060d8-116">Here is a JSON representation of the resource.</span></span>

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
