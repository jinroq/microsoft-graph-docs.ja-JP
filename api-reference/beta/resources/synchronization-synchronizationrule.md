---
title: 同期規則リソースの種類
description: 同期エンジンに対して同期を実行する方法を定義します。どのオブジェクトを同期するか、どの方向に、どのようにソースディレクトリのオブジェクトをターゲットディレクトリのオブジェクトと照合するか、どのように属性を使用するかを指定します。ソースとターゲットディレクトリの同期時に変換する必要があります。
localization_priority: Normal
ms.openlocfilehash: b881c73d8fec8dc6b342192195d486807c744cf7
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33340027"
---
# <a name="synchronizationrule-resource-type"></a><span data-ttu-id="daee0-103">同期規則リソースの種類</span><span class="sxs-lookup"><span data-stu-id="daee0-103">synchronizationRule resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="daee0-104">同期エンジンに対して同期を実行する方法を定義します。どのオブジェクトを同期するか、どの方向に、どのようにソースディレクトリのオブジェクトをターゲットディレクトリのオブジェクトと照合するか、どのように属性を使用するかを指定します。ソースとターゲットディレクトリの同期時に変換する必要があります。</span><span class="sxs-lookup"><span data-stu-id="daee0-104">Defines how the synchronization should be performed for the synchronization engine, including which objects to synchronize and in which direction, how objects from the source directory should be matched with objects in the target directory, and how attributes should be transformed when they're synchronized from the source to the target directory.</span></span>

><span data-ttu-id="daee0-105">**注:** 同期ルールは、ソースディレクトリからターゲットディレクトリへの一方向での同期を定義します。</span><span class="sxs-lookup"><span data-stu-id="daee0-105">**Note:** Synchronization rules define synchronization in one direction - from the source directory to the target directory.</span></span> <span data-ttu-id="daee0-106">ソースディレクトリとターゲットディレクトリは、ルールのプロパティの一部として定義されます。</span><span class="sxs-lookup"><span data-stu-id="daee0-106">The source and target directories are defined as part of the rule properties.</span></span>

<span data-ttu-id="daee0-107">同期ルールは、[同期スキーマ](synchronization-synchronizationschema.md)の一部として更新されます。</span><span class="sxs-lookup"><span data-stu-id="daee0-107">Synchronization rules are updated as part of the [synchronization schema](synchronization-synchronizationschema.md).</span></span>

## <a name="properties"></a><span data-ttu-id="daee0-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="daee0-108">Properties</span></span>

| <span data-ttu-id="daee0-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="daee0-109">Property</span></span>      | <span data-ttu-id="daee0-110">型</span><span class="sxs-lookup"><span data-stu-id="daee0-110">Type</span></span>      | <span data-ttu-id="daee0-111">説明</span><span class="sxs-lookup"><span data-stu-id="daee0-111">Description</span></span>    |
|:--------------|:----------|:---------------|
|<span data-ttu-id="daee0-112">可能</span><span class="sxs-lookup"><span data-stu-id="daee0-112">editable</span></span>       |<span data-ttu-id="daee0-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="daee0-113">Boolean</span></span>    |<span data-ttu-id="daee0-114">`true`同期ルールをカスタマイズできる場合は、`false`このルールは読み取り専用であり、変更する必要はありません。</span><span class="sxs-lookup"><span data-stu-id="daee0-114">`true` if the synchronization rule can be customized; `false` if this rule is read-only and should not be changed.</span></span>|
|<span data-ttu-id="daee0-115">id</span><span class="sxs-lookup"><span data-stu-id="daee0-115">id</span></span>             |<span data-ttu-id="daee0-116">String</span><span class="sxs-lookup"><span data-stu-id="daee0-116">String</span></span>     |<span data-ttu-id="daee0-117">同期ルール識別子。</span><span class="sxs-lookup"><span data-stu-id="daee0-117">Synchronization rule identifier.</span></span> <span data-ttu-id="daee0-118">同期エンジンで認識される識別子のいずれかである必要があります。</span><span class="sxs-lookup"><span data-stu-id="daee0-118">Must be one of the identifiers recognized by the synchronization engine.</span></span> <span data-ttu-id="daee0-119">サポートされているルール識別子は、API によって返される同期テンプレートにあります。</span><span class="sxs-lookup"><span data-stu-id="daee0-119">Supported rule identifiers can be found in the synchronization template returned by the API.</span></span>|
|<span data-ttu-id="daee0-120">metadata</span><span class="sxs-lookup"><span data-stu-id="daee0-120">metadata</span></span>       |<span data-ttu-id="daee0-121">[stringkeystringvaluepair](synchronization-stringkeystringvaluepair.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="daee0-121">[stringKeyStringValuePair](synchronization-stringkeystringvaluepair.md) collection</span></span> |<span data-ttu-id="daee0-122">追加の拡張機能のプロパティ。</span><span class="sxs-lookup"><span data-stu-id="daee0-122">Additional extension properties.</span></span> <span data-ttu-id="daee0-123">サポートチームによって明示的に指示されていない限り、メタデータ値は変更しないでください。</span><span class="sxs-lookup"><span data-stu-id="daee0-123">Unless instructed explicitly by the support team, metadata values should not be changed.</span></span>|
|<span data-ttu-id="daee0-124">name</span><span class="sxs-lookup"><span data-stu-id="daee0-124">name</span></span>           |<span data-ttu-id="daee0-125">String</span><span class="sxs-lookup"><span data-stu-id="daee0-125">String</span></span>     |<span data-ttu-id="daee0-126">ユーザーが読み取ることができる同期ルールの名前。</span><span class="sxs-lookup"><span data-stu-id="daee0-126">Human-readable name of the synchronization rule.</span></span> <span data-ttu-id="daee0-127">null 許容型ではありません。</span><span class="sxs-lookup"><span data-stu-id="daee0-127">Not nullable.</span></span>|
|<span data-ttu-id="daee0-128">objectmappings</span><span class="sxs-lookup"><span data-stu-id="daee0-128">objectMappings</span></span> |<span data-ttu-id="daee0-129">[objectmapping](synchronization-objectmapping.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="daee0-129">[objectMapping](synchronization-objectmapping.md) collection</span></span>    |<span data-ttu-id="daee0-130">ルールでサポートされているオブジェクトマッピングのコレクション。</span><span class="sxs-lookup"><span data-stu-id="daee0-130">Collection of object mappings supported by the rule.</span></span> <span data-ttu-id="daee0-131">同期するオブジェクトを同期エンジンに通知します。</span><span class="sxs-lookup"><span data-stu-id="daee0-131">Tells the synchronization engine which objects should be synchronized.</span></span>|
|<span data-ttu-id="daee0-132">priority</span><span class="sxs-lookup"><span data-stu-id="daee0-132">priority</span></span>       |<span data-ttu-id="daee0-133">整数</span><span class="sxs-lookup"><span data-stu-id="daee0-133">Integer</span></span>    |<span data-ttu-id="daee0-134">[同期スキーマ](synchronization-synchronizationschema.md)内の他のルールに対する優先度。</span><span class="sxs-lookup"><span data-stu-id="daee0-134">Priority relative to other rules in the [synchronizationSchema](synchronization-synchronizationschema.md).</span></span> <span data-ttu-id="daee0-135">優先度が最も低いルールが最初に処理されます。</span><span class="sxs-lookup"><span data-stu-id="daee0-135">Rules with the lowest priority number will be processed first.</span></span>|
|<span data-ttu-id="daee0-136">sourceDirectoryName</span><span class="sxs-lookup"><span data-stu-id="daee0-136">sourceDirectoryName</span></span>       |<span data-ttu-id="daee0-137">String</span><span class="sxs-lookup"><span data-stu-id="daee0-137">String</span></span>    |<span data-ttu-id="daee0-138">ソースディレクトリの名前。</span><span class="sxs-lookup"><span data-stu-id="daee0-138">Name of the source directory.</span></span> <span data-ttu-id="daee0-139">は、[同期スキーマ](synchronization-synchronizationschema.md)のディレクトリ定義のいずれかと一致している必要があります。</span><span class="sxs-lookup"><span data-stu-id="daee0-139">Must match one of the directory definitions in [synchronizationSchema](synchronization-synchronizationschema.md).</span></span>|
|<span data-ttu-id="daee0-140">targetDirectoryName</span><span class="sxs-lookup"><span data-stu-id="daee0-140">targetDirectoryName</span></span>       |<span data-ttu-id="daee0-141">String</span><span class="sxs-lookup"><span data-stu-id="daee0-141">String</span></span>    |<span data-ttu-id="daee0-142">ターゲットディレクトリの名前。</span><span class="sxs-lookup"><span data-stu-id="daee0-142">Name of the target directory.</span></span> <span data-ttu-id="daee0-143">は、[同期スキーマ](synchronization-synchronizationschema.md)のディレクトリ定義のいずれかと一致している必要があります。</span><span class="sxs-lookup"><span data-stu-id="daee0-143">Must match one of the directory definitions in [synchronizationSchema](synchronization-synchronizationschema.md).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="daee0-144">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="daee0-144">JSON representation</span></span>

<span data-ttu-id="daee0-145">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="daee0-145">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.synchronizationRule"
}-->

```json
{
  "editable": true,
  "id": "String",
  "metadata": [{"@odata.type": "microsoft.graph.stringKeyStringValuePair"}],
  "name": "String",
  "objectMappings": [{"@odata.type": "microsoft.graph.objectMapping"}],
  "priority": 1024,
  "sourceDirectoryName": "String",
  "targetDirectoryName": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "synchronizationRule resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
