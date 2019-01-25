---
title: synchronizationSchema リソースの種類
description: オブジェクトがどのようになるかを定義する同期し、同期する方法です。 同期スキーマには、特定の同期ジョブのセットアップ情報のほとんどが含まれています。 通常にするいくつかの属性のマッピングをカスタマイズするかを特定の条件を満たすオブジェクトのみを同期するスコープのフィルターを追加します。
localization_priority: Normal
ms.openlocfilehash: e7bb91ef473a04552c4c5f33ffc9d54eb86a9b7a
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515931"
---
# <a name="synchronizationschema-resource-type"></a><span data-ttu-id="ab3bc-105">synchronizationSchema リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ab3bc-105">synchronizationSchema resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ab3bc-106">オブジェクトがどのようになるかを定義する同期し、同期する方法です。</span><span class="sxs-lookup"><span data-stu-id="ab3bc-106">Defines what objects will be synchronized and how they will be synchronized.</span></span> <span data-ttu-id="ab3bc-107">同期スキーマには、特定の同期ジョブのセットアップ情報のほとんどが含まれています。</span><span class="sxs-lookup"><span data-stu-id="ab3bc-107">The synchronization schema contains most of the setup information for a particular synchronization job.</span></span> <span data-ttu-id="ab3bc-108">通常、[属性マッピング](synchronization-attributemapping.md)の一部をカスタマイズまたはを特定の条件を満たすオブジェクトのみを同期する[スコープのフィルター](synchronization-filter.md)が追加されます。</span><span class="sxs-lookup"><span data-stu-id="ab3bc-108">Typically, you will customize some of the [attribute mappings](synchronization-attributemapping.md), or add a [scoping filter](synchronization-filter.md) to synchronize only objects that satisfy a certain condition.</span></span>

<span data-ttu-id="ab3bc-109">次のセクションでは、同期スキーマの高度なコンポーネントについて説明します。</span><span class="sxs-lookup"><span data-stu-id="ab3bc-109">The following sections describe the high-level components of the synchronization schema.</span></span>

## <a name="directory-definitions"></a><span data-ttu-id="ab3bc-110">ディレクトリの定義</span><span class="sxs-lookup"><span data-stu-id="ab3bc-110">Directory definitions</span></span>

<span data-ttu-id="ab3bc-111">[ディレクトリの定義](synchronization-directorydefinition.md)では、ディレクトリとそのオブジェクトの同期エンジンに関する情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="ab3bc-111">[Directory definitions](synchronization-directorydefinition.md) provide the synchronization engine information about directories and their objects.</span></span> <span data-ttu-id="ab3bc-112">などのディレクトリの定義では、同期エンジンが指示、Azure AD ディレクトリが**ユーザー**と**グループ**、それらのオブジェクトとそれらの属性の型の属性はサポートされてをという名前のオブジェクトを持っています。</span><span class="sxs-lookup"><span data-stu-id="ab3bc-112">For example, the directory definition tells the synchronization engine that an Azure AD directory has objects named **user** and **group**, which attributes are supported for those objects, and the types for those attributes.</span></span> <span data-ttu-id="ab3bc-113">同期規則とオブジェクトのマッピングで使用する特定のオブジェクトと属性の順序でディレクトリの定義の一部として定義する必要があります。</span><span class="sxs-lookup"><span data-stu-id="ab3bc-113">In order for a particular object and attribute to be used in synchronization rules/object mappings, they have to be defined as part of the directory definition.</span></span>

## <a name="synchronization-rules"></a><span data-ttu-id="ab3bc-114">同期ルール</span><span class="sxs-lookup"><span data-stu-id="ab3bc-114">Synchronization rules</span></span>

<span data-ttu-id="ab3bc-115">[同期ルール](synchronization-synchronizationrule.md)は、同期の設定の中核です。</span><span class="sxs-lookup"><span data-stu-id="ab3bc-115">[Synchronization rules](synchronization-synchronizationrule.md) are the core of the synchronization setup.</span></span> <span data-ttu-id="ab3bc-116">同期を実行する方法、同期エンジンを定義する、どのようなオブジェクトを含む同期するか、ソース ディレクトリからオブジェクトのコピー先のディレクトリ内のオブジェクトとの照合方法と、属性がどのようにする必要がありますか目的のディレクトリにソースから同期されている場合に変換されます。</span><span class="sxs-lookup"><span data-stu-id="ab3bc-116">They define for the synchronization engine how the synchronization should be performed, including what objects should be synchronized, how objects from the source directory should be matched with objects in the target directory, and how attributes should be transformed when they're synchronized from the source to the target directory.</span></span> 

## <a name="object-mappings"></a><span data-ttu-id="ab3bc-117">オブジェクトのマッピング</span><span class="sxs-lookup"><span data-stu-id="ab3bc-117">Object mappings</span></span>

<span data-ttu-id="ab3bc-118">[オブジェクトのマッピング](synchronization-objectmapping.md)は、同期ルールの主な部分です。</span><span class="sxs-lookup"><span data-stu-id="ab3bc-118">[Object mappings](synchronization-objectmapping.md) are the main part of the synchronization rule.</span></span> <span data-ttu-id="ab3bc-119">どのように特定のオブジェクト同期する必要があるソースからターゲット ・ ディレクトリに各オブジェクトのマッピングを定義します。</span><span class="sxs-lookup"><span data-stu-id="ab3bc-119">Each object mapping defines how a given object should be synchronized from the source to the target directory.</span></span> <span data-ttu-id="ab3bc-120">マッピングがコピー先のディレクトリ内のオブジェクトのソース ディレクトリ内のオブジェクトの照合方法を定義する具体的には、どのような (ある場合) し、オブジェクトを提供するかどうか、オブジェクトの属性を変換する方法を決定するフィルターのスコープを使用する必要があります同期されているソースからコピー先のディレクトリにします。</span><span class="sxs-lookup"><span data-stu-id="ab3bc-120">In particular, the mapping defines how an object in the source directory should be matched with an object in the target directory, what (if any) scoping filters should be used to decide whether to provision an object, and how object attributes should be transformed when they're synchronized from the source to the target directory.</span></span>

## <a name="methods"></a><span data-ttu-id="ab3bc-121">メソッド</span><span class="sxs-lookup"><span data-stu-id="ab3bc-121">Methods</span></span>

| <span data-ttu-id="ab3bc-122">メソッド</span><span class="sxs-lookup"><span data-stu-id="ab3bc-122">Method</span></span>        | <span data-ttu-id="ab3bc-123">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="ab3bc-123">Return Type</span></span>               | <span data-ttu-id="ab3bc-124">説明</span><span class="sxs-lookup"><span data-stu-id="ab3bc-124">Description</span></span>                  |
|:--------------|:--------------------------|:-----------------------------|
|[<span data-ttu-id="ab3bc-125">スキーマを取得します</span><span class="sxs-lookup"><span data-stu-id="ab3bc-125">Get schema</span></span>](../api/synchronization-synchronizationschema-get.md)    |[<span data-ttu-id="ab3bc-126">synchronizationSchema</span><span class="sxs-lookup"><span data-stu-id="ab3bc-126">synchronizationSchema</span></span>](synchronization-synchronizationschema.md)   |<span data-ttu-id="ab3bc-127">**SynchronizationSchema**オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ab3bc-127">Read properties and relationships of the **synchronizationSchema** object.</span></span>|
|[<span data-ttu-id="ab3bc-128">スキーマを更新します。</span><span class="sxs-lookup"><span data-stu-id="ab3bc-128">Update schema</span></span>](../api/synchronization-synchronizationschema-update.md)    |<span data-ttu-id="ab3bc-129">なし</span><span class="sxs-lookup"><span data-stu-id="ab3bc-129">None</span></span>   |<span data-ttu-id="ab3bc-130">同期スキーマを更新します。</span><span class="sxs-lookup"><span data-stu-id="ab3bc-130">Update the synchronization schema.</span></span> |
|[<span data-ttu-id="ab3bc-131">スキーマを削除します。</span><span class="sxs-lookup"><span data-stu-id="ab3bc-131">Delete schema</span></span>](../api/synchronization-synchronizationschema-delete.md)    |<span data-ttu-id="ab3bc-132">なし</span><span class="sxs-lookup"><span data-stu-id="ab3bc-132">None</span></span>   |<span data-ttu-id="ab3bc-133">スキーマを既定の構成にリセットする、カスタマイズされたスキーマを削除します。</span><span class="sxs-lookup"><span data-stu-id="ab3bc-133">Delete the customized schema, resetting the schema to the default configuration.</span></span> |
|[<span data-ttu-id="ab3bc-134">リスト フィルターの演算子</span><span class="sxs-lookup"><span data-stu-id="ab3bc-134">List filter operators</span></span>](../api/synchronization-synchronizationschema-filteroperators.md)    |<span data-ttu-id="ab3bc-135">[filterOperatorSchema](../resources/synchronization-filteroperatorschema.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="ab3bc-135">[filterOperatorSchema](../resources/synchronization-filteroperatorschema.md) colection</span></span>   |<span data-ttu-id="ab3bc-136">スコープ フィルターでサポートされているすべての演算子の一覧を表示します。</span><span class="sxs-lookup"><span data-stu-id="ab3bc-136">List all operators supported in the scoping filters.</span></span> |
|[<span data-ttu-id="ab3bc-137">リストの属性が関数のマッピング</span><span class="sxs-lookup"><span data-stu-id="ab3bc-137">List attribute mapping functions</span></span>](../api/synchronization-synchronizationschema-functions.md)    |<span data-ttu-id="ab3bc-138">[attributeMappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="ab3bc-138">[attributeMappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md) collection</span></span>   |<span data-ttu-id="ab3bc-139">属性マッピングの式でサポートされているすべての関数の一覧を表示します。</span><span class="sxs-lookup"><span data-stu-id="ab3bc-139">List all functions supported in the attribute mapping expressions.</span></span> |
|[<span data-ttu-id="ab3bc-140">属性マッピングの式を解析します。</span><span class="sxs-lookup"><span data-stu-id="ab3bc-140">Parse attribute mapping expression</span></span>](../api/synchronization-synchronizationschema-parseexpression.md)|[<span data-ttu-id="ab3bc-141">parseExpressionResponse</span><span class="sxs-lookup"><span data-stu-id="ab3bc-141">parseExpressionResponse</span></span>](synchronization-parseexpressionresponse.md)|<span data-ttu-id="ab3bc-142">[AttributeMappingSource に文字列を解析します。</span><span class="sxs-lookup"><span data-stu-id="ab3bc-142">Parse a string expression into an [attributeMappingSource</span></span>|<span data-ttu-id="ab3bc-143">(../resources/synchronization_attributemappingsource.md) オブジェクト。</span><span class="sxs-lookup"><span data-stu-id="ab3bc-143">(../resources/synchronization_attributemappingsource.md) object.</span></span>|


## <a name="properties"></a><span data-ttu-id="ab3bc-144">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ab3bc-144">Properties</span></span>

| <span data-ttu-id="ab3bc-145">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ab3bc-145">Property</span></span>      | <span data-ttu-id="ab3bc-146">型</span><span class="sxs-lookup"><span data-stu-id="ab3bc-146">Type</span></span>      | <span data-ttu-id="ab3bc-147">説明</span><span class="sxs-lookup"><span data-stu-id="ab3bc-147">Description</span></span>    |
|:--------------|:----------|:---------------|
|<span data-ttu-id="ab3bc-148">directories</span><span class="sxs-lookup"><span data-stu-id="ab3bc-148">directories</span></span>            |<span data-ttu-id="ab3bc-149">[directoryDefinition](synchronization-directorydefinition.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="ab3bc-149">[directoryDefinition](synchronization-directorydefinition.md) collection</span></span>   |<span data-ttu-id="ab3bc-150">ディレクトリおよび[synchronizationJob](synchronization-synchronizationjob.md)または[synchronizationTemplate](synchronization-synchronizationtemplate.md)の一部であるオブジェクトについて説明します。</span><span class="sxs-lookup"><span data-stu-id="ab3bc-150">Describes directories and objects that are part of the [synchronizationJob](synchronization-synchronizationjob.md) or [synchronizationTemplate](synchronization-synchronizationtemplate.md).</span></span> |
|<span data-ttu-id="ab3bc-151">synchronizationRules</span><span class="sxs-lookup"><span data-stu-id="ab3bc-151">synchronizationRules</span></span>   |<span data-ttu-id="ab3bc-152">[synchronizationRule](synchronization-synchronizationrule.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="ab3bc-152">[synchronizationRule](synchronization-synchronizationrule.md) collection</span></span>   |<span data-ttu-id="ab3bc-153">[SynchronizationJob](synchronization-synchronizationjob.md)または[synchronizationTemplate](synchronization-synchronizationtemplate.md)、用に構成された同期規則のコレクション</span><span class="sxs-lookup"><span data-stu-id="ab3bc-153">A collection of synchronization rules configured for the [synchronizationJob](synchronization-synchronizationjob.md) or [synchronizationTemplate](synchronization-synchronizationtemplate.md),</span></span> |
|<span data-ttu-id="ab3bc-154">version</span><span class="sxs-lookup"><span data-stu-id="ab3bc-154">version</span></span>                |<span data-ttu-id="ab3bc-155">String</span><span class="sxs-lookup"><span data-stu-id="ab3bc-155">String</span></span>                             |<span data-ttu-id="ab3bc-156">スキーマ変更のたびに自動的に更新、スキーマのバージョン。</span><span class="sxs-lookup"><span data-stu-id="ab3bc-156">The version of the schema, updated automatically with every schema change.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="ab3bc-157">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ab3bc-157">JSON representation</span></span>

<span data-ttu-id="ab3bc-158">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="ab3bc-158">The following is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "synchronizationSchema resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-synchronizationschema.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
