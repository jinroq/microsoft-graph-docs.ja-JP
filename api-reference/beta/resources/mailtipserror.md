---
title: mailTipsError リソースの種類
description: アクション中に発生するエラー。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: bcf56c3f5f090fd2f14f3556442e5c19ece9c6cf
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33342682"
---
# <a name="mailtipserror-resource-type"></a><span data-ttu-id="be5de-103">mailTipsError リソースの種類</span><span class="sxs-lookup"><span data-stu-id="be5de-103">mailTipsError resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="be5de-104">アクション中に発生するエラー。</span><span class="sxs-lookup"><span data-stu-id="be5de-104">An error that occurs during an action.</span></span>

## <a name="properties"></a><span data-ttu-id="be5de-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="be5de-105">Properties</span></span>
| <span data-ttu-id="be5de-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="be5de-106">Property</span></span>     | <span data-ttu-id="be5de-107">型</span><span class="sxs-lookup"><span data-stu-id="be5de-107">Type</span></span>   |<span data-ttu-id="be5de-108">説明</span><span class="sxs-lookup"><span data-stu-id="be5de-108">Description</span></span>|
|:-----|:-----|:-----|
| <span data-ttu-id="be5de-109">メッセージ​​</span><span class="sxs-lookup"><span data-stu-id="be5de-109">message</span></span> | <span data-ttu-id="be5de-110">String</span><span class="sxs-lookup"><span data-stu-id="be5de-110">String</span></span> | <span data-ttu-id="be5de-111">エラー メッセージ。</span><span class="sxs-lookup"><span data-stu-id="be5de-111">The error message.</span></span> |
| <span data-ttu-id="be5de-112">code</span><span class="sxs-lookup"><span data-stu-id="be5de-112">code</span></span> | <span data-ttu-id="be5de-113">String</span><span class="sxs-lookup"><span data-stu-id="be5de-113">String</span></span> | <span data-ttu-id="be5de-114">エラーコード。</span><span class="sxs-lookup"><span data-stu-id="be5de-114">The error code.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="be5de-115">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="be5de-115">JSON representation</span></span>

<span data-ttu-id="be5de-116">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="be5de-116">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "mailTipsError resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
