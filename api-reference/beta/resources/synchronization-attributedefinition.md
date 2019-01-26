---
title: attributeDefinition リソースの種類
description: オブジェクトの属性について説明します。
localization_priority: Normal
ms.openlocfilehash: 30c9d6b2f57aaadd9ef17982b1affa765bbfbec0
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/26/2019
ms.locfileid: "29571864"
---
# <a name="attributedefinition-resource-type"></a><span data-ttu-id="4d327-103">attributeDefinition リソースの種類</span><span class="sxs-lookup"><span data-stu-id="4d327-103">attributeDefinition resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4d327-104">オブジェクトの属性について説明します。</span><span class="sxs-lookup"><span data-stu-id="4d327-104">Describes an attribute of an object.</span></span>

## <a name="properties"></a><span data-ttu-id="4d327-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4d327-105">Properties</span></span>

| <span data-ttu-id="4d327-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4d327-106">Property</span></span>      | <span data-ttu-id="4d327-107">型</span><span class="sxs-lookup"><span data-stu-id="4d327-107">Type</span></span>      | <span data-ttu-id="4d327-108">説明</span><span class="sxs-lookup"><span data-stu-id="4d327-108">Description</span></span>    |
|:--------------|:----------|:---------------|
|<span data-ttu-id="4d327-109">アンカー</span><span class="sxs-lookup"><span data-stu-id="4d327-109">anchor</span></span>         |<span data-ttu-id="4d327-110">Boolean</span><span class="sxs-lookup"><span data-stu-id="4d327-110">Boolean</span></span>    | <span data-ttu-id="4d327-111">`true`属性は、オブジェクトのアンカーとして使用する必要があります。 場合、</span><span class="sxs-lookup"><span data-stu-id="4d327-111">`true` if the attribute should be used as the anchor for the object.</span></span> <span data-ttu-id="4d327-112">アンカー属性は、オブジェクトを識別する一意の値を持つ必要があり、不変である必要があります。</span><span class="sxs-lookup"><span data-stu-id="4d327-112">Anchor attributes must have a unique value identifying an object, and must be immutable.</span></span> <span data-ttu-id="4d327-113">既定値は `false` です。</span><span class="sxs-lookup"><span data-stu-id="4d327-113">Default is `false`.</span></span> <span data-ttu-id="4d327-114">のみのいずれか、オブジェクトの属性は、同期をサポートするためにアンカーとして指定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="4d327-114">One, and only one, of the object's attributes must be designated as the anchor to support synchronization.</span></span> |
|<span data-ttu-id="4d327-115">caseExact</span><span class="sxs-lookup"><span data-stu-id="4d327-115">caseExact</span></span>      |<span data-ttu-id="4d327-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="4d327-116">Boolean</span></span>    |<span data-ttu-id="4d327-117">`true`この属性の値を扱う場合、大文字小文字を区別します。</span><span class="sxs-lookup"><span data-stu-id="4d327-117">`true` if value of this attribute should be treated as case-sensitive.</span></span> <span data-ttu-id="4d327-118">この設定は、同期エンジンが、属性の変更を検出する方法に影響します。</span><span class="sxs-lookup"><span data-stu-id="4d327-118">This setting affects how the synchronization engine detects changes for the attribute.</span></span>|
|<span data-ttu-id="4d327-119">metadata</span><span class="sxs-lookup"><span data-stu-id="4d327-119">metadata</span></span>       |<span data-ttu-id="4d327-120">[metadataEntry](../resources/synchronization-metadataentry.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="4d327-120">[metadataEntry](../resources/synchronization-metadataentry.md) collection</span></span> |<span data-ttu-id="4d327-121">プロパティをさらに拡張します。</span><span class="sxs-lookup"><span data-stu-id="4d327-121">Additional extension properties.</span></span> <span data-ttu-id="4d327-122">明示的に記載されている、しない限り、メタデータの値を変更できませんする必要があります。</span><span class="sxs-lookup"><span data-stu-id="4d327-122">Unless mentioned explicitly, metadata values should not be changed.</span></span>|
|<span data-ttu-id="4d327-123">複数値を持つ</span><span class="sxs-lookup"><span data-stu-id="4d327-123">multivalued</span></span>    |<span data-ttu-id="4d327-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="4d327-124">Boolean</span></span>    |<span data-ttu-id="4d327-125">`true`属性は、複数の値を持つことができます。 場合、</span><span class="sxs-lookup"><span data-stu-id="4d327-125">`true` if an attribute can have multiple values.</span></span> <span data-ttu-id="4d327-126">既定値は `false` です。</span><span class="sxs-lookup"><span data-stu-id="4d327-126">Default is `false`.</span></span>|
|<span data-ttu-id="4d327-127">可変性</span><span class="sxs-lookup"><span data-stu-id="4d327-127">mutability</span></span>     |<span data-ttu-id="4d327-128">String</span><span class="sxs-lookup"><span data-stu-id="4d327-128">String</span></span>     |<span data-ttu-id="4d327-129">属性の変更。</span><span class="sxs-lookup"><span data-stu-id="4d327-129">An attribute's mutability.</span></span> <span data-ttu-id="4d327-130">使用可能な値: `ReadWrite`、 `ReadOnly`、 `Immutable`、 `WriteOnly`。</span><span class="sxs-lookup"><span data-stu-id="4d327-130">Possible values are:  `ReadWrite`, `ReadOnly`, `Immutable`, `WriteOnly`.</span></span> <span data-ttu-id="4d327-131">既定値は `ReadWrite` です。</span><span class="sxs-lookup"><span data-stu-id="4d327-131">Default is `ReadWrite`.</span></span>|
|<span data-ttu-id="4d327-132">name</span><span class="sxs-lookup"><span data-stu-id="4d327-132">name</span></span>           |<span data-ttu-id="4d327-133">String</span><span class="sxs-lookup"><span data-stu-id="4d327-133">String</span></span>     |<span data-ttu-id="4d327-134">属性の名前です。</span><span class="sxs-lookup"><span data-stu-id="4d327-134">Name of the attribute.</span></span> <span data-ttu-id="4d327-135">オブジェクト定義内で一意である必要があります。</span><span class="sxs-lookup"><span data-stu-id="4d327-135">Must be unique within the object definition.</span></span> <span data-ttu-id="4d327-136">null 許容ではありません。</span><span class="sxs-lookup"><span data-stu-id="4d327-136">Not nullable.</span></span>|
|<span data-ttu-id="4d327-137">必須</span><span class="sxs-lookup"><span data-stu-id="4d327-137">required</span></span>       |<span data-ttu-id="4d327-138">Boolean</span><span class="sxs-lookup"><span data-stu-id="4d327-138">Boolean</span></span>    |<span data-ttu-id="4d327-139">`true`属性が必要な場合です。</span><span class="sxs-lookup"><span data-stu-id="4d327-139">`true` if attribute is required.</span></span> <span data-ttu-id="4d327-140">必要な属性のいずれかが表示されない場合は、オブジェクトを作成できません。</span><span class="sxs-lookup"><span data-stu-id="4d327-140">Object can not be created if any of the required attributes are missing.</span></span> <span data-ttu-id="4d327-141">場合は、同期時に必要な属性値を持たない、既定値が適用されます。</span><span class="sxs-lookup"><span data-stu-id="4d327-141">If during synchronization, the required attribute has no value, the default value will be used.</span></span> <span data-ttu-id="4d327-142">既定値が設定されていない場合、同期はエラーを記録します。</span><span class="sxs-lookup"><span data-stu-id="4d327-142">If default the value was not set, synchronization will record an error.</span></span>|
|<span data-ttu-id="4d327-143">referencedObjects</span><span class="sxs-lookup"><span data-stu-id="4d327-143">referencedObjects</span></span>|<span data-ttu-id="4d327-144">[referencedObject](../resources/synchronization-referencedobject.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="4d327-144">[referencedObject](../resources/synchronization-referencedobject.md) collection</span></span> |<span data-ttu-id="4d327-145">属性の場合`reference`参照されるオブジェクトのリストを入力します。 (たとえば、、`manager`属性のリストが`User`として参照されているオブジェクト)。</span><span class="sxs-lookup"><span data-stu-id="4d327-145">For attributes with `reference` type, lists referenced objects (for example, the `manager` attribute would list `User` as the referenced object).</span></span>|
|<span data-ttu-id="4d327-146">type</span><span class="sxs-lookup"><span data-stu-id="4d327-146">type</span></span>           |<span data-ttu-id="4d327-147">String</span><span class="sxs-lookup"><span data-stu-id="4d327-147">String</span></span>     |<span data-ttu-id="4d327-148">属性の値の種類。</span><span class="sxs-lookup"><span data-stu-id="4d327-148">Attribute value type.</span></span> <span data-ttu-id="4d327-149">使用可能な値は、`String`、`Integer`、`Reference`、`Binary`、`Boolean` です。</span><span class="sxs-lookup"><span data-stu-id="4d327-149">Possible values are: `String`, `Integer`, `Reference`, `Binary`, `Boolean`.</span></span> <span data-ttu-id="4d327-150">既定値は `String` です。</span><span class="sxs-lookup"><span data-stu-id="4d327-150">Default is `String`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4d327-151">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="4d327-151">JSON representation</span></span>

<span data-ttu-id="4d327-152">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="4d327-152">The following is a JSON representation of the resource.</span></span>

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
