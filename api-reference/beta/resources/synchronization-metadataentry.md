---
title: metadataEntry リソースの種類
description: 指定したオブジェクトのメタデータ。
localization_priority: Normal
doc_type: resourcePageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 55b686bc04ccf869ddf9d6dc6029c6206f7b2274
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964842"
---
# <a name="metadataentry-resource-type"></a><span data-ttu-id="40a9a-103">metadataEntry リソースの種類</span><span class="sxs-lookup"><span data-stu-id="40a9a-103">metadataEntry resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="40a9a-104">指定したオブジェクトのメタデータ。</span><span class="sxs-lookup"><span data-stu-id="40a9a-104">Metadata for the given object.</span></span>

## <a name="properties"></a><span data-ttu-id="40a9a-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="40a9a-105">Properties</span></span>
| <span data-ttu-id="40a9a-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="40a9a-106">Property</span></span>     | <span data-ttu-id="40a9a-107">型</span><span class="sxs-lookup"><span data-stu-id="40a9a-107">Type</span></span>   |<span data-ttu-id="40a9a-108">説明</span><span class="sxs-lookup"><span data-stu-id="40a9a-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="40a9a-109">Key</span><span class="sxs-lookup"><span data-stu-id="40a9a-109">key</span></span>|<span data-ttu-id="40a9a-110">String</span><span class="sxs-lookup"><span data-stu-id="40a9a-110">String</span></span>|<span data-ttu-id="40a9a-111">メタデータプロパティの名前。</span><span class="sxs-lookup"><span data-stu-id="40a9a-111">Name of the metadata property.</span></span>|
|<span data-ttu-id="40a9a-112">value</span><span class="sxs-lookup"><span data-stu-id="40a9a-112">value</span></span>|<span data-ttu-id="40a9a-113">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="40a9a-113">String</span></span>|<span data-ttu-id="40a9a-114">メタデータプロパティの値。</span><span class="sxs-lookup"><span data-stu-id="40a9a-114">Value of the metadata property.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="40a9a-115">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="40a9a-115">JSON representation</span></span>

<span data-ttu-id="40a9a-116">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="40a9a-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.metadataEntry"
}-->

```json
{
  "key": "String",
  "value": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "metadataEntry resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
