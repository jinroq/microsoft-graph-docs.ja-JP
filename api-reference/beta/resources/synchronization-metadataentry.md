---
title: metadataEntry リソースの種類
description: 指定したオブジェクトのメタデータ。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 49c43e502cfb06832172f46c1e790b2a20eb0f08
ms.sourcegitcommit: 121c0fad692fb3c5c01dc051481b5249e4491b48
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/11/2019
ms.locfileid: "35620557"
---
# <a name="metadataentry-resource-type"></a><span data-ttu-id="cb637-103">metadataEntry リソースの種類</span><span class="sxs-lookup"><span data-stu-id="cb637-103">metadataEntry resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cb637-104">指定したオブジェクトのメタデータ。</span><span class="sxs-lookup"><span data-stu-id="cb637-104">Metadata for the given object.</span></span>

## <a name="properties"></a><span data-ttu-id="cb637-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cb637-105">Properties</span></span>
| <span data-ttu-id="cb637-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cb637-106">Property</span></span>     | <span data-ttu-id="cb637-107">型</span><span class="sxs-lookup"><span data-stu-id="cb637-107">Type</span></span>   |<span data-ttu-id="cb637-108">説明</span><span class="sxs-lookup"><span data-stu-id="cb637-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cb637-109">Key</span><span class="sxs-lookup"><span data-stu-id="cb637-109">key</span></span>|<span data-ttu-id="cb637-110">String</span><span class="sxs-lookup"><span data-stu-id="cb637-110">String</span></span>|<span data-ttu-id="cb637-111">メタデータプロパティの名前。</span><span class="sxs-lookup"><span data-stu-id="cb637-111">Name of the metadata property.</span></span>|
|<span data-ttu-id="cb637-112">value</span><span class="sxs-lookup"><span data-stu-id="cb637-112">value</span></span>|<span data-ttu-id="cb637-113">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="cb637-113">String</span></span>|<span data-ttu-id="cb637-114">メタデータプロパティの値。</span><span class="sxs-lookup"><span data-stu-id="cb637-114">Value of the metadata property.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="cb637-115">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="cb637-115">JSON representation</span></span>

<span data-ttu-id="cb637-116">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="cb637-116">The following is a JSON representation of the resource.</span></span>

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
