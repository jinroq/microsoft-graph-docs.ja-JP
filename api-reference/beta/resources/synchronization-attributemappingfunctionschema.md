---
title: attributeMappingFunctionSchema リソースの種類
description: 同期中に値を変換するための属性のマップで使用できる関数について説明します。
localization_priority: Normal
ms.openlocfilehash: e2c0139f7c797c3f519cc638561b09f611018b28
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511983"
---
# <a name="attributemappingfunctionschema-resource-type"></a><span data-ttu-id="0c8f6-103">attributeMappingFunctionSchema リソースの種類</span><span class="sxs-lookup"><span data-stu-id="0c8f6-103">attributeMappingFunctionSchema resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0c8f6-104">同期中に値を変換するのには、[属性のマッピング](synchronization-attributemapping.md)で使用できる関数について説明します。</span><span class="sxs-lookup"><span data-stu-id="0c8f6-104">Describes a function that can be used in an [attribute mapping](synchronization-attributemapping.md) to transform values during synchronization.</span></span>

## <a name="methods"></a><span data-ttu-id="0c8f6-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="0c8f6-105">Methods</span></span>

| <span data-ttu-id="0c8f6-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="0c8f6-106">Method</span></span>           | <span data-ttu-id="0c8f6-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="0c8f6-107">Return Type</span></span>    |<span data-ttu-id="0c8f6-108">説明</span><span class="sxs-lookup"><span data-stu-id="0c8f6-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="0c8f6-109">List</span><span class="sxs-lookup"><span data-stu-id="0c8f6-109">List</span></span>](../api/synchronization-synchronizationschema-functions.md) | <span data-ttu-id="0c8f6-110">[attributeMappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="0c8f6-110">[attributeMappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md) collection</span></span>|<span data-ttu-id="0c8f6-111">リストがサポートされている属性のマッピング関数。</span><span class="sxs-lookup"><span data-stu-id="0c8f6-111">List supported attribute mapping functions.</span></span>|

## <a name="properties"></a><span data-ttu-id="0c8f6-112">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0c8f6-112">Properties</span></span>

| <span data-ttu-id="0c8f6-113">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0c8f6-113">Property</span></span>                   | <span data-ttu-id="0c8f6-114">型</span><span class="sxs-lookup"><span data-stu-id="0c8f6-114">Type</span></span>                      | <span data-ttu-id="0c8f6-115">説明</span><span class="sxs-lookup"><span data-stu-id="0c8f6-115">Description</span></span>    |
|:---------------------------|:-------------------------|:---------------|
|<span data-ttu-id="0c8f6-116">name</span><span class="sxs-lookup"><span data-stu-id="0c8f6-116">name</span></span>                        |<span data-ttu-id="0c8f6-117">String</span><span class="sxs-lookup"><span data-stu-id="0c8f6-117">String</span></span>                    |<span data-ttu-id="0c8f6-118">オペレーター名です。</span><span class="sxs-lookup"><span data-stu-id="0c8f6-118">Operator name.</span></span> |
|<span data-ttu-id="0c8f6-119">parameters</span><span class="sxs-lookup"><span data-stu-id="0c8f6-119">parameters</span></span>                  |<span data-ttu-id="0c8f6-120">[attributeMappingParameterSchema](../resources/synchronization-attributemappingparameterschema.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="0c8f6-120">[attributeMappingParameterSchema](../resources/synchronization-attributemappingparameterschema.md) collection</span></span>  |<span data-ttu-id="0c8f6-121">関数のパラメーターのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="0c8f6-121">Collection of function parameters.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0c8f6-122">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0c8f6-122">JSON representation</span></span>

<span data-ttu-id="0c8f6-123">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="0c8f6-123">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-attributemappingfunctionschema.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
