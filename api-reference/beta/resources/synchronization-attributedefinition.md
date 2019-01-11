---
title: attributeDefinition リソースの種類
description: オブジェクトの属性について説明します。
localization_priority: Normal
ms.openlocfilehash: 63b7f67808ab6695b30f5464d72aed2814e46c5a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27829681"
---
# <a name="attributedefinition-resource-type"></a><span data-ttu-id="ce6fc-103">attributeDefinition リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ce6fc-103">attributeDefinition resource type</span></span>

> <span data-ttu-id="ce6fc-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="ce6fc-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ce6fc-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ce6fc-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ce6fc-106">オブジェクトの属性について説明します。</span><span class="sxs-lookup"><span data-stu-id="ce6fc-106">Describes an attribute of an object.</span></span>

## <a name="properties"></a><span data-ttu-id="ce6fc-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ce6fc-107">Properties</span></span>

| <span data-ttu-id="ce6fc-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ce6fc-108">Property</span></span>      | <span data-ttu-id="ce6fc-109">種類</span><span class="sxs-lookup"><span data-stu-id="ce6fc-109">Type</span></span>      | <span data-ttu-id="ce6fc-110">説明</span><span class="sxs-lookup"><span data-stu-id="ce6fc-110">Description</span></span>    |
|:--------------|:----------|:---------------|
|<span data-ttu-id="ce6fc-111">アンカー</span><span class="sxs-lookup"><span data-stu-id="ce6fc-111">anchor</span></span>         |<span data-ttu-id="ce6fc-112">ブール型</span><span class="sxs-lookup"><span data-stu-id="ce6fc-112">Boolean</span></span>    | <span data-ttu-id="ce6fc-113">`true`属性は、オブジェクトのアンカーとして使用する必要があります。 場合、</span><span class="sxs-lookup"><span data-stu-id="ce6fc-113">`true` if the attribute should be used as the anchor for the object.</span></span> <span data-ttu-id="ce6fc-114">アンカー属性は、オブジェクトを識別する一意の値を持つ必要があり、不変である必要があります。</span><span class="sxs-lookup"><span data-stu-id="ce6fc-114">Anchor attributes must have a unique value identifying an object, and must be immutable.</span></span> <span data-ttu-id="ce6fc-115">既定値は `false` です。</span><span class="sxs-lookup"><span data-stu-id="ce6fc-115">Default is `false`.</span></span> <span data-ttu-id="ce6fc-116">のみのいずれか、オブジェクトの属性は、同期をサポートするためにアンカーとして指定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="ce6fc-116">One, and only one, of the object's attributes must be designated as the anchor to support synchronization.</span></span> |
|<span data-ttu-id="ce6fc-117">caseExact</span><span class="sxs-lookup"><span data-stu-id="ce6fc-117">caseExact</span></span>      |<span data-ttu-id="ce6fc-118">ブール型</span><span class="sxs-lookup"><span data-stu-id="ce6fc-118">Boolean</span></span>    |<span data-ttu-id="ce6fc-119">`true`この属性の値を扱う場合、大文字小文字を区別します。</span><span class="sxs-lookup"><span data-stu-id="ce6fc-119">`true` if value of this attribute should be treated as case-sensitive.</span></span> <span data-ttu-id="ce6fc-120">この設定は、同期エンジンが、属性の変更を検出する方法に影響します。</span><span class="sxs-lookup"><span data-stu-id="ce6fc-120">This setting affects how the synchronization engine detects changes for the attribute.</span></span>|
|<span data-ttu-id="ce6fc-121">metadata</span><span class="sxs-lookup"><span data-stu-id="ce6fc-121">metadata</span></span>       |[<span data-ttu-id="ce6fc-122">metadataEntry</span><span class="sxs-lookup"><span data-stu-id="ce6fc-122">metadataEntry</span></span>](../resources/synchronization-metadataentry.md)    |<span data-ttu-id="ce6fc-123">プロパティをさらに拡張します。</span><span class="sxs-lookup"><span data-stu-id="ce6fc-123">Additional extension properties.</span></span> <span data-ttu-id="ce6fc-124">明示的に記載されている、しない限り、メタデータの値を変更できませんする必要があります。</span><span class="sxs-lookup"><span data-stu-id="ce6fc-124">Unless mentioned explicitly, metadata values should not be changed.</span></span>|
|<span data-ttu-id="ce6fc-125">複数値を持つ</span><span class="sxs-lookup"><span data-stu-id="ce6fc-125">multivalued</span></span>    |<span data-ttu-id="ce6fc-126">ブール型</span><span class="sxs-lookup"><span data-stu-id="ce6fc-126">Boolean</span></span>    |<span data-ttu-id="ce6fc-127">`true`属性は、複数の値を持つことができます。 場合、</span><span class="sxs-lookup"><span data-stu-id="ce6fc-127">`true` if an attribute can have multiple values.</span></span> <span data-ttu-id="ce6fc-128">既定値は `false` です。</span><span class="sxs-lookup"><span data-stu-id="ce6fc-128">Default is `false`.</span></span>|
|<span data-ttu-id="ce6fc-129">可変性</span><span class="sxs-lookup"><span data-stu-id="ce6fc-129">mutability</span></span>     |<span data-ttu-id="ce6fc-130">String</span><span class="sxs-lookup"><span data-stu-id="ce6fc-130">String</span></span>     |<span data-ttu-id="ce6fc-131">属性の変更。</span><span class="sxs-lookup"><span data-stu-id="ce6fc-131">An attribute's mutability.</span></span> <span data-ttu-id="ce6fc-132">使用可能な値: `ReadWrite`、 `ReadOnly`、 `Immutable`、 `WriteOnly`。</span><span class="sxs-lookup"><span data-stu-id="ce6fc-132">Possible values are:  `ReadWrite`, `ReadOnly`, `Immutable`, `WriteOnly`.</span></span> <span data-ttu-id="ce6fc-133">既定値は `ReadWrite` です。</span><span class="sxs-lookup"><span data-stu-id="ce6fc-133">Default is `ReadWrite`.</span></span>|
|<span data-ttu-id="ce6fc-134">名前</span><span class="sxs-lookup"><span data-stu-id="ce6fc-134">name</span></span>           |<span data-ttu-id="ce6fc-135">String</span><span class="sxs-lookup"><span data-stu-id="ce6fc-135">String</span></span>     |<span data-ttu-id="ce6fc-136">属性の名前です。</span><span class="sxs-lookup"><span data-stu-id="ce6fc-136">Name of the attribute.</span></span> <span data-ttu-id="ce6fc-137">オブジェクト定義内で一意である必要があります。</span><span class="sxs-lookup"><span data-stu-id="ce6fc-137">Must be unique within the object definition.</span></span> <span data-ttu-id="ce6fc-138">null 許容ではありません。</span><span class="sxs-lookup"><span data-stu-id="ce6fc-138">Not nullable.</span></span>|
|<span data-ttu-id="ce6fc-139">必須</span><span class="sxs-lookup"><span data-stu-id="ce6fc-139">required</span></span>       |<span data-ttu-id="ce6fc-140">ブール型</span><span class="sxs-lookup"><span data-stu-id="ce6fc-140">Boolean</span></span>    |<span data-ttu-id="ce6fc-141">`true`属性が必要な場合です。</span><span class="sxs-lookup"><span data-stu-id="ce6fc-141">`true` if attribute is required.</span></span> <span data-ttu-id="ce6fc-142">必要な属性のいずれかが表示されない場合は、オブジェクトを作成できません。</span><span class="sxs-lookup"><span data-stu-id="ce6fc-142">Object can not be created if any of the required attributes are missing.</span></span> <span data-ttu-id="ce6fc-143">場合は、同期時に必要な属性値を持たない、既定値が適用されます。</span><span class="sxs-lookup"><span data-stu-id="ce6fc-143">If during synchronization, the required attribute has no value, the default value will be used.</span></span> <span data-ttu-id="ce6fc-144">既定値が設定されていない場合、同期はエラーを記録します。</span><span class="sxs-lookup"><span data-stu-id="ce6fc-144">If default the value was not set, synchronization will record an error.</span></span>|
|<span data-ttu-id="ce6fc-145">referencedObjects</span><span class="sxs-lookup"><span data-stu-id="ce6fc-145">referencedObjects</span></span>|[<span data-ttu-id="ce6fc-146">referencedObject</span><span class="sxs-lookup"><span data-stu-id="ce6fc-146">referencedObject</span></span>](../resources/synchronization-referencedobject.md) |<span data-ttu-id="ce6fc-147">属性の場合`reference`参照されるオブジェクトのリストを入力します。 (たとえば、、`manager`属性のリストが`User`として参照されているオブジェクト)。</span><span class="sxs-lookup"><span data-stu-id="ce6fc-147">For attributes with `reference` type, lists referenced objects (for example, the `manager` attribute would list `User` as the referenced object).</span></span>|
|<span data-ttu-id="ce6fc-148">type</span><span class="sxs-lookup"><span data-stu-id="ce6fc-148">type</span></span>           |<span data-ttu-id="ce6fc-149">String</span><span class="sxs-lookup"><span data-stu-id="ce6fc-149">String</span></span>     |<span data-ttu-id="ce6fc-150">属性の値の種類。</span><span class="sxs-lookup"><span data-stu-id="ce6fc-150">Attribute value type.</span></span> <span data-ttu-id="ce6fc-151">使用可能な値は、`String`、`Integer`、`Reference`、`Binary`、`Boolean` です。</span><span class="sxs-lookup"><span data-stu-id="ce6fc-151">Possible values are: `String`, `Integer`, `Reference`, `Binary`, `Boolean`.</span></span> <span data-ttu-id="ce6fc-152">既定値は `String` です。</span><span class="sxs-lookup"><span data-stu-id="ce6fc-152">Default is `String`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ce6fc-153">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ce6fc-153">JSON representation</span></span>

<span data-ttu-id="ce6fc-154">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="ce6fc-154">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "attributeDefinition resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
