---
title: educationMakeCodeResource リソースの種類
description: MakeCode リソース
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: e983f217af71b6e27f750599ee2f8db295da5fec
ms.sourcegitcommit: 129e58f83fc566f9d9f36e26b0c0b8cdf81d27d9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/03/2019
ms.locfileid: "36173371"
---
# <a name="educationmakecoderesource-resource-type"></a><span data-ttu-id="849ac-103">educationMakeCodeResource リソースの種類</span><span class="sxs-lookup"><span data-stu-id="849ac-103">educationMakeCodeResource resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="849ac-104">[MakeCode](https://www.microsoft.com/en-us/makecode)プロジェクトを表すリソース。</span><span class="sxs-lookup"><span data-stu-id="849ac-104">A resource representing a [MakeCode](https://www.microsoft.com/en-us/makecode) project.</span></span>

## <a name="properties"></a><span data-ttu-id="849ac-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="849ac-105">Properties</span></span>

| <span data-ttu-id="849ac-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="849ac-106">Property</span></span>     | <span data-ttu-id="849ac-107">型</span><span class="sxs-lookup"><span data-stu-id="849ac-107">Type</span></span>        | <span data-ttu-id="849ac-108">説明</span><span class="sxs-lookup"><span data-stu-id="849ac-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="849ac-109">mkcd</span><span class="sxs-lookup"><span data-stu-id="849ac-109">mkcd</span></span>|<span data-ttu-id="849ac-110">String</span><span class="sxs-lookup"><span data-stu-id="849ac-110">String</span></span>|<span data-ttu-id="849ac-111">MakeCode プロジェクトの ID</span><span class="sxs-lookup"><span data-stu-id="849ac-111">ID of the MakeCode project</span></span>|
|<span data-ttu-id="849ac-112">url</span><span class="sxs-lookup"><span data-stu-id="849ac-112">url</span></span>|<span data-ttu-id="849ac-113">String</span><span class="sxs-lookup"><span data-stu-id="849ac-113">String</span></span>|<span data-ttu-id="849ac-114">MakeCode リソースの種類 (アーケード、microbit など) のホスト</span><span class="sxs-lookup"><span data-stu-id="849ac-114">Host for the type of MakeCode resource (for example, arcade, microbit)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="849ac-115">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="849ac-115">JSON representation</span></span>

<span data-ttu-id="849ac-116">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="849ac-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationMakeCodeResource",
  "baseType": "microsoft.graph.educationResource"
}-->

```json
{
  "mkcd": "String",
  "url": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationMakeCodeResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->