---
title: keyValue リソースの種類
description: 標準のキーと値のペアのリソースの種類。
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 7a3008b328337e4dd4d816f4b0d7432b7e24c08d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36036492"
---
# <a name="keyvalue-resource-type"></a><span data-ttu-id="98daf-103">keyValue リソースの種類</span><span class="sxs-lookup"><span data-stu-id="98daf-103">keyValue resource type</span></span>

<span data-ttu-id="98daf-104">キーと値のペアを表します。</span><span class="sxs-lookup"><span data-stu-id="98daf-104">Represents a key-value pair.</span></span>

## <a name="properties"></a><span data-ttu-id="98daf-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="98daf-105">Properties</span></span>

| <span data-ttu-id="98daf-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="98daf-106">Property</span></span>     | <span data-ttu-id="98daf-107">型</span><span class="sxs-lookup"><span data-stu-id="98daf-107">Type</span></span>   |<span data-ttu-id="98daf-108">説明</span><span class="sxs-lookup"><span data-stu-id="98daf-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="98daf-109">Key</span><span class="sxs-lookup"><span data-stu-id="98daf-109">key</span></span>|<span data-ttu-id="98daf-110">string</span><span class="sxs-lookup"><span data-stu-id="98daf-110">string</span></span>| <span data-ttu-id="98daf-111">キーと値のペアのキー。</span><span class="sxs-lookup"><span data-stu-id="98daf-111">Key for the key-value pair.</span></span> |
|<span data-ttu-id="98daf-112">value</span><span class="sxs-lookup"><span data-stu-id="98daf-112">value</span></span>|<span data-ttu-id="98daf-113">string</span><span class="sxs-lookup"><span data-stu-id="98daf-113">string</span></span>| <span data-ttu-id="98daf-114">キーと値のペアの値。</span><span class="sxs-lookup"><span data-stu-id="98daf-114">Value for the key-value pair.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="98daf-115">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="98daf-115">JSON representation</span></span>

<span data-ttu-id="98daf-116">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="98daf-116">Here is a JSON representation of the resource.</span></span>

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
