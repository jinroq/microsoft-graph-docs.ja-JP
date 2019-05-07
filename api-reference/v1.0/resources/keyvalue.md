---
title: keyValue リソースの種類
description: 標準のキーと値のペアのリソースの種類。
localization_priority: Normal
ms.openlocfilehash: aa026f36d69e894e056f21ba19865c730ec5b643
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33629272"
---
# <a name="keyvalue-resource-type"></a><span data-ttu-id="6ce28-103">keyValue リソースの種類</span><span class="sxs-lookup"><span data-stu-id="6ce28-103">keyValue resource type</span></span>

<span data-ttu-id="6ce28-104">キーと値のペアを表します。</span><span class="sxs-lookup"><span data-stu-id="6ce28-104">Represents a key-value pair.</span></span>

## <a name="properties"></a><span data-ttu-id="6ce28-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6ce28-105">Properties</span></span>

| <span data-ttu-id="6ce28-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6ce28-106">Property</span></span>     | <span data-ttu-id="6ce28-107">型</span><span class="sxs-lookup"><span data-stu-id="6ce28-107">Type</span></span>   |<span data-ttu-id="6ce28-108">説明</span><span class="sxs-lookup"><span data-stu-id="6ce28-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6ce28-109">Key</span><span class="sxs-lookup"><span data-stu-id="6ce28-109">key</span></span>|<span data-ttu-id="6ce28-110">string</span><span class="sxs-lookup"><span data-stu-id="6ce28-110">string</span></span>| <span data-ttu-id="6ce28-111">キーと値のペアのキー。</span><span class="sxs-lookup"><span data-stu-id="6ce28-111">Key for the key-value pair.</span></span> |
|<span data-ttu-id="6ce28-112">value</span><span class="sxs-lookup"><span data-stu-id="6ce28-112">value</span></span>|<span data-ttu-id="6ce28-113">string</span><span class="sxs-lookup"><span data-stu-id="6ce28-113">string</span></span>| <span data-ttu-id="6ce28-114">キーと値のペアの値。</span><span class="sxs-lookup"><span data-stu-id="6ce28-114">Value for the key-value pair.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6ce28-115">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="6ce28-115">JSON representation</span></span>

<span data-ttu-id="6ce28-116">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="6ce28-116">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.keyValue"
}-->

```json
{
  "key": "string",
  "value": "string"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "keyValue resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}
-->
