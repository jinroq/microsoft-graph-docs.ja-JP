---
title: genericerror リソースの種類
description: 汎用エラー。
localization_priority: Normal
ms.openlocfilehash: 314bb5f5e94e44c326fceb71f4a79463989f2129
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33333670"
---
# <a name="genericerror-resource-type"></a><span data-ttu-id="fae4d-103">genericerror リソースの種類</span><span class="sxs-lookup"><span data-stu-id="fae4d-103">genericError resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fae4d-104">汎用エラー。</span><span class="sxs-lookup"><span data-stu-id="fae4d-104">A general-purpose error.</span></span>

## <a name="properties"></a><span data-ttu-id="fae4d-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fae4d-105">Properties</span></span>

| <span data-ttu-id="fae4d-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fae4d-106">Property</span></span> | <span data-ttu-id="fae4d-107">型</span><span class="sxs-lookup"><span data-stu-id="fae4d-107">Type</span></span> | <span data-ttu-id="fae4d-108">説明</span><span class="sxs-lookup"><span data-stu-id="fae4d-108">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="fae4d-109">メッセージ​​</span><span class="sxs-lookup"><span data-stu-id="fae4d-109">message</span></span> | <span data-ttu-id="fae4d-110">String</span><span class="sxs-lookup"><span data-stu-id="fae4d-110">String</span></span> | <span data-ttu-id="fae4d-111">エラー メッセージ。</span><span class="sxs-lookup"><span data-stu-id="fae4d-111">The error message.</span></span> |
| <span data-ttu-id="fae4d-112">code</span><span class="sxs-lookup"><span data-stu-id="fae4d-112">code</span></span> | <span data-ttu-id="fae4d-113">String</span><span class="sxs-lookup"><span data-stu-id="fae4d-113">String</span></span> | <span data-ttu-id="fae4d-114">エラーコード。</span><span class="sxs-lookup"><span data-stu-id="fae4d-114">The error code.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="fae4d-115">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="fae4d-115">JSON representation</span></span>

<span data-ttu-id="fae4d-116">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="fae4d-116">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
  ],
  "@odata.type": "microsoft.graph.genericError"
}-->

```json
{
  "message": "String",
  "code": "String"
}
```
