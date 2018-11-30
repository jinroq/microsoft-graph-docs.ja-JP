---
title: attributeMapping リソースの種類
description: 特定のターゲット属性の値が同期中にフローは方法を定義します。
ms.openlocfilehash: e4fd8ba0aece448f358d51373dfca0157759a23e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27069846"
---
# <a name="attributemapping-resource-type"></a><span data-ttu-id="d9e1b-103">attributeMapping リソースの種類</span><span class="sxs-lookup"><span data-stu-id="d9e1b-103">attributeMapping resource type</span></span>

> <span data-ttu-id="d9e1b-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="d9e1b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d9e1b-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d9e1b-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d9e1b-106">特定のターゲット属性の値が同期中にフローは方法を定義します。</span><span class="sxs-lookup"><span data-stu-id="d9e1b-106">Defines how values for the given target attribute should flow during synchronization.</span></span>

## <a name="properties"></a><span data-ttu-id="d9e1b-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d9e1b-107">Properties</span></span>

| <span data-ttu-id="d9e1b-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d9e1b-108">Property</span></span>                  | <span data-ttu-id="d9e1b-109">型</span><span class="sxs-lookup"><span data-stu-id="d9e1b-109">Type</span></span>                      | <span data-ttu-id="d9e1b-110">説明</span><span class="sxs-lookup"><span data-stu-id="d9e1b-110">Description</span></span>    |
|:--------------------------|:--------------------------|:---------------|
|<span data-ttu-id="d9e1b-111">defaultValue</span><span class="sxs-lookup"><span data-stu-id="d9e1b-111">defaultValue</span></span>               | <span data-ttu-id="d9e1b-112">文字列</span><span class="sxs-lookup"><span data-stu-id="d9e1b-112">String</span></span>                    |<span data-ttu-id="d9e1b-113">既定値に、 **source**プロパティが評価された場合に使用する`null`。</span><span class="sxs-lookup"><span data-stu-id="d9e1b-113">Default value to be used in case the **source** property was evaluated to `null`.</span></span> <span data-ttu-id="d9e1b-114">省略可能。</span><span class="sxs-lookup"><span data-stu-id="d9e1b-114">Optional.</span></span>|
|<span data-ttu-id="d9e1b-115">exportMissingReferences</span><span class="sxs-lookup"><span data-stu-id="d9e1b-115">exportMissingReferences</span></span>    |<span data-ttu-id="d9e1b-116">String</span><span class="sxs-lookup"><span data-stu-id="d9e1b-116">String</span></span>                     |<span data-ttu-id="d9e1b-117">内部使用のみ。</span><span class="sxs-lookup"><span data-stu-id="d9e1b-117">For internal use only.</span></span>|
|<span data-ttu-id="d9e1b-118">flowBehavior</span><span class="sxs-lookup"><span data-stu-id="d9e1b-118">flowBehavior</span></span>               |<span data-ttu-id="d9e1b-119">attributeFlowBehavior</span><span class="sxs-lookup"><span data-stu-id="d9e1b-119">attributeFlowBehavior</span></span>      |<span data-ttu-id="d9e1b-120">この属性をターゲット ディレクトリにエクスポートするときを定義します。</span><span class="sxs-lookup"><span data-stu-id="d9e1b-120">Defines when this attribute should be exported to the target directory.</span></span> <span data-ttu-id="d9e1b-121">使用可能な値:`FlowWhenChanged`と`FlowAlways`。</span><span class="sxs-lookup"><span data-stu-id="d9e1b-121">Possible values are: `FlowWhenChanged` and `FlowAlways`.</span></span> <span data-ttu-id="d9e1b-122">既定値は `FlowWhenChanged` です。</span><span class="sxs-lookup"><span data-stu-id="d9e1b-122">Default is `FlowWhenChanged`.</span></span> |
|<span data-ttu-id="d9e1b-123">flowType</span><span class="sxs-lookup"><span data-stu-id="d9e1b-123">flowType</span></span>                   |<span data-ttu-id="d9e1b-124">attributeFlowType</span><span class="sxs-lookup"><span data-stu-id="d9e1b-124">attributeFlowType</span></span>          |<span data-ttu-id="d9e1b-125">ターゲット ディレクトリにこの属性を更新するときを定義します。</span><span class="sxs-lookup"><span data-stu-id="d9e1b-125">Defines when this attribute should be updated in the target directory.</span></span> <span data-ttu-id="d9e1b-126">使用可能な値: `Always` (既定値)、 `ObjectAddOnly` (だけ新しいオブジェクトが作成された日時) `MultiValueAddOnly` (のみと変更は、値を追加する新しい複数値を持つ属性に)。</span><span class="sxs-lookup"><span data-stu-id="d9e1b-126">Possible values are: `Always` (default), `ObjectAddOnly` (only when new object is created), `MultiValueAddOnly` (only when the change is adding new values to a multi-valued attribute).</span></span> |
|<span data-ttu-id="d9e1b-127">matchingPriority</span><span class="sxs-lookup"><span data-stu-id="d9e1b-127">matchingPriority</span></span>           |<span data-ttu-id="d9e1b-128">Int32</span><span class="sxs-lookup"><span data-stu-id="d9e1b-128">Int32</span></span>                      |<span data-ttu-id="d9e1b-129">0 よりも大きい場合、は、ソースとターゲットのディレクトリ間でオブジェクトの最初の一致を実行するこの属性が使用されます。</span><span class="sxs-lookup"><span data-stu-id="d9e1b-129">If higher than 0, this attribute will be used to perform an initial match of the objects between source and target directories.</span></span> <span data-ttu-id="d9e1b-130">同期エンジンは、優先度と一致する最初の最小値を持つ属性を使用して一致するオブジェクトを検索しようとしています。</span><span class="sxs-lookup"><span data-stu-id="d9e1b-130">The synchronization engine will try to find the matching object using attribute with lowest value of matching priority first.</span></span> <span data-ttu-id="d9e1b-131">かどうか、次に一致する優先順位を持つ属性を使用してために、一致が見つかったか、これ以上の一致する属性が残っているまでです。</span><span class="sxs-lookup"><span data-stu-id="d9e1b-131">If not found, the attribute with the next matching priority will be used, and so on a until match is found or no more matching attributes are left.</span></span> <span data-ttu-id="d9e1b-132">一致する属性としては、e メールのような一意の値があると予想される属性だけを使用してください。</span><span class="sxs-lookup"><span data-stu-id="d9e1b-132">Only attributes that are expected to have unique values, such as email, should be used as matching attributes.</span></span>|
|<span data-ttu-id="d9e1b-133">source</span><span class="sxs-lookup"><span data-stu-id="d9e1b-133">source</span></span>                     |[<span data-ttu-id="d9e1b-134">attributeMappingSource</span><span class="sxs-lookup"><span data-stu-id="d9e1b-134">attributeMappingSource</span></span>](synchronization-attributemappingsource.md)     | <span data-ttu-id="d9e1b-135">定義の値がどのようにする必要があります抽出 (変換)、ソース オブジェクトからです。</span><span class="sxs-lookup"><span data-stu-id="d9e1b-135">Defines how a value should be extracted (or transformed) from the source object.</span></span> |
|<span data-ttu-id="d9e1b-136">targetAttributeName</span><span class="sxs-lookup"><span data-stu-id="d9e1b-136">targetAttributeName</span></span>        |<span data-ttu-id="d9e1b-137">String</span><span class="sxs-lookup"><span data-stu-id="d9e1b-137">String</span></span>                     |<span data-ttu-id="d9e1b-138">対象のオブジェクトの属性の名前です。</span><span class="sxs-lookup"><span data-stu-id="d9e1b-138">Name of the attribute on the target object.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="d9e1b-139">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d9e1b-139">JSON representation</span></span>

<span data-ttu-id="d9e1b-140">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="d9e1b-140">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "attributeMapping resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->