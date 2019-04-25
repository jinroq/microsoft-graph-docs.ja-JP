---
title: mailTipsError リソースの種類
description: アクション中に発生するエラー。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 499949c5995025e9327e1f662365b0c5e43c80f4
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32574006"
---
# <a name="mailtipserror-resource-type"></a><span data-ttu-id="6f9d2-103">mailTipsError リソースの種類</span><span class="sxs-lookup"><span data-stu-id="6f9d2-103">mailTipsError resource type</span></span>

<span data-ttu-id="6f9d2-104">アクション中に発生するエラー。</span><span class="sxs-lookup"><span data-stu-id="6f9d2-104">An error that occurs during an action.</span></span>

## <a name="properties"></a><span data-ttu-id="6f9d2-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6f9d2-105">Properties</span></span>
| <span data-ttu-id="6f9d2-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6f9d2-106">Property</span></span>     | <span data-ttu-id="6f9d2-107">型</span><span class="sxs-lookup"><span data-stu-id="6f9d2-107">Type</span></span>   |<span data-ttu-id="6f9d2-108">説明</span><span class="sxs-lookup"><span data-stu-id="6f9d2-108">Description</span></span>|
|:-----|:-----|:-----|
| <span data-ttu-id="6f9d2-109">メッセージ​​</span><span class="sxs-lookup"><span data-stu-id="6f9d2-109">message</span></span> | <span data-ttu-id="6f9d2-110">String</span><span class="sxs-lookup"><span data-stu-id="6f9d2-110">String</span></span> | <span data-ttu-id="6f9d2-111">エラー メッセージ。</span><span class="sxs-lookup"><span data-stu-id="6f9d2-111">The error message.</span></span> |
| <span data-ttu-id="6f9d2-112">code</span><span class="sxs-lookup"><span data-stu-id="6f9d2-112">code</span></span> | <span data-ttu-id="6f9d2-113">String</span><span class="sxs-lookup"><span data-stu-id="6f9d2-113">String</span></span> | <span data-ttu-id="6f9d2-114">エラーコード。</span><span class="sxs-lookup"><span data-stu-id="6f9d2-114">The error code.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="6f9d2-115">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="6f9d2-115">JSON representation</span></span>

<span data-ttu-id="6f9d2-116">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="6f9d2-116">Here is a JSON representation of the resource.</span></span>

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
