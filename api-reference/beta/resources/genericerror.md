---
title: genericError リソースの種類
description: 汎用エラー。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 701a3b7ed0d7bad6e33f8ba41e77ec7340a57146
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35973528"
---
# <a name="genericerror-resource-type"></a><span data-ttu-id="f0ab5-103">genericError リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f0ab5-103">genericError resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f0ab5-104">汎用エラー。</span><span class="sxs-lookup"><span data-stu-id="f0ab5-104">A general-purpose error.</span></span>

## <a name="properties"></a><span data-ttu-id="f0ab5-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f0ab5-105">Properties</span></span>

| <span data-ttu-id="f0ab5-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f0ab5-106">Property</span></span> | <span data-ttu-id="f0ab5-107">型</span><span class="sxs-lookup"><span data-stu-id="f0ab5-107">Type</span></span> | <span data-ttu-id="f0ab5-108">説明</span><span class="sxs-lookup"><span data-stu-id="f0ab5-108">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="f0ab5-109">メッセージ​​</span><span class="sxs-lookup"><span data-stu-id="f0ab5-109">message</span></span> | <span data-ttu-id="f0ab5-110">String</span><span class="sxs-lookup"><span data-stu-id="f0ab5-110">String</span></span> | <span data-ttu-id="f0ab5-111">エラー メッセージ。</span><span class="sxs-lookup"><span data-stu-id="f0ab5-111">The error message.</span></span> |
| <span data-ttu-id="f0ab5-112">code</span><span class="sxs-lookup"><span data-stu-id="f0ab5-112">code</span></span> | <span data-ttu-id="f0ab5-113">String</span><span class="sxs-lookup"><span data-stu-id="f0ab5-113">String</span></span> | <span data-ttu-id="f0ab5-114">エラーコード。</span><span class="sxs-lookup"><span data-stu-id="f0ab5-114">The error code.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="f0ab5-115">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f0ab5-115">JSON representation</span></span>

<span data-ttu-id="f0ab5-116">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="f0ab5-116">Here is a JSON representation of the resource.</span></span>

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
