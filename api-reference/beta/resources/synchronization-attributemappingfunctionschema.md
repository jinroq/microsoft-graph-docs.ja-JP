---
title: attributeMappingFunctionSchema リソースの種類
description: 同期時に値を変換するために属性マッピングで使用できる関数について説明します。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 2290f2c3140d9c955dc3a3d4bc72f9b953a7775f
ms.sourcegitcommit: 121c0fad692fb3c5c01dc051481b5249e4491b48
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/11/2019
ms.locfileid: "35620284"
---
# <a name="attributemappingfunctionschema-resource-type"></a><span data-ttu-id="31a4c-103">attributeMappingFunctionSchema リソースの種類</span><span class="sxs-lookup"><span data-stu-id="31a4c-103">attributeMappingFunctionSchema resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="31a4c-104">同期時に値を変換するために[属性マッピング](synchronization-attributemapping.md)で使用できる関数について説明します。</span><span class="sxs-lookup"><span data-stu-id="31a4c-104">Describes a function that can be used in an [attribute mapping](synchronization-attributemapping.md) to transform values during synchronization.</span></span>

## <a name="methods"></a><span data-ttu-id="31a4c-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="31a4c-105">Methods</span></span>

| <span data-ttu-id="31a4c-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="31a4c-106">Method</span></span>           | <span data-ttu-id="31a4c-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="31a4c-107">Return Type</span></span>    |<span data-ttu-id="31a4c-108">説明</span><span class="sxs-lookup"><span data-stu-id="31a4c-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="31a4c-109">List</span><span class="sxs-lookup"><span data-stu-id="31a4c-109">List</span></span>](../api/synchronization-synchronizationschema-functions.md) | <span data-ttu-id="31a4c-110">[attributeMappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="31a4c-110">[attributeMappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md) collection</span></span>|<span data-ttu-id="31a4c-111">サポートされている属性マッピング関数を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="31a4c-111">List supported attribute mapping functions.</span></span>|

## <a name="properties"></a><span data-ttu-id="31a4c-112">プロパティ</span><span class="sxs-lookup"><span data-stu-id="31a4c-112">Properties</span></span>

| <span data-ttu-id="31a4c-113">プロパティ</span><span class="sxs-lookup"><span data-stu-id="31a4c-113">Property</span></span>                   | <span data-ttu-id="31a4c-114">型</span><span class="sxs-lookup"><span data-stu-id="31a4c-114">Type</span></span>                      | <span data-ttu-id="31a4c-115">説明</span><span class="sxs-lookup"><span data-stu-id="31a4c-115">Description</span></span>    |
|:---------------------------|:-------------------------|:---------------|
|<span data-ttu-id="31a4c-116">name</span><span class="sxs-lookup"><span data-stu-id="31a4c-116">name</span></span>                        |<span data-ttu-id="31a4c-117">String</span><span class="sxs-lookup"><span data-stu-id="31a4c-117">String</span></span>                    |<span data-ttu-id="31a4c-118">オペレーター名。</span><span class="sxs-lookup"><span data-stu-id="31a4c-118">Operator name.</span></span> |
|<span data-ttu-id="31a4c-119">parameters</span><span class="sxs-lookup"><span data-stu-id="31a4c-119">parameters</span></span>                  |<span data-ttu-id="31a4c-120">[attributeMappingParameterSchema](../resources/synchronization-attributemappingparameterschema.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="31a4c-120">[attributeMappingParameterSchema](../resources/synchronization-attributemappingparameterschema.md) collection</span></span>  |<span data-ttu-id="31a4c-121">関数パラメータのコレクション。</span><span class="sxs-lookup"><span data-stu-id="31a4c-121">Collection of function parameters.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="31a4c-122">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="31a4c-122">JSON representation</span></span>

<span data-ttu-id="31a4c-123">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="31a4c-123">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.attributeMappingFunctionSchema"
}-->

```json
{
  "name": "String (identifier)",
  "parameters": [{"@odata.type": "microsoft.graph.attributeMappingParameterSchema"}]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "attributeMappingFunctionSchema resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
