---
title: attributeMappingFunctionSchema リソースの種類
description: 同期中に値を変換するための属性のマップで使用できる関数について説明します。
ms.openlocfilehash: 9760669bb29700bfa79c1cd375857b4fd673879b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27070376"
---
# <a name="attributemappingfunctionschema-resource-type"></a><span data-ttu-id="ab80c-103">attributeMappingFunctionSchema リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ab80c-103">attributeMappingFunctionSchema resource type</span></span>

> <span data-ttu-id="ab80c-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="ab80c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ab80c-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ab80c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ab80c-106">同期中に値を変換するのには、[属性のマッピング](synchronization-attributemapping.md)で使用できる関数について説明します。</span><span class="sxs-lookup"><span data-stu-id="ab80c-106">Describes a function that can be used in an [attribute mapping](synchronization-attributemapping.md) to transform values during synchronization.</span></span>

## <a name="methods"></a><span data-ttu-id="ab80c-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="ab80c-107">Methods</span></span>

| <span data-ttu-id="ab80c-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="ab80c-108">Method</span></span>           | <span data-ttu-id="ab80c-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="ab80c-109">Return Type</span></span>    |<span data-ttu-id="ab80c-110">説明</span><span class="sxs-lookup"><span data-stu-id="ab80c-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ab80c-111">List</span><span class="sxs-lookup"><span data-stu-id="ab80c-111">List</span></span>](../api/synchronization-synchronizationschema-functions.md) | <span data-ttu-id="ab80c-112">[attributeMappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="ab80c-112">[attributeMappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md) collection</span></span>|<span data-ttu-id="ab80c-113">リストがサポートされている属性のマッピング関数。</span><span class="sxs-lookup"><span data-stu-id="ab80c-113">List supported attribute mapping functions.</span></span>|

## <a name="properties"></a><span data-ttu-id="ab80c-114">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ab80c-114">Properties</span></span>

| <span data-ttu-id="ab80c-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ab80c-115">Property</span></span>                   | <span data-ttu-id="ab80c-116">型</span><span class="sxs-lookup"><span data-stu-id="ab80c-116">Type</span></span>                      | <span data-ttu-id="ab80c-117">説明</span><span class="sxs-lookup"><span data-stu-id="ab80c-117">Description</span></span>    |
|:---------------------------|:-------------------------|:---------------|
|<span data-ttu-id="ab80c-118">名前</span><span class="sxs-lookup"><span data-stu-id="ab80c-118">name</span></span>                        |<span data-ttu-id="ab80c-119">String</span><span class="sxs-lookup"><span data-stu-id="ab80c-119">String</span></span>                    |<span data-ttu-id="ab80c-120">オペレーター名です。</span><span class="sxs-lookup"><span data-stu-id="ab80c-120">Operator name.</span></span> |
|<span data-ttu-id="ab80c-121">parameters</span><span class="sxs-lookup"><span data-stu-id="ab80c-121">parameters</span></span>                  |<span data-ttu-id="ab80c-122">[attributeMappingParameterSchema](../resources/synchronization-attributemappingparameterschema.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="ab80c-122">[attributeMappingParameterSchema](../resources/synchronization-attributemappingparameterschema.md) collection</span></span>  |<span data-ttu-id="ab80c-123">関数のパラメーターのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="ab80c-123">Collection of function parameters.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ab80c-124">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ab80c-124">JSON representation</span></span>

<span data-ttu-id="ab80c-125">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="ab80c-125">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "attributeMappingFunctionSchema resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->