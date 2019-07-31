---
title: directoryDefinition リソースの種類
description: ディレクトリとそのオブジェクトに関する同期エンジン情報を提供します。
localization_priority: Normal
doc_type: resourcePageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 0858c714fab3fbfb862119d5ece1af2650888391
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964810"
---
# <a name="directorydefinition-resource-type"></a><span data-ttu-id="38cfa-103">directoryDefinition リソースの種類</span><span class="sxs-lookup"><span data-stu-id="38cfa-103">directoryDefinition resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="38cfa-104">ディレクトリとそのオブジェクトに関する同期エンジン情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="38cfa-104">Provides the synchronization engine information about a directory and its objects.</span></span> <span data-ttu-id="38cfa-105">このリソースは、同期エンジンに対して、たとえば、ディレクトリには、**ユーザー**と**グループ**という名前のオブジェクト、これらのオブジェクトに対してサポートされている属性、およびそれらの属性の種類を示します。</span><span class="sxs-lookup"><span data-stu-id="38cfa-105">This resource tells the synchronization engine, for example, that the directory has objects named **user** and **group**, which attributes are supported for those objects, and the types for those attributes.</span></span> <span data-ttu-id="38cfa-106">オブジェクトと属性を[同期ルール](synchronization-synchronizationrule.md)および[オブジェクトマッピング](synchronization-objectmapping.md)に参加させるには、それらをディレクトリ定義の一部として定義する必要があります。</span><span class="sxs-lookup"><span data-stu-id="38cfa-106">In order for the object and attribute to participate in [synchronization rules](synchronization-synchronizationrule.md) and [object mappings](synchronization-objectmapping.md), they must be defined as part of the directory definition.</span></span>

<span data-ttu-id="38cfa-107">通常、[同期テンプレート](synchronization-synchronizationtemplate.md)の一部として提供される既定の[同期スキーマ](synchronization-synchronizationschema.md)は、そのディレクトリに最もよく使用されるオブジェクトと属性を定義します。</span><span class="sxs-lookup"><span data-stu-id="38cfa-107">In general, the default [synchronization schema](synchronization-synchronizationschema.md) provided as part of the [synchronization template](synchronization-synchronizationtemplate.md) will define most commonly used objects and attributes for that directory.</span></span> <span data-ttu-id="38cfa-108">ただし、ディレクトリでカスタム属性の追加がサポートされている場合は、独自のカスタムオブジェクトまたは属性を使用して、既定の定義を拡張することもできます。</span><span class="sxs-lookup"><span data-stu-id="38cfa-108">However, if the directory supports the addition of custom attributes, you might want to expand the default definition with your own custom objects or attributes.</span></span> <span data-ttu-id="38cfa-109">詳細については、「[カスタム属性を使用して同期を構成する](synchronization-configure-with-custom-target-attributes.md)」および「 [configure synchronization with directory extension attributes](synchronization-configure-with-directory-extension-attributes.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="38cfa-109">For more information, see [Configure synchronization with custom attributes](synchronization-configure-with-custom-target-attributes.md) and [Configure synchronization with directory extension attributes](synchronization-configure-with-directory-extension-attributes.md).</span></span>

<span data-ttu-id="38cfa-110">ディレクトリ定義は、[同期スキーマ](synchronization-synchronizationschema.md)の一部として更新されます。</span><span class="sxs-lookup"><span data-stu-id="38cfa-110">Directory definitions are updated as part of the [synchronization schema](synchronization-synchronizationschema.md).</span></span>

## <a name="methods"></a><span data-ttu-id="38cfa-111">メソッド</span><span class="sxs-lookup"><span data-stu-id="38cfa-111">Methods</span></span>

| <span data-ttu-id="38cfa-112">メソッド</span><span class="sxs-lookup"><span data-stu-id="38cfa-112">Method</span></span>       | <span data-ttu-id="38cfa-113">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="38cfa-113">Return Type</span></span>  |<span data-ttu-id="38cfa-114">説明</span><span class="sxs-lookup"><span data-stu-id="38cfa-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="38cfa-115">Discover directoryDefinition</span><span class="sxs-lookup"><span data-stu-id="38cfa-115">Discover directoryDefinition</span></span>](../api/directorydefinition-discover.md) | [<span data-ttu-id="38cfa-116">directoryDefinition</span><span class="sxs-lookup"><span data-stu-id="38cfa-116">directoryDefinition</span></span>](synchronization-directorydefinition.md) |<span data-ttu-id="38cfa-117">ディレクトリのスキーマとサポートされているプロパティを検出します。</span><span class="sxs-lookup"><span data-stu-id="38cfa-117">Discover the schema and supported properties of the directory.</span></span>|

## <a name="properties"></a><span data-ttu-id="38cfa-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="38cfa-118">Properties</span></span>

| <span data-ttu-id="38cfa-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="38cfa-119">Property</span></span>      | <span data-ttu-id="38cfa-120">型</span><span class="sxs-lookup"><span data-stu-id="38cfa-120">Type</span></span>      | <span data-ttu-id="38cfa-121">説明</span><span class="sxs-lookup"><span data-stu-id="38cfa-121">Description</span></span>    |
|:--------------|:----------|:---------------|
|<span data-ttu-id="38cfa-122">id</span><span class="sxs-lookup"><span data-stu-id="38cfa-122">id</span></span>           |<span data-ttu-id="38cfa-123">文字列</span><span class="sxs-lookup"><span data-stu-id="38cfa-123">String</span></span>     |<span data-ttu-id="38cfa-124">ディレクトリ識別子。</span><span class="sxs-lookup"><span data-stu-id="38cfa-124">Directory identifier.</span></span> <span data-ttu-id="38cfa-125">null 許容ではありません。</span><span class="sxs-lookup"><span data-stu-id="38cfa-125">Not nullable.</span></span>|
|<span data-ttu-id="38cfa-126">metadata</span><span class="sxs-lookup"><span data-stu-id="38cfa-126">metadata</span></span>       |<span data-ttu-id="38cfa-127">metadataEntry コレクション</span><span class="sxs-lookup"><span data-stu-id="38cfa-127">metadataEntry collection</span></span>    |<span data-ttu-id="38cfa-128">追加の拡張機能のプロパティ。</span><span class="sxs-lookup"><span data-stu-id="38cfa-128">Additional extension properties.</span></span> <span data-ttu-id="38cfa-129">明示的に記述されていない限り、メタデータ値は変更しないでください。</span><span class="sxs-lookup"><span data-stu-id="38cfa-129">Unless mentioned explicitly, metadata values should not be changed.</span></span>|
|<span data-ttu-id="38cfa-130">name</span><span class="sxs-lookup"><span data-stu-id="38cfa-130">name</span></span>           |<span data-ttu-id="38cfa-131">String</span><span class="sxs-lookup"><span data-stu-id="38cfa-131">String</span></span>     |<span data-ttu-id="38cfa-132">ディレクトリの名前。</span><span class="sxs-lookup"><span data-stu-id="38cfa-132">Name of the directory.</span></span> <span data-ttu-id="38cfa-133">[同期スキーマ](synchronization-synchronizationschema.md)内で一意である必要があります。</span><span class="sxs-lookup"><span data-stu-id="38cfa-133">Must be unique within the [synchronization schema](synchronization-synchronizationschema.md).</span></span> <span data-ttu-id="38cfa-134">null 許容ではありません。</span><span class="sxs-lookup"><span data-stu-id="38cfa-134">Not nullable.</span></span>|
|<span data-ttu-id="38cfa-135">対象</span><span class="sxs-lookup"><span data-stu-id="38cfa-135">objects</span></span>        |<span data-ttu-id="38cfa-136">[Objectdefinition](synchronization-objectdefinition.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="38cfa-136">[objectDefinition](synchronization-objectdefinition.md) collection</span></span>    |<span data-ttu-id="38cfa-137">ディレクトリでサポートされているオブジェクトのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="38cfa-137">Collection of objects supported by the directory.</span></span>|
|<span data-ttu-id="38cfa-138">version</span><span class="sxs-lookup"><span data-stu-id="38cfa-138">version</span></span>|<span data-ttu-id="38cfa-139">String</span><span class="sxs-lookup"><span data-stu-id="38cfa-139">String</span></span>|<span data-ttu-id="38cfa-140">検出されたバージョンを示す値を取得します。</span><span class="sxs-lookup"><span data-stu-id="38cfa-140">Read only value that indicates version discovered.</span></span> <span data-ttu-id="38cfa-141">検出がまだ行われていない場合は、Null。</span><span class="sxs-lookup"><span data-stu-id="38cfa-141">Null if discovery has not yet occurred.</span></span>|
|<span data-ttu-id="38cfa-142">discoveryDateTime</span><span class="sxs-lookup"><span data-stu-id="38cfa-142">discoveryDateTime</span></span>|<span data-ttu-id="38cfa-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="38cfa-143">DateTimeOffset</span></span>| <span data-ttu-id="38cfa-144">は、ISO 8601 形式を使用した検出日時を表し、常に UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="38cfa-144">Represents the discovery date and time using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="38cfa-145">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="38cfa-145">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="38cfa-146">discoverabilities</span><span class="sxs-lookup"><span data-stu-id="38cfa-146">discoverabilities</span></span>|<span data-ttu-id="38cfa-147">string</span><span class="sxs-lookup"><span data-stu-id="38cfa-147">string</span></span>| <span data-ttu-id="38cfa-148">アプリでサポートされている検出の種類を示す値の読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="38cfa-148">Read only value indicating what type of discovery the app supports.</span></span> <span data-ttu-id="38cfa-149">使用可能な値: `AttributeDataTypes`、`AttributeNames`、`AttributeReadOnly`、`None`、`ReferenceAttributes`、`UnknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="38cfa-149">Possible values are: `AttributeDataTypes`, `AttributeNames`, `AttributeReadOnly`, `None`, `ReferenceAttributes`, `UnknownFutureValue`.</span></span>| 

## <a name="json-representation"></a><span data-ttu-id="38cfa-150">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="38cfa-150">JSON representation</span></span>

<span data-ttu-id="38cfa-151">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="38cfa-151">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.directoryDefinition"
}-->

```json
{
  "discoverabilities": "String",
  "discoveryDateTime": "DateTimeOffset",
  "id": "String",
  "metadata": [{"@odata.type": "microsoft.graph.stringKeyStringValuePair"}],
  "name": "String",
  "objects": [{"@odata.type": "microsoft.graph.objectDefinition"}],
  "version": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "directoryDefinition resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
