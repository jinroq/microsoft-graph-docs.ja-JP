---
title: keyValuePair リソースの種類
description: アクションパラメーターのキーと値のペア。
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: db8d3b14ceaa0ff05181894af803b8b6feea77c6
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35967036"
---
# <a name="keyvaluepair-resource-type"></a><span data-ttu-id="aeb18-103">keyValuePair リソースの種類</span><span class="sxs-lookup"><span data-stu-id="aeb18-103">keyValuePair resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="aeb18-104">アクションパラメーターのキーと値のペア。</span><span class="sxs-lookup"><span data-stu-id="aeb18-104">Key value pair for action parameters.</span></span>

## <a name="properties"></a><span data-ttu-id="aeb18-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="aeb18-105">Properties</span></span>

| <span data-ttu-id="aeb18-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="aeb18-106">Property</span></span>     | <span data-ttu-id="aeb18-107">型</span><span class="sxs-lookup"><span data-stu-id="aeb18-107">Type</span></span>        | <span data-ttu-id="aeb18-108">説明</span><span class="sxs-lookup"><span data-stu-id="aeb18-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="aeb18-109">name</span><span class="sxs-lookup"><span data-stu-id="aeb18-109">name</span></span>|<span data-ttu-id="aeb18-110">String</span><span class="sxs-lookup"><span data-stu-id="aeb18-110">String</span></span>|<span data-ttu-id="aeb18-111">キーと値のペアの名前</span><span class="sxs-lookup"><span data-stu-id="aeb18-111">Name for this key-value pair</span></span>|
|<span data-ttu-id="aeb18-112">value</span><span class="sxs-lookup"><span data-stu-id="aeb18-112">value</span></span>|<span data-ttu-id="aeb18-113">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="aeb18-113">String</span></span>|<span data-ttu-id="aeb18-114">キーと値のペアの値</span><span class="sxs-lookup"><span data-stu-id="aeb18-114">Value for this key-value pair</span></span>|

## <a name="json-representation"></a><span data-ttu-id="aeb18-115">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="aeb18-115">JSON representation</span></span>

<span data-ttu-id="aeb18-116">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="aeb18-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.keyValuePair",
  "baseType": null
}-->

```json
{
  "name": "String",
  "value": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "keyValuePair resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->