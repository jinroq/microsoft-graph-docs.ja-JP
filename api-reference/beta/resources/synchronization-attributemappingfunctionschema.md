---
title: attributeMappingFunctionSchema リソースの種類
description: 同期中に値を変換するための属性のマップで使用できる関数について説明します。
localization_priority: Normal
ms.openlocfilehash: 7273534d281d8ea5eaf3709b530776295cd9c767
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27822163"
---
# <a name="attributemappingfunctionschema-resource-type"></a><span data-ttu-id="4c30d-103">attributeMappingFunctionSchema リソースの種類</span><span class="sxs-lookup"><span data-stu-id="4c30d-103">attributeMappingFunctionSchema resource type</span></span>

> <span data-ttu-id="4c30d-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="4c30d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4c30d-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4c30d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4c30d-106">同期中に値を変換するのには、[属性のマッピング](synchronization-attributemapping.md)で使用できる関数について説明します。</span><span class="sxs-lookup"><span data-stu-id="4c30d-106">Describes a function that can be used in an [attribute mapping](synchronization-attributemapping.md) to transform values during synchronization.</span></span>

## <a name="methods"></a><span data-ttu-id="4c30d-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="4c30d-107">Methods</span></span>

| <span data-ttu-id="4c30d-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="4c30d-108">Method</span></span>           | <span data-ttu-id="4c30d-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="4c30d-109">Return Type</span></span>    |<span data-ttu-id="4c30d-110">説明</span><span class="sxs-lookup"><span data-stu-id="4c30d-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="4c30d-111">List</span><span class="sxs-lookup"><span data-stu-id="4c30d-111">List</span></span>](../api/synchronization-synchronizationschema-functions.md) | <span data-ttu-id="4c30d-112">[attributeMappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="4c30d-112">[attributeMappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md) collection</span></span>|<span data-ttu-id="4c30d-113">リストがサポートされている属性のマッピング関数。</span><span class="sxs-lookup"><span data-stu-id="4c30d-113">List supported attribute mapping functions.</span></span>|

## <a name="properties"></a><span data-ttu-id="4c30d-114">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4c30d-114">Properties</span></span>

| <span data-ttu-id="4c30d-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4c30d-115">Property</span></span>                   | <span data-ttu-id="4c30d-116">種類</span><span class="sxs-lookup"><span data-stu-id="4c30d-116">Type</span></span>                      | <span data-ttu-id="4c30d-117">説明</span><span class="sxs-lookup"><span data-stu-id="4c30d-117">Description</span></span>    |
|:---------------------------|:-------------------------|:---------------|
|<span data-ttu-id="4c30d-118">名前</span><span class="sxs-lookup"><span data-stu-id="4c30d-118">name</span></span>                        |<span data-ttu-id="4c30d-119">String</span><span class="sxs-lookup"><span data-stu-id="4c30d-119">String</span></span>                    |<span data-ttu-id="4c30d-120">オペレーター名です。</span><span class="sxs-lookup"><span data-stu-id="4c30d-120">Operator name.</span></span> |
|<span data-ttu-id="4c30d-121">parameters</span><span class="sxs-lookup"><span data-stu-id="4c30d-121">parameters</span></span>                  |<span data-ttu-id="4c30d-122">[attributeMappingParameterSchema](../resources/synchronization-attributemappingparameterschema.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="4c30d-122">[attributeMappingParameterSchema](../resources/synchronization-attributemappingparameterschema.md) collection</span></span>  |<span data-ttu-id="4c30d-123">関数のパラメーターのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="4c30d-123">Collection of function parameters.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4c30d-124">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="4c30d-124">JSON representation</span></span>

<span data-ttu-id="4c30d-125">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="4c30d-125">The following is a JSON representation of the resource.</span></span>

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
