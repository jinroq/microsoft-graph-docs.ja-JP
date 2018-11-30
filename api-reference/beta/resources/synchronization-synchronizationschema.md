---
title: synchronizationSchema リソースの種類
description: オブジェクトがどのようになるかを定義する同期し、同期する方法です。 同期スキーマには、特定の同期ジョブのセットアップ情報のほとんどが含まれています。 通常にするいくつかの属性のマッピングをカスタマイズするかを特定の条件を満たすオブジェクトのみを同期するスコープのフィルターを追加します。
ms.openlocfilehash: 13e57db5f78af2d3f0a8243d247fe5c3f3d5e0af
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27069795"
---
# <a name="synchronizationschema-resource-type"></a><span data-ttu-id="b156a-105">synchronizationSchema リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b156a-105">synchronizationSchema resource type</span></span>

> <span data-ttu-id="b156a-106">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="b156a-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b156a-107">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b156a-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b156a-108">オブジェクトがどのようになるかを定義する同期し、同期する方法です。</span><span class="sxs-lookup"><span data-stu-id="b156a-108">Defines what objects will be synchronized and how they will be synchronized.</span></span> <span data-ttu-id="b156a-109">同期スキーマには、特定の同期ジョブのセットアップ情報のほとんどが含まれています。</span><span class="sxs-lookup"><span data-stu-id="b156a-109">The synchronization schema contains most of the setup information for a particular synchronization job.</span></span> <span data-ttu-id="b156a-110">通常、[属性マッピング](synchronization-attributemapping.md)の一部をカスタマイズまたはを特定の条件を満たすオブジェクトのみを同期する[スコープのフィルター](synchronization-filter.md)が追加されます。</span><span class="sxs-lookup"><span data-stu-id="b156a-110">Typically, you will customize some of the [attribute mappings](synchronization-attributemapping.md), or add a [scoping filter](synchronization-filter.md) to synchronize only objects that satisfy a certain condition.</span></span>

<span data-ttu-id="b156a-111">次のセクションでは、同期スキーマの高度なコンポーネントについて説明します。</span><span class="sxs-lookup"><span data-stu-id="b156a-111">The following sections describe the high-level components of the synchronization schema.</span></span>

## <a name="directory-definitions"></a><span data-ttu-id="b156a-112">ディレクトリの定義</span><span class="sxs-lookup"><span data-stu-id="b156a-112">Directory definitions</span></span>

<span data-ttu-id="b156a-113">[ディレクトリの定義](synchronization-directorydefinition.md)では、ディレクトリとそのオブジェクトの同期エンジンに関する情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="b156a-113">[Directory definitions](synchronization-directorydefinition.md) provide the synchronization engine information about directories and their objects.</span></span> <span data-ttu-id="b156a-114">などのディレクトリの定義では、同期エンジンが指示、Azure AD ディレクトリが**ユーザー**と**グループ**、それらのオブジェクトとそれらの属性の型の属性はサポートされてをという名前のオブジェクトを持っています。</span><span class="sxs-lookup"><span data-stu-id="b156a-114">For example, the directory definition tells the synchronization engine that an Azure AD directory has objects named **user** and **group**, which attributes are supported for those objects, and the types for those attributes.</span></span> <span data-ttu-id="b156a-115">同期規則とオブジェクトのマッピングで使用する特定のオブジェクトと属性の順序でディレクトリの定義の一部として定義する必要があります。</span><span class="sxs-lookup"><span data-stu-id="b156a-115">In order for a particular object and attribute to be used in synchronization rules/object mappings, they have to be defined as part of the directory definition.</span></span>

## <a name="synchronization-rules"></a><span data-ttu-id="b156a-116">同期ルール</span><span class="sxs-lookup"><span data-stu-id="b156a-116">Synchronization rules</span></span>

<span data-ttu-id="b156a-117">[同期ルール](synchronization-synchronizationrule.md)は、同期の設定の中核です。</span><span class="sxs-lookup"><span data-stu-id="b156a-117">[Synchronization rules](synchronization-synchronizationrule.md) are the core of the synchronization setup.</span></span> <span data-ttu-id="b156a-118">同期を実行する方法、同期エンジンを定義する、どのようなオブジェクトを含む同期するか、ソース ディレクトリからオブジェクトのコピー先のディレクトリ内のオブジェクトとの照合方法と、属性がどのようにする必要がありますか目的のディレクトリにソースから同期されている場合に変換されます。</span><span class="sxs-lookup"><span data-stu-id="b156a-118">They define for the synchronization engine how the synchronization should be performed, including what objects should be synchronized, how objects from the source directory should be matched with objects in the target directory, and how attributes should be transformed when they're synchronized from the source to the target directory.</span></span> 

## <a name="object-mappings"></a><span data-ttu-id="b156a-119">オブジェクトのマッピング</span><span class="sxs-lookup"><span data-stu-id="b156a-119">Object mappings</span></span>

<span data-ttu-id="b156a-120">[オブジェクトのマッピング](synchronization-objectmapping.md)は、同期ルールの主な部分です。</span><span class="sxs-lookup"><span data-stu-id="b156a-120">[Object mappings](synchronization-objectmapping.md) are the main part of the synchronization rule.</span></span> <span data-ttu-id="b156a-121">どのように特定のオブジェクト同期する必要があるソースからターゲット ・ ディレクトリに各オブジェクトのマッピングを定義します。</span><span class="sxs-lookup"><span data-stu-id="b156a-121">Each object mapping defines how a given object should be synchronized from the source to the target directory.</span></span> <span data-ttu-id="b156a-122">マッピングがコピー先のディレクトリ内のオブジェクトのソース ディレクトリ内のオブジェクトの照合方法を定義する具体的には、どのような (ある場合) し、オブジェクトを提供するかどうか、オブジェクトの属性を変換する方法を決定するフィルターのスコープを使用する必要があります同期されているソースからコピー先のディレクトリにします。</span><span class="sxs-lookup"><span data-stu-id="b156a-122">In particular, the mapping defines how an object in the source directory should be matched with an object in the target directory, what (if any) scoping filters should be used to decide whether to provision an object, and how object attributes should be transformed when they're synchronized from the source to the target directory.</span></span>

## <a name="methods"></a><span data-ttu-id="b156a-123">メソッド</span><span class="sxs-lookup"><span data-stu-id="b156a-123">Methods</span></span>

| <span data-ttu-id="b156a-124">メソッド</span><span class="sxs-lookup"><span data-stu-id="b156a-124">Method</span></span>        | <span data-ttu-id="b156a-125">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="b156a-125">Return Type</span></span>               | <span data-ttu-id="b156a-126">説明</span><span class="sxs-lookup"><span data-stu-id="b156a-126">Description</span></span>                  |
|:--------------|:--------------------------|:-----------------------------|
|[<span data-ttu-id="b156a-127">スキーマを取得します</span><span class="sxs-lookup"><span data-stu-id="b156a-127">Get schema</span></span>](../api/synchronization-synchronizationschema-get.md)    |[<span data-ttu-id="b156a-128">synchronizationSchema</span><span class="sxs-lookup"><span data-stu-id="b156a-128">synchronizationSchema</span></span>](synchronization-synchronizationschema.md)   |<span data-ttu-id="b156a-129">**SynchronizationSchema**オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b156a-129">Read properties and relationships of the **synchronizationSchema** object.</span></span>|
|[<span data-ttu-id="b156a-130">スキーマを更新します。</span><span class="sxs-lookup"><span data-stu-id="b156a-130">Update schema</span></span>](../api/synchronization-synchronizationschema-update.md)    |<span data-ttu-id="b156a-131">なし</span><span class="sxs-lookup"><span data-stu-id="b156a-131">None</span></span>   |<span data-ttu-id="b156a-132">同期スキーマを更新します。</span><span class="sxs-lookup"><span data-stu-id="b156a-132">Update the synchronization schema.</span></span> |
|[<span data-ttu-id="b156a-133">スキーマを削除します。</span><span class="sxs-lookup"><span data-stu-id="b156a-133">Delete schema</span></span>](../api/synchronization-synchronizationschema-delete.md)    |<span data-ttu-id="b156a-134">なし</span><span class="sxs-lookup"><span data-stu-id="b156a-134">None</span></span>   |<span data-ttu-id="b156a-135">スキーマを既定の構成にリセットする、カスタマイズされたスキーマを削除します。</span><span class="sxs-lookup"><span data-stu-id="b156a-135">Delete the customized schema, resetting the schema to the default configuration.</span></span> |
|[<span data-ttu-id="b156a-136">リスト フィルターの演算子</span><span class="sxs-lookup"><span data-stu-id="b156a-136">List filter operators</span></span>](../api/synchronization-synchronizationschema-filteroperators.md)    |<span data-ttu-id="b156a-137">[filterOperatorSchema](../resources/synchronization-filteroperatorschema.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="b156a-137">[filterOperatorSchema](../resources/synchronization-filteroperatorschema.md) colection</span></span>   |<span data-ttu-id="b156a-138">スコープ フィルターでサポートされているすべての演算子の一覧を表示します。</span><span class="sxs-lookup"><span data-stu-id="b156a-138">List all operators supported in the scoping filters.</span></span> |
|[<span data-ttu-id="b156a-139">リストの属性が関数のマッピング</span><span class="sxs-lookup"><span data-stu-id="b156a-139">List attribute mapping functions</span></span>](../api/synchronization-synchronizationschema-functions.md)    |<span data-ttu-id="b156a-140">[attributeMappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="b156a-140">[attributeMappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md) collection</span></span>   |<span data-ttu-id="b156a-141">属性マッピングの式でサポートされているすべての関数の一覧を表示します。</span><span class="sxs-lookup"><span data-stu-id="b156a-141">List all functions supported in the attribute mapping expressions.</span></span> |
|[<span data-ttu-id="b156a-142">属性マッピングの式を解析します。</span><span class="sxs-lookup"><span data-stu-id="b156a-142">Parse attribute mapping expression</span></span>](../api/synchronization-synchronizationschema-parseexpression.md)|[<span data-ttu-id="b156a-143">parseExpressionResponse</span><span class="sxs-lookup"><span data-stu-id="b156a-143">parseExpressionResponse</span></span>](synchronization-parseexpressionresponse.md)|<span data-ttu-id="b156a-144">[AttributeMappingSource に文字列を解析します。</span><span class="sxs-lookup"><span data-stu-id="b156a-144">Parse a string expression into an [attributeMappingSource</span></span>|<span data-ttu-id="b156a-145">(../resources/synchronization_attributemappingsource.md) オブジェクト。</span><span class="sxs-lookup"><span data-stu-id="b156a-145">(../resources/synchronization_attributemappingsource.md) object.</span></span>|


## <a name="properties"></a><span data-ttu-id="b156a-146">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b156a-146">Properties</span></span>

| <span data-ttu-id="b156a-147">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b156a-147">Property</span></span>      | <span data-ttu-id="b156a-148">型</span><span class="sxs-lookup"><span data-stu-id="b156a-148">Type</span></span>      | <span data-ttu-id="b156a-149">説明</span><span class="sxs-lookup"><span data-stu-id="b156a-149">Description</span></span>    |
|:--------------|:----------|:---------------|
|<span data-ttu-id="b156a-150">directories</span><span class="sxs-lookup"><span data-stu-id="b156a-150">directories</span></span>            |<span data-ttu-id="b156a-151">[directoryDefinition](synchronization-directorydefinition.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="b156a-151">[directoryDefinition](synchronization-directorydefinition.md) collection</span></span>   |<span data-ttu-id="b156a-152">ディレクトリおよび[synchronizationJob](synchronization-synchronizationjob.md)または[synchronizationTemplate](synchronization-synchronizationtemplate.md)の一部であるオブジェクトについて説明します。</span><span class="sxs-lookup"><span data-stu-id="b156a-152">Describes directories and objects that are part of the [synchronizationJob](synchronization-synchronizationjob.md) or [synchronizationTemplate](synchronization-synchronizationtemplate.md).</span></span> |
|<span data-ttu-id="b156a-153">synchronizationRules</span><span class="sxs-lookup"><span data-stu-id="b156a-153">synchronizationRules</span></span>   |<span data-ttu-id="b156a-154">[synchronizationRule](synchronization-synchronizationrule.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="b156a-154">[synchronizationRule](synchronization-synchronizationrule.md) collection</span></span>   |<span data-ttu-id="b156a-155">[SynchronizationJob](synchronization-synchronizationjob.md)または[synchronizationTemplate](synchronization-synchronizationtemplate.md)、用に構成された同期規則のコレクション</span><span class="sxs-lookup"><span data-stu-id="b156a-155">A collection of synchronization rules configured for the [synchronizationJob](synchronization-synchronizationjob.md) or [synchronizationTemplate](synchronization-synchronizationtemplate.md),</span></span> |
|<span data-ttu-id="b156a-156">version</span><span class="sxs-lookup"><span data-stu-id="b156a-156">version</span></span>                |<span data-ttu-id="b156a-157">String</span><span class="sxs-lookup"><span data-stu-id="b156a-157">String</span></span>                             |<span data-ttu-id="b156a-158">スキーマ変更のたびに自動的に更新、スキーマのバージョン。</span><span class="sxs-lookup"><span data-stu-id="b156a-158">The version of the schema, updated automatically with every schema change.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="b156a-159">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b156a-159">JSON representation</span></span>

<span data-ttu-id="b156a-160">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="b156a-160">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.synchronizationSchema"
}-->

```json
{
  "directories": [{"@odata.type": "microsoft.graph.directoryDefinition"}],
  "provisioningTaskIdentifier": "String (identifier)",
  "synchronizationRules": [{"@odata.type": "microsoft.graph.synchronizationRule"}],
  "version": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "synchronizationSchema resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->