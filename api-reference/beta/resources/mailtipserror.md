---
title: mailTipsError リソースの種類
description: アクション中に発生するエラー。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 0c17a2fa6cd5475c043fddadef735599c954779d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36009819"
---
# <a name="mailtipserror-resource-type"></a><span data-ttu-id="25957-103">mailTipsError リソースの種類</span><span class="sxs-lookup"><span data-stu-id="25957-103">mailTipsError resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="25957-104">アクション中に発生するエラー。</span><span class="sxs-lookup"><span data-stu-id="25957-104">An error that occurs during an action.</span></span>

## <a name="properties"></a><span data-ttu-id="25957-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="25957-105">Properties</span></span>
| <span data-ttu-id="25957-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="25957-106">Property</span></span>     | <span data-ttu-id="25957-107">型</span><span class="sxs-lookup"><span data-stu-id="25957-107">Type</span></span>   |<span data-ttu-id="25957-108">説明</span><span class="sxs-lookup"><span data-stu-id="25957-108">Description</span></span>|
|:-----|:-----|:-----|
| <span data-ttu-id="25957-109">メッセージ​​</span><span class="sxs-lookup"><span data-stu-id="25957-109">message</span></span> | <span data-ttu-id="25957-110">String</span><span class="sxs-lookup"><span data-stu-id="25957-110">String</span></span> | <span data-ttu-id="25957-111">エラー メッセージ。</span><span class="sxs-lookup"><span data-stu-id="25957-111">The error message.</span></span> |
| <span data-ttu-id="25957-112">code</span><span class="sxs-lookup"><span data-stu-id="25957-112">code</span></span> | <span data-ttu-id="25957-113">String</span><span class="sxs-lookup"><span data-stu-id="25957-113">String</span></span> | <span data-ttu-id="25957-114">エラーコード。</span><span class="sxs-lookup"><span data-stu-id="25957-114">The error code.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="25957-115">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="25957-115">JSON representation</span></span>

<span data-ttu-id="25957-116">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="25957-116">Here is a JSON representation of the resource.</span></span>

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
