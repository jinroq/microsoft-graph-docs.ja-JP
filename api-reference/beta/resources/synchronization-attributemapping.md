---
title: attributeMapping リソースの種類
description: 特定のターゲット属性の値が同期中にフローは方法を定義します。
localization_priority: Normal
ms.openlocfilehash: 16235cce73a17b462f6f44aedf0c8759277983c1
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29509323"
---
# <a name="attributemapping-resource-type"></a><span data-ttu-id="16f93-103">attributeMapping リソースの種類</span><span class="sxs-lookup"><span data-stu-id="16f93-103">attributeMapping resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="16f93-104">特定のターゲット属性の値が同期中にフローは方法を定義します。</span><span class="sxs-lookup"><span data-stu-id="16f93-104">Defines how values for the given target attribute should flow during synchronization.</span></span>

## <a name="properties"></a><span data-ttu-id="16f93-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="16f93-105">Properties</span></span>

| <span data-ttu-id="16f93-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="16f93-106">Property</span></span>                  | <span data-ttu-id="16f93-107">型</span><span class="sxs-lookup"><span data-stu-id="16f93-107">Type</span></span>                      | <span data-ttu-id="16f93-108">説明</span><span class="sxs-lookup"><span data-stu-id="16f93-108">Description</span></span>    |
|:--------------------------|:--------------------------|:---------------|
|<span data-ttu-id="16f93-109">defaultValue</span><span class="sxs-lookup"><span data-stu-id="16f93-109">defaultValue</span></span>               | <span data-ttu-id="16f93-110">文字列</span><span class="sxs-lookup"><span data-stu-id="16f93-110">String</span></span>                    |<span data-ttu-id="16f93-111">既定値に、 **source**プロパティが評価された場合に使用する`null`。</span><span class="sxs-lookup"><span data-stu-id="16f93-111">Default value to be used in case the **source** property was evaluated to `null`.</span></span> <span data-ttu-id="16f93-112">省略可能。</span><span class="sxs-lookup"><span data-stu-id="16f93-112">Optional.</span></span>|
|<span data-ttu-id="16f93-113">exportMissingReferences</span><span class="sxs-lookup"><span data-stu-id="16f93-113">exportMissingReferences</span></span>    |<span data-ttu-id="16f93-114">String</span><span class="sxs-lookup"><span data-stu-id="16f93-114">String</span></span>                     |<span data-ttu-id="16f93-115">内部使用のみ。</span><span class="sxs-lookup"><span data-stu-id="16f93-115">For internal use only.</span></span>|
|<span data-ttu-id="16f93-116">flowBehavior</span><span class="sxs-lookup"><span data-stu-id="16f93-116">flowBehavior</span></span>               |<span data-ttu-id="16f93-117">attributeFlowBehavior</span><span class="sxs-lookup"><span data-stu-id="16f93-117">attributeFlowBehavior</span></span>      |<span data-ttu-id="16f93-118">この属性をターゲット ディレクトリにエクスポートするときを定義します。</span><span class="sxs-lookup"><span data-stu-id="16f93-118">Defines when this attribute should be exported to the target directory.</span></span> <span data-ttu-id="16f93-119">使用可能な値:`FlowWhenChanged`と`FlowAlways`。</span><span class="sxs-lookup"><span data-stu-id="16f93-119">Possible values are: `FlowWhenChanged` and `FlowAlways`.</span></span> <span data-ttu-id="16f93-120">既定値は `FlowWhenChanged` です。</span><span class="sxs-lookup"><span data-stu-id="16f93-120">Default is `FlowWhenChanged`.</span></span> |
|<span data-ttu-id="16f93-121">flowType</span><span class="sxs-lookup"><span data-stu-id="16f93-121">flowType</span></span>                   |<span data-ttu-id="16f93-122">attributeFlowType</span><span class="sxs-lookup"><span data-stu-id="16f93-122">attributeFlowType</span></span>          |<span data-ttu-id="16f93-123">ターゲット ディレクトリにこの属性を更新するときを定義します。</span><span class="sxs-lookup"><span data-stu-id="16f93-123">Defines when this attribute should be updated in the target directory.</span></span> <span data-ttu-id="16f93-124">使用可能な値: `Always` (既定値)、 `ObjectAddOnly` (だけ新しいオブジェクトが作成された日時) `MultiValueAddOnly` (のみと変更は、値を追加する新しい複数値を持つ属性に)。</span><span class="sxs-lookup"><span data-stu-id="16f93-124">Possible values are: `Always` (default), `ObjectAddOnly` (only when new object is created), `MultiValueAddOnly` (only when the change is adding new values to a multi-valued attribute).</span></span> |
|<span data-ttu-id="16f93-125">matchingPriority</span><span class="sxs-lookup"><span data-stu-id="16f93-125">matchingPriority</span></span>           |<span data-ttu-id="16f93-126">Int32</span><span class="sxs-lookup"><span data-stu-id="16f93-126">Int32</span></span>                      |<span data-ttu-id="16f93-127">0 よりも大きい場合、は、ソースとターゲットのディレクトリ間でオブジェクトの最初の一致を実行するこの属性が使用されます。</span><span class="sxs-lookup"><span data-stu-id="16f93-127">If higher than 0, this attribute will be used to perform an initial match of the objects between source and target directories.</span></span> <span data-ttu-id="16f93-128">同期エンジンは、優先度と一致する最初の最小値を持つ属性を使用して一致するオブジェクトを検索しようとしています。</span><span class="sxs-lookup"><span data-stu-id="16f93-128">The synchronization engine will try to find the matching object using attribute with lowest value of matching priority first.</span></span> <span data-ttu-id="16f93-129">かどうか、次に一致する優先順位を持つ属性を使用してために、一致が見つかったか、これ以上の一致する属性が残っているまでです。</span><span class="sxs-lookup"><span data-stu-id="16f93-129">If not found, the attribute with the next matching priority will be used, and so on a until match is found or no more matching attributes are left.</span></span> <span data-ttu-id="16f93-130">一致する属性としては、e メールのような一意の値があると予想される属性だけを使用してください。</span><span class="sxs-lookup"><span data-stu-id="16f93-130">Only attributes that are expected to have unique values, such as email, should be used as matching attributes.</span></span>|
|<span data-ttu-id="16f93-131">source</span><span class="sxs-lookup"><span data-stu-id="16f93-131">source</span></span>                     |[<span data-ttu-id="16f93-132">attributeMappingSource</span><span class="sxs-lookup"><span data-stu-id="16f93-132">attributeMappingSource</span></span>](synchronization-attributemappingsource.md)     | <span data-ttu-id="16f93-133">定義の値がどのようにする必要があります抽出 (変換)、ソース オブジェクトからです。</span><span class="sxs-lookup"><span data-stu-id="16f93-133">Defines how a value should be extracted (or transformed) from the source object.</span></span> |
|<span data-ttu-id="16f93-134">targetAttributeName</span><span class="sxs-lookup"><span data-stu-id="16f93-134">targetAttributeName</span></span>        |<span data-ttu-id="16f93-135">String</span><span class="sxs-lookup"><span data-stu-id="16f93-135">String</span></span>                     |<span data-ttu-id="16f93-136">対象のオブジェクトの属性の名前です。</span><span class="sxs-lookup"><span data-stu-id="16f93-136">Name of the attribute on the target object.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="16f93-137">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="16f93-137">JSON representation</span></span>

<span data-ttu-id="16f93-138">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="16f93-138">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-attributemapping.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
