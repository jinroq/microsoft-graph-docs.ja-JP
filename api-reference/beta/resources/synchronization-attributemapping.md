---
title: attributeMapping リソースの種類
description: 特定のターゲット属性の値が同期中にどのように流れるかを定義します。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 1f2884a4fc9f4e3091f1e7523c615d9ed132abc6
ms.sourcegitcommit: 121c0fad692fb3c5c01dc051481b5249e4491b48
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/11/2019
ms.locfileid: "35621392"
---
# <a name="attributemapping-resource-type"></a><span data-ttu-id="b2863-103">attributeMapping リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b2863-103">attributeMapping resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b2863-104">特定のターゲット属性の値が同期中にどのように流れるかを定義します。</span><span class="sxs-lookup"><span data-stu-id="b2863-104">Defines how values for the given target attribute should flow during synchronization.</span></span>

## <a name="properties"></a><span data-ttu-id="b2863-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b2863-105">Properties</span></span>

| <span data-ttu-id="b2863-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b2863-106">Property</span></span>                  | <span data-ttu-id="b2863-107">型</span><span class="sxs-lookup"><span data-stu-id="b2863-107">Type</span></span>                      | <span data-ttu-id="b2863-108">説明</span><span class="sxs-lookup"><span data-stu-id="b2863-108">Description</span></span>    |
|:--------------------------|:--------------------------|:---------------|
|<span data-ttu-id="b2863-109">defaultValue</span><span class="sxs-lookup"><span data-stu-id="b2863-109">defaultValue</span></span>               | <span data-ttu-id="b2863-110">String</span><span class="sxs-lookup"><span data-stu-id="b2863-110">String</span></span>                    |<span data-ttu-id="b2863-111">**Source**プロパティがに`null`評価された場合に使用される既定値です。</span><span class="sxs-lookup"><span data-stu-id="b2863-111">Default value to be used in case the **source** property was evaluated to `null`.</span></span> <span data-ttu-id="b2863-112">省略可能。</span><span class="sxs-lookup"><span data-stu-id="b2863-112">Optional.</span></span>|
|<span data-ttu-id="b2863-113">exportMissingReferences</span><span class="sxs-lookup"><span data-stu-id="b2863-113">exportMissingReferences</span></span>    |<span data-ttu-id="b2863-114">String</span><span class="sxs-lookup"><span data-stu-id="b2863-114">String</span></span>                     |<span data-ttu-id="b2863-115">内部使用のために用意されています。</span><span class="sxs-lookup"><span data-stu-id="b2863-115">For internal use only.</span></span>|
|<span data-ttu-id="b2863-116">flowBehavior</span><span class="sxs-lookup"><span data-stu-id="b2863-116">flowBehavior</span></span>               |<span data-ttu-id="b2863-117">attributeFlowBehavior</span><span class="sxs-lookup"><span data-stu-id="b2863-117">attributeFlowBehavior</span></span>      |<span data-ttu-id="b2863-118">この属性をターゲットディレクトリにエクスポートするタイミングを定義します。</span><span class="sxs-lookup"><span data-stu-id="b2863-118">Defines when this attribute should be exported to the target directory.</span></span> <span data-ttu-id="b2863-119">可能な値は`FlowWhenChanged` 、 `FlowAlways`とです。</span><span class="sxs-lookup"><span data-stu-id="b2863-119">Possible values are: `FlowWhenChanged` and `FlowAlways`.</span></span> <span data-ttu-id="b2863-120">既定値は `FlowWhenChanged` です。</span><span class="sxs-lookup"><span data-stu-id="b2863-120">Default is `FlowWhenChanged`.</span></span> |
|<span data-ttu-id="b2863-121">flowType</span><span class="sxs-lookup"><span data-stu-id="b2863-121">flowType</span></span>                   |<span data-ttu-id="b2863-122">attributeFlowType</span><span class="sxs-lookup"><span data-stu-id="b2863-122">attributeFlowType</span></span>          |<span data-ttu-id="b2863-123">この属性をターゲットディレクトリでいつ更新する必要があるかを定義します。</span><span class="sxs-lookup"><span data-stu-id="b2863-123">Defines when this attribute should be updated in the target directory.</span></span> <span data-ttu-id="b2863-124">可能な値は`Always`次のとおりです`ObjectAddOnly` (既定値)。 (新しいオブジェクトが`MultiValueAddOnly`作成された場合のみ)、(変更によって新しい値が複数値属性に追加されている場合のみ)。</span><span class="sxs-lookup"><span data-stu-id="b2863-124">Possible values are: `Always` (default), `ObjectAddOnly` (only when new object is created), `MultiValueAddOnly` (only when the change is adding new values to a multi-valued attribute).</span></span> |
|<span data-ttu-id="b2863-125">matchingPriority</span><span class="sxs-lookup"><span data-stu-id="b2863-125">matchingPriority</span></span>           |<span data-ttu-id="b2863-126">Int32</span><span class="sxs-lookup"><span data-stu-id="b2863-126">Int32</span></span>                      |<span data-ttu-id="b2863-127">0より大きい場合は、この属性を使用して、ソースディレクトリとターゲットディレクトリの間でオブジェクトの初期一致を実行します。</span><span class="sxs-lookup"><span data-stu-id="b2863-127">If higher than 0, this attribute will be used to perform an initial match of the objects between source and target directories.</span></span> <span data-ttu-id="b2863-128">同期エンジンは、一致する優先度の値が最も小さい属性を使用して、一致するオブジェクトを検索します。</span><span class="sxs-lookup"><span data-stu-id="b2863-128">The synchronization engine will try to find the matching object using attribute with lowest value of matching priority first.</span></span> <span data-ttu-id="b2863-129">見つからない場合は、次に一致する優先度の属性が使用され、一致が見つかるまで、またはそれ以上一致する属性が残っていないことを示します。</span><span class="sxs-lookup"><span data-stu-id="b2863-129">If not found, the attribute with the next matching priority will be used, and so on a until match is found or no more matching attributes are left.</span></span> <span data-ttu-id="b2863-130">電子メールなどの一意の値を持つことが予想される属性のみを一致属性として使用する必要があります。</span><span class="sxs-lookup"><span data-stu-id="b2863-130">Only attributes that are expected to have unique values, such as email, should be used as matching attributes.</span></span>|
|<span data-ttu-id="b2863-131">source</span><span class="sxs-lookup"><span data-stu-id="b2863-131">source</span></span>                     |[<span data-ttu-id="b2863-132">attributeMappingSource</span><span class="sxs-lookup"><span data-stu-id="b2863-132">attributeMappingSource</span></span>](synchronization-attributemappingsource.md)     | <span data-ttu-id="b2863-133">ソースオブジェクトから値を抽出 (変換) する方法を定義します。</span><span class="sxs-lookup"><span data-stu-id="b2863-133">Defines how a value should be extracted (or transformed) from the source object.</span></span> |
|<span data-ttu-id="b2863-134">targetAttributeName</span><span class="sxs-lookup"><span data-stu-id="b2863-134">targetAttributeName</span></span>        |<span data-ttu-id="b2863-135">String</span><span class="sxs-lookup"><span data-stu-id="b2863-135">String</span></span>                     |<span data-ttu-id="b2863-136">ターゲットオブジェクトの属性の名前。</span><span class="sxs-lookup"><span data-stu-id="b2863-136">Name of the attribute on the target object.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="b2863-137">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b2863-137">JSON representation</span></span>

<span data-ttu-id="b2863-138">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="b2863-138">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.attributeMapping"
}-->

```json
{
  "defaultValue": "String",
  "exportMissingReferences": true,
  "flowBehavior": "String",
  "flowType": "String",
  "matchingPriority": 1024,
  "source": {"@odata.type": "microsoft.graph.attributeMappingSource"},
  "targetAttributeName": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "attributeMapping resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
