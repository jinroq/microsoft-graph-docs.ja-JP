---
title: synchronizationRule リソースの種類
description: 同期する対象のオブジェクトを含む、同期エンジンと、方向の同期の実行方法を定義するソース ディレクトリからオブジェクトをコピー先のディレクトリ内のオブジェクトと一致する方法、および属性先のディレクトリにソースから同期されている場合は変換する必要があります。
ms.openlocfilehash: c860228637a6cc3ad9137851408379bd7f779c75
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27068412"
---
# <a name="synchronizationrule-resource-type"></a><span data-ttu-id="f7e7d-103">synchronizationRule リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f7e7d-103">synchronizationRule resource type</span></span>

> <span data-ttu-id="f7e7d-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="f7e7d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f7e7d-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f7e7d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f7e7d-106">同期する対象のオブジェクトを含む、同期エンジンと、方向の同期の実行方法を定義するソース ディレクトリからオブジェクトをコピー先のディレクトリ内のオブジェクトと一致する方法、および属性先のディレクトリにソースから同期されている場合は変換する必要があります。</span><span class="sxs-lookup"><span data-stu-id="f7e7d-106">Defines how the synchronization should be performed for the synchronization engine, including which objects to synchronize and in which direction, how objects from the source directory should be matched with objects in the target directory, and how attributes should be transformed when they're synchronized from the source to the target directory.</span></span>

><span data-ttu-id="f7e7d-107">**注:** 同期規則では、目的のディレクトリにソース ディレクトリからの一方向の同期を定義します。</span><span class="sxs-lookup"><span data-stu-id="f7e7d-107">**Note:** Synchronization rules define synchronization in one direction - from the source directory to the target directory.</span></span> <span data-ttu-id="f7e7d-108">ソースとターゲットのディレクトリは、ルールのプロパティの一部として定義されます。</span><span class="sxs-lookup"><span data-stu-id="f7e7d-108">The source and target directories are defined as part of the rule properties.</span></span>

<span data-ttu-id="f7e7d-109">同期ルールは、[同期スキーマ](synchronization-synchronizationschema.md)の一部として更新されます。</span><span class="sxs-lookup"><span data-stu-id="f7e7d-109">Synchronization rules are updated as part of the [synchronization schema](synchronization-synchronizationschema.md).</span></span>

## <a name="properties"></a><span data-ttu-id="f7e7d-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f7e7d-110">Properties</span></span>

| <span data-ttu-id="f7e7d-111">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f7e7d-111">Property</span></span>      | <span data-ttu-id="f7e7d-112">型</span><span class="sxs-lookup"><span data-stu-id="f7e7d-112">Type</span></span>      | <span data-ttu-id="f7e7d-113">説明</span><span class="sxs-lookup"><span data-stu-id="f7e7d-113">Description</span></span>    |
|:--------------|:----------|:---------------|
|<span data-ttu-id="f7e7d-114">編集可能です</span><span class="sxs-lookup"><span data-stu-id="f7e7d-114">editable</span></span>       |<span data-ttu-id="f7e7d-115">ブール値</span><span class="sxs-lookup"><span data-stu-id="f7e7d-115">Boolean</span></span>    |<span data-ttu-id="f7e7d-116">`true`場合は同期ルールをカスタマイズすることができます。`false`場合は、これは読み取り専用で、変更してはなりません。</span><span class="sxs-lookup"><span data-stu-id="f7e7d-116">`true` if the synchronization rule can be customized; `false` if this rule is read-only and should not be changed.</span></span>|
|<span data-ttu-id="f7e7d-117">id</span><span class="sxs-lookup"><span data-stu-id="f7e7d-117">id</span></span>             |<span data-ttu-id="f7e7d-118">String</span><span class="sxs-lookup"><span data-stu-id="f7e7d-118">String</span></span>     |<span data-ttu-id="f7e7d-119">同期規則の識別子です。</span><span class="sxs-lookup"><span data-stu-id="f7e7d-119">Synchronization rule identifier.</span></span> <span data-ttu-id="f7e7d-120">同期エンジンによって認識される識別子の 1 つである必要があります。</span><span class="sxs-lookup"><span data-stu-id="f7e7d-120">Must be one of the identifiers recognized by the synchronization engine.</span></span> <span data-ttu-id="f7e7d-121">ルールの識別子を参照して、API によって返される同期テンプレートをサポートします。</span><span class="sxs-lookup"><span data-stu-id="f7e7d-121">Supported rule identifiers can be found in the synchronization template returned by the API.</span></span>|
|<span data-ttu-id="f7e7d-122">metadata</span><span class="sxs-lookup"><span data-stu-id="f7e7d-122">metadata</span></span>       |<span data-ttu-id="f7e7d-123">[stringKeyStringValuePair](synchronization-stringkeystringvaluepair.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="f7e7d-123">[stringKeyStringValuePair](synchronization-stringkeystringvaluepair.md) collection</span></span> |<span data-ttu-id="f7e7d-124">プロパティをさらに拡張します。</span><span class="sxs-lookup"><span data-stu-id="f7e7d-124">Additional extension properties.</span></span> <span data-ttu-id="f7e7d-125">サポート チームによって明示的に指示しない限り、メタデータの値を変更できませんする必要があります。</span><span class="sxs-lookup"><span data-stu-id="f7e7d-125">Unless instructed explicitly by the support team, metadata values should not be changed.</span></span>|
|<span data-ttu-id="f7e7d-126">名前</span><span class="sxs-lookup"><span data-stu-id="f7e7d-126">name</span></span>           |<span data-ttu-id="f7e7d-127">String</span><span class="sxs-lookup"><span data-stu-id="f7e7d-127">String</span></span>     |<span data-ttu-id="f7e7d-128">同期規則の名前を人間が判読できます。</span><span class="sxs-lookup"><span data-stu-id="f7e7d-128">Human-readable name of the synchronization rule.</span></span> <span data-ttu-id="f7e7d-129">null 許容ではありません。</span><span class="sxs-lookup"><span data-stu-id="f7e7d-129">Not nullable.</span></span>|
|<span data-ttu-id="f7e7d-130">objectMappings</span><span class="sxs-lookup"><span data-stu-id="f7e7d-130">objectMappings</span></span> |<span data-ttu-id="f7e7d-131">[objectMapping](synchronization-objectmapping.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="f7e7d-131">[objectMapping](synchronization-objectmapping.md) collection</span></span>    |<span data-ttu-id="f7e7d-132">ルールでサポートされているオブジェクトのマッピングのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="f7e7d-132">Collection of object mappings supported by the rule.</span></span> <span data-ttu-id="f7e7d-133">どのオブジェクトを同期する必要があります同期エンジンに指示します。</span><span class="sxs-lookup"><span data-stu-id="f7e7d-133">Tells the synchronization engine which objects should be synchronized.</span></span>|
|<span data-ttu-id="f7e7d-134">priority</span><span class="sxs-lookup"><span data-stu-id="f7e7d-134">priority</span></span>       |<span data-ttu-id="f7e7d-135">整数</span><span class="sxs-lookup"><span data-stu-id="f7e7d-135">Integer</span></span>    |<span data-ttu-id="f7e7d-136">[SynchronizationSchema](synchronization-synchronizationschema.md)でその他の規則を基準に優先順位です。</span><span class="sxs-lookup"><span data-stu-id="f7e7d-136">Priority relative to other rules in the [synchronizationSchema](synchronization-synchronizationschema.md).</span></span> <span data-ttu-id="f7e7d-137">優先度番号が最も小さいルールが最初に処理されます。</span><span class="sxs-lookup"><span data-stu-id="f7e7d-137">Rules with the lowest priority number will be processed first.</span></span>|
|<span data-ttu-id="f7e7d-138">sourceDirectoryName</span><span class="sxs-lookup"><span data-stu-id="f7e7d-138">sourceDirectoryName</span></span>       |<span data-ttu-id="f7e7d-139">String</span><span class="sxs-lookup"><span data-stu-id="f7e7d-139">String</span></span>    |<span data-ttu-id="f7e7d-140">ソース ディレクトリの名前です。</span><span class="sxs-lookup"><span data-stu-id="f7e7d-140">Name of the source directory.</span></span> <span data-ttu-id="f7e7d-141">[SynchronizationSchema](synchronization-synchronizationschema.md)でディレクトリの定義のいずれかに一致する必要があります。</span><span class="sxs-lookup"><span data-stu-id="f7e7d-141">Must match one of the directory definitions in [synchronizationSchema](synchronization-synchronizationschema.md).</span></span>|
|<span data-ttu-id="f7e7d-142">targetDirectoryName</span><span class="sxs-lookup"><span data-stu-id="f7e7d-142">targetDirectoryName</span></span>       |<span data-ttu-id="f7e7d-143">String</span><span class="sxs-lookup"><span data-stu-id="f7e7d-143">String</span></span>    |<span data-ttu-id="f7e7d-144">コピー先のディレクトリの名前です。</span><span class="sxs-lookup"><span data-stu-id="f7e7d-144">Name of the target directory.</span></span> <span data-ttu-id="f7e7d-145">[SynchronizationSchema](synchronization-synchronizationschema.md)でディレクトリの定義のいずれかに一致する必要があります。</span><span class="sxs-lookup"><span data-stu-id="f7e7d-145">Must match one of the directory definitions in [synchronizationSchema](synchronization-synchronizationschema.md).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f7e7d-146">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f7e7d-146">JSON representation</span></span>

<span data-ttu-id="f7e7d-147">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="f7e7d-147">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "synchronizationRule resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->