---
title: synchronizationRule リソースの種類
description: 同期する対象のオブジェクトを含む、同期エンジンと、方向の同期の実行方法を定義するソース ディレクトリからオブジェクトをコピー先のディレクトリ内のオブジェクトと一致する方法、および属性先のディレクトリにソースから同期されている場合は変換する必要があります。
localization_priority: Normal
ms.openlocfilehash: deaf27ec46268eebe289e502bdf3b62a659cf1fb
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29517926"
---
# <a name="synchronizationrule-resource-type"></a><span data-ttu-id="0d634-103">synchronizationRule リソースの種類</span><span class="sxs-lookup"><span data-stu-id="0d634-103">synchronizationRule resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0d634-104">同期する対象のオブジェクトを含む、同期エンジンと、方向の同期の実行方法を定義するソース ディレクトリからオブジェクトをコピー先のディレクトリ内のオブジェクトと一致する方法、および属性先のディレクトリにソースから同期されている場合は変換する必要があります。</span><span class="sxs-lookup"><span data-stu-id="0d634-104">Defines how the synchronization should be performed for the synchronization engine, including which objects to synchronize and in which direction, how objects from the source directory should be matched with objects in the target directory, and how attributes should be transformed when they're synchronized from the source to the target directory.</span></span>

><span data-ttu-id="0d634-105">**注:** 同期規則では、目的のディレクトリにソース ディレクトリからの一方向の同期を定義します。</span><span class="sxs-lookup"><span data-stu-id="0d634-105">**Note:** Synchronization rules define synchronization in one direction - from the source directory to the target directory.</span></span> <span data-ttu-id="0d634-106">ソースとターゲットのディレクトリは、ルールのプロパティの一部として定義されます。</span><span class="sxs-lookup"><span data-stu-id="0d634-106">The source and target directories are defined as part of the rule properties.</span></span>

<span data-ttu-id="0d634-107">同期ルールは、[同期スキーマ](synchronization-synchronizationschema.md)の一部として更新されます。</span><span class="sxs-lookup"><span data-stu-id="0d634-107">Synchronization rules are updated as part of the [synchronization schema](synchronization-synchronizationschema.md).</span></span>

## <a name="properties"></a><span data-ttu-id="0d634-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0d634-108">Properties</span></span>

| <span data-ttu-id="0d634-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0d634-109">Property</span></span>      | <span data-ttu-id="0d634-110">型</span><span class="sxs-lookup"><span data-stu-id="0d634-110">Type</span></span>      | <span data-ttu-id="0d634-111">説明</span><span class="sxs-lookup"><span data-stu-id="0d634-111">Description</span></span>    |
|:--------------|:----------|:---------------|
|<span data-ttu-id="0d634-112">Editable</span><span class="sxs-lookup"><span data-stu-id="0d634-112">editable</span></span>       |<span data-ttu-id="0d634-113">ブール値</span><span class="sxs-lookup"><span data-stu-id="0d634-113">Boolean</span></span>    |<span data-ttu-id="0d634-114">`true`場合は同期ルールをカスタマイズすることができます。`false`場合は、これは読み取り専用で、変更してはなりません。</span><span class="sxs-lookup"><span data-stu-id="0d634-114">`true` if the synchronization rule can be customized; `false` if this rule is read-only and should not be changed.</span></span>|
|<span data-ttu-id="0d634-115">id</span><span class="sxs-lookup"><span data-stu-id="0d634-115">id</span></span>             |<span data-ttu-id="0d634-116">String</span><span class="sxs-lookup"><span data-stu-id="0d634-116">String</span></span>     |<span data-ttu-id="0d634-117">同期規則の識別子です。</span><span class="sxs-lookup"><span data-stu-id="0d634-117">Synchronization rule identifier.</span></span> <span data-ttu-id="0d634-118">同期エンジンによって認識される識別子の 1 つである必要があります。</span><span class="sxs-lookup"><span data-stu-id="0d634-118">Must be one of the identifiers recognized by the synchronization engine.</span></span> <span data-ttu-id="0d634-119">ルールの識別子を参照して、API によって返される同期テンプレートをサポートします。</span><span class="sxs-lookup"><span data-stu-id="0d634-119">Supported rule identifiers can be found in the synchronization template returned by the API.</span></span>|
|<span data-ttu-id="0d634-120">metadata</span><span class="sxs-lookup"><span data-stu-id="0d634-120">metadata</span></span>       |<span data-ttu-id="0d634-121">[stringKeyStringValuePair](synchronization-stringkeystringvaluepair.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="0d634-121">[stringKeyStringValuePair](synchronization-stringkeystringvaluepair.md) collection</span></span> |<span data-ttu-id="0d634-122">プロパティをさらに拡張します。</span><span class="sxs-lookup"><span data-stu-id="0d634-122">Additional extension properties.</span></span> <span data-ttu-id="0d634-123">サポート チームによって明示的に指示しない限り、メタデータの値を変更できませんする必要があります。</span><span class="sxs-lookup"><span data-stu-id="0d634-123">Unless instructed explicitly by the support team, metadata values should not be changed.</span></span>|
|<span data-ttu-id="0d634-124">name</span><span class="sxs-lookup"><span data-stu-id="0d634-124">name</span></span>           |<span data-ttu-id="0d634-125">String</span><span class="sxs-lookup"><span data-stu-id="0d634-125">String</span></span>     |<span data-ttu-id="0d634-126">同期規則の名前を人間が判読できます。</span><span class="sxs-lookup"><span data-stu-id="0d634-126">Human-readable name of the synchronization rule.</span></span> <span data-ttu-id="0d634-127">null 許容ではありません。</span><span class="sxs-lookup"><span data-stu-id="0d634-127">Not nullable.</span></span>|
|<span data-ttu-id="0d634-128">objectMappings</span><span class="sxs-lookup"><span data-stu-id="0d634-128">objectMappings</span></span> |<span data-ttu-id="0d634-129">[objectMapping](synchronization-objectmapping.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="0d634-129">[objectMapping](synchronization-objectmapping.md) collection</span></span>    |<span data-ttu-id="0d634-130">ルールでサポートされているオブジェクトのマッピングのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="0d634-130">Collection of object mappings supported by the rule.</span></span> <span data-ttu-id="0d634-131">どのオブジェクトを同期する必要があります同期エンジンに指示します。</span><span class="sxs-lookup"><span data-stu-id="0d634-131">Tells the synchronization engine which objects should be synchronized.</span></span>|
|<span data-ttu-id="0d634-132">priority</span><span class="sxs-lookup"><span data-stu-id="0d634-132">priority</span></span>       |<span data-ttu-id="0d634-133">整数</span><span class="sxs-lookup"><span data-stu-id="0d634-133">Integer</span></span>    |<span data-ttu-id="0d634-134">[SynchronizationSchema](synchronization-synchronizationschema.md)でその他の規則を基準に優先順位です。</span><span class="sxs-lookup"><span data-stu-id="0d634-134">Priority relative to other rules in the [synchronizationSchema](synchronization-synchronizationschema.md).</span></span> <span data-ttu-id="0d634-135">優先度番号が最も小さいルールが最初に処理されます。</span><span class="sxs-lookup"><span data-stu-id="0d634-135">Rules with the lowest priority number will be processed first.</span></span>|
|<span data-ttu-id="0d634-136">sourceDirectoryName</span><span class="sxs-lookup"><span data-stu-id="0d634-136">sourceDirectoryName</span></span>       |<span data-ttu-id="0d634-137">String</span><span class="sxs-lookup"><span data-stu-id="0d634-137">String</span></span>    |<span data-ttu-id="0d634-138">ソース ディレクトリの名前です。</span><span class="sxs-lookup"><span data-stu-id="0d634-138">Name of the source directory.</span></span> <span data-ttu-id="0d634-139">[SynchronizationSchema](synchronization-synchronizationschema.md)でディレクトリの定義のいずれかに一致する必要があります。</span><span class="sxs-lookup"><span data-stu-id="0d634-139">Must match one of the directory definitions in [synchronizationSchema](synchronization-synchronizationschema.md).</span></span>|
|<span data-ttu-id="0d634-140">targetDirectoryName</span><span class="sxs-lookup"><span data-stu-id="0d634-140">targetDirectoryName</span></span>       |<span data-ttu-id="0d634-141">String</span><span class="sxs-lookup"><span data-stu-id="0d634-141">String</span></span>    |<span data-ttu-id="0d634-142">コピー先のディレクトリの名前です。</span><span class="sxs-lookup"><span data-stu-id="0d634-142">Name of the target directory.</span></span> <span data-ttu-id="0d634-143">[SynchronizationSchema](synchronization-synchronizationschema.md)でディレクトリの定義のいずれかに一致する必要があります。</span><span class="sxs-lookup"><span data-stu-id="0d634-143">Must match one of the directory definitions in [synchronizationSchema](synchronization-synchronizationschema.md).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0d634-144">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0d634-144">JSON representation</span></span>

<span data-ttu-id="0d634-145">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="0d634-145">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-synchronizationrule.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
