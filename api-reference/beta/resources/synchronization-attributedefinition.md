---
title: attributedefinition リソースの種類
description: オブジェクトの属性を表します。
localization_priority: Normal
ms.openlocfilehash: f9268bf61fec397c53744c9999635ba159b047f4
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32582086"
---
# <a name="attributedefinition-resource-type"></a><span data-ttu-id="88faa-103">attributedefinition リソースの種類</span><span class="sxs-lookup"><span data-stu-id="88faa-103">attributeDefinition resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="88faa-104">オブジェクトの属性を表します。</span><span class="sxs-lookup"><span data-stu-id="88faa-104">Describes an attribute of an object.</span></span>

## <a name="properties"></a><span data-ttu-id="88faa-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="88faa-105">Properties</span></span>

| <span data-ttu-id="88faa-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="88faa-106">Property</span></span>      | <span data-ttu-id="88faa-107">型</span><span class="sxs-lookup"><span data-stu-id="88faa-107">Type</span></span>      | <span data-ttu-id="88faa-108">説明</span><span class="sxs-lookup"><span data-stu-id="88faa-108">Description</span></span>    |
|:--------------|:----------|:---------------|
|<span data-ttu-id="88faa-109">位置</span><span class="sxs-lookup"><span data-stu-id="88faa-109">anchor</span></span>         |<span data-ttu-id="88faa-110">Boolean</span><span class="sxs-lookup"><span data-stu-id="88faa-110">Boolean</span></span>    | <span data-ttu-id="88faa-111">`true`オブジェクトのアンカーとして属性を使用する必要があるかどうか。</span><span class="sxs-lookup"><span data-stu-id="88faa-111">`true` if the attribute should be used as the anchor for the object.</span></span> <span data-ttu-id="88faa-112">アンカー属性には、オブジェクトを識別する一意の値を指定する必要があります。不変にする必要があります。</span><span class="sxs-lookup"><span data-stu-id="88faa-112">Anchor attributes must have a unique value identifying an object, and must be immutable.</span></span> <span data-ttu-id="88faa-113">既定値は `false` です。</span><span class="sxs-lookup"><span data-stu-id="88faa-113">Default is `false`.</span></span> <span data-ttu-id="88faa-114">同期をサポートするには、オブジェクトの属性の1つだけをアンカーとして指定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="88faa-114">One, and only one, of the object's attributes must be designated as the anchor to support synchronization.</span></span> |
|<span data-ttu-id="88faa-115">ケース exact</span><span class="sxs-lookup"><span data-stu-id="88faa-115">caseExact</span></span>      |<span data-ttu-id="88faa-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="88faa-116">Boolean</span></span>    |<span data-ttu-id="88faa-117">`true`この属性の値を大文字と小文字を区別して扱う必要がある場合。</span><span class="sxs-lookup"><span data-stu-id="88faa-117">`true` if value of this attribute should be treated as case-sensitive.</span></span> <span data-ttu-id="88faa-118">この設定は、同期エンジンが属性の変更を検出する方法に影響します。</span><span class="sxs-lookup"><span data-stu-id="88faa-118">This setting affects how the synchronization engine detects changes for the attribute.</span></span>|
|<span data-ttu-id="88faa-119">metadata</span><span class="sxs-lookup"><span data-stu-id="88faa-119">metadata</span></span>       |[<span data-ttu-id="88faa-120">metadataentry</span><span class="sxs-lookup"><span data-stu-id="88faa-120">metadataEntry</span></span>](../resources/synchronization-metadataentry.md)    |<span data-ttu-id="88faa-121">追加の拡張機能のプロパティ。</span><span class="sxs-lookup"><span data-stu-id="88faa-121">Additional extension properties.</span></span> <span data-ttu-id="88faa-122">明示的に記述されていない限り、メタデータ値は変更しないでください。</span><span class="sxs-lookup"><span data-stu-id="88faa-122">Unless mentioned explicitly, metadata values should not be changed.</span></span>|
|<span data-ttu-id="88faa-123">複数値</span><span class="sxs-lookup"><span data-stu-id="88faa-123">multivalued</span></span>    |<span data-ttu-id="88faa-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="88faa-124">Boolean</span></span>    |<span data-ttu-id="88faa-125">`true`属性に複数の値を設定できる場合。</span><span class="sxs-lookup"><span data-stu-id="88faa-125">`true` if an attribute can have multiple values.</span></span> <span data-ttu-id="88faa-126">既定値は `false` です。</span><span class="sxs-lookup"><span data-stu-id="88faa-126">Default is `false`.</span></span>|
|<span data-ttu-id="88faa-127">mutability</span><span class="sxs-lookup"><span data-stu-id="88faa-127">mutability</span></span>     |<span data-ttu-id="88faa-128">String</span><span class="sxs-lookup"><span data-stu-id="88faa-128">String</span></span>     |<span data-ttu-id="88faa-129">属性の変わり可能性。</span><span class="sxs-lookup"><span data-stu-id="88faa-129">An attribute's mutability.</span></span> <span data-ttu-id="88faa-130">可能な値は`ReadWrite`、 `ReadOnly`、 `Immutable`、 `WriteOnly`、です。</span><span class="sxs-lookup"><span data-stu-id="88faa-130">Possible values are:  `ReadWrite`, `ReadOnly`, `Immutable`, `WriteOnly`.</span></span> <span data-ttu-id="88faa-131">既定値は `ReadWrite` です。</span><span class="sxs-lookup"><span data-stu-id="88faa-131">Default is `ReadWrite`.</span></span>|
|<span data-ttu-id="88faa-132">name</span><span class="sxs-lookup"><span data-stu-id="88faa-132">name</span></span>           |<span data-ttu-id="88faa-133">String</span><span class="sxs-lookup"><span data-stu-id="88faa-133">String</span></span>     |<span data-ttu-id="88faa-134">属性の名前。</span><span class="sxs-lookup"><span data-stu-id="88faa-134">Name of the attribute.</span></span> <span data-ttu-id="88faa-135">オブジェクト定義内で一意である必要があります。</span><span class="sxs-lookup"><span data-stu-id="88faa-135">Must be unique within the object definition.</span></span> <span data-ttu-id="88faa-136">null 許容ではありません。</span><span class="sxs-lookup"><span data-stu-id="88faa-136">Not nullable.</span></span>|
|<span data-ttu-id="88faa-137">必須</span><span class="sxs-lookup"><span data-stu-id="88faa-137">required</span></span>       |<span data-ttu-id="88faa-138">Boolean</span><span class="sxs-lookup"><span data-stu-id="88faa-138">Boolean</span></span>    |<span data-ttu-id="88faa-139">`true`属性が必要かどうか。</span><span class="sxs-lookup"><span data-stu-id="88faa-139">`true` if attribute is required.</span></span> <span data-ttu-id="88faa-140">必要な属性のいずれかが不足している場合は、オブジェクトを作成できません。</span><span class="sxs-lookup"><span data-stu-id="88faa-140">Object can not be created if any of the required attributes are missing.</span></span> <span data-ttu-id="88faa-141">同期時に必須属性に値がない場合は、既定値が使用されます。</span><span class="sxs-lookup"><span data-stu-id="88faa-141">If during synchronization, the required attribute has no value, the default value will be used.</span></span> <span data-ttu-id="88faa-142">既定値が設定されていない場合は、同期によってエラーが記録されます。</span><span class="sxs-lookup"><span data-stu-id="88faa-142">If default the value was not set, synchronization will record an error.</span></span>|
|<span data-ttu-id="88faa-143">referencedopivot</span><span class="sxs-lookup"><span data-stu-id="88faa-143">referencedObjects</span></span>|[<span data-ttu-id="88faa-144">referencedobject</span><span class="sxs-lookup"><span data-stu-id="88faa-144">referencedObject</span></span>](../resources/synchronization-referencedobject.md) |<span data-ttu-id="88faa-145">type の属性の場合は、参照されているオブジェクト`manager`を一覧表示`User`します (たとえば、属性が参照されるオブジェクトとしてリストになります)。 `reference`</span><span class="sxs-lookup"><span data-stu-id="88faa-145">For attributes with `reference` type, lists referenced objects (for example, the `manager` attribute would list `User` as the referenced object).</span></span>|
|<span data-ttu-id="88faa-146">type</span><span class="sxs-lookup"><span data-stu-id="88faa-146">type</span></span>           |<span data-ttu-id="88faa-147">String</span><span class="sxs-lookup"><span data-stu-id="88faa-147">String</span></span>     |<span data-ttu-id="88faa-148">属性値の型。</span><span class="sxs-lookup"><span data-stu-id="88faa-148">Attribute value type.</span></span> <span data-ttu-id="88faa-149">使用可能な値は、`String`、`Integer`、`Reference`、`Binary`、`Boolean` です。</span><span class="sxs-lookup"><span data-stu-id="88faa-149">Possible values are: `String`, `Integer`, `Reference`, `Binary`, `Boolean`.</span></span> <span data-ttu-id="88faa-150">既定値は `String` です。</span><span class="sxs-lookup"><span data-stu-id="88faa-150">Default is `String`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="88faa-151">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="88faa-151">JSON representation</span></span>

<span data-ttu-id="88faa-152">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="88faa-152">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.attributeDefinition"
}-->

```json
{
  "anchor": true,
  "caseExact": true,
  "defaultValue": "String",
  "metadata": [{"@odata.type": "microsoft.graph.metadataEntry"}],
  "multivalued": true,
  "mutability": "String",
  "name": "String",
  "referencedObjects": [{"@odata.type": "microsoft.graph.referencedObject"}],
  "required": true,
  "type": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "attributeDefinition resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-attributedefinition.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
