---
title: keyValuePair リソースの種類
description: アクションパラメーターのキーと値のペア。
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: 86a5415c20721f717947238838341345ec9a4250
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32522686"
---
# <a name="keyvaluepair-resource-type"></a><span data-ttu-id="cb988-103">keyValuePair リソースの種類</span><span class="sxs-lookup"><span data-stu-id="cb988-103">keyValuePair resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cb988-104">アクションパラメーターのキーと値のペア。</span><span class="sxs-lookup"><span data-stu-id="cb988-104">Key value pair for action parameters.</span></span>

## <a name="properties"></a><span data-ttu-id="cb988-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cb988-105">Properties</span></span>

| <span data-ttu-id="cb988-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cb988-106">Property</span></span>     | <span data-ttu-id="cb988-107">型</span><span class="sxs-lookup"><span data-stu-id="cb988-107">Type</span></span>        | <span data-ttu-id="cb988-108">説明</span><span class="sxs-lookup"><span data-stu-id="cb988-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="cb988-109">name</span><span class="sxs-lookup"><span data-stu-id="cb988-109">name</span></span>|<span data-ttu-id="cb988-110">String</span><span class="sxs-lookup"><span data-stu-id="cb988-110">String</span></span>|<span data-ttu-id="cb988-111">キーと値のペアの名前</span><span class="sxs-lookup"><span data-stu-id="cb988-111">Name for this key-value pair</span></span>|
|<span data-ttu-id="cb988-112">value</span><span class="sxs-lookup"><span data-stu-id="cb988-112">value</span></span>|<span data-ttu-id="cb988-113">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="cb988-113">String</span></span>|<span data-ttu-id="cb988-114">キーと値のペアの値</span><span class="sxs-lookup"><span data-stu-id="cb988-114">Value for this key-value pair</span></span>|

## <a name="json-representation"></a><span data-ttu-id="cb988-115">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="cb988-115">JSON representation</span></span>

<span data-ttu-id="cb988-116">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="cb988-116">The following is a JSON representation of the resource.</span></span>

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