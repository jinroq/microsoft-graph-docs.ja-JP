---
title: 同期スキーマリソースの種類
description: 同期されるオブジェクトと、それらの同期方法を定義します。 同期スキーマには、特定の同期ジョブの設定情報の大部分が含まれています。 通常、属性マッピングの一部をカスタマイズするか、特定の条件を満たすオブジェクトのみを同期するスコープフィルターを追加します。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 7d4302cec5fe568f322e5a8d1b86bc4681b50f7c
ms.sourcegitcommit: 121c0fad692fb3c5c01dc051481b5249e4491b48
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/11/2019
ms.locfileid: "35620683"
---
# <a name="synchronizationschema-resource-type"></a><span data-ttu-id="c1aa4-105">同期スキーマリソースの種類</span><span class="sxs-lookup"><span data-stu-id="c1aa4-105">synchronizationSchema resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c1aa4-106">同期されるオブジェクトと、それらの同期方法を定義します。</span><span class="sxs-lookup"><span data-stu-id="c1aa4-106">Defines what objects will be synchronized and how they will be synchronized.</span></span> <span data-ttu-id="c1aa4-107">同期スキーマには、特定の同期ジョブの設定情報の大部分が含まれています。</span><span class="sxs-lookup"><span data-stu-id="c1aa4-107">The synchronization schema contains most of the setup information for a particular synchronization job.</span></span> <span data-ttu-id="c1aa4-108">通常、[属性マッピング](synchronization-attributemapping.md)の一部をカスタマイズするか、特定の条件を満たすオブジェクトのみを同期する[スコープフィルター](synchronization-filter.md)を追加します。</span><span class="sxs-lookup"><span data-stu-id="c1aa4-108">Typically, you will customize some of the [attribute mappings](synchronization-attributemapping.md), or add a [scoping filter](synchronization-filter.md) to synchronize only objects that satisfy a certain condition.</span></span>

<span data-ttu-id="c1aa4-109">次のセクションでは、同期スキーマの高レベルのコンポーネントについて説明します。</span><span class="sxs-lookup"><span data-stu-id="c1aa4-109">The following sections describe the high-level components of the synchronization schema.</span></span>

## <a name="directory-definitions"></a><span data-ttu-id="c1aa4-110">ディレクトリ定義</span><span class="sxs-lookup"><span data-stu-id="c1aa4-110">Directory definitions</span></span>

<span data-ttu-id="c1aa4-111">[ディレクトリ定義](synchronization-directorydefinition.md)は、ディレクトリとそのオブジェクトに関する同期エンジン情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="c1aa4-111">[Directory definitions](synchronization-directorydefinition.md) provide the synchronization engine information about directories and their objects.</span></span> <span data-ttu-id="c1aa4-112">たとえば、ディレクトリ定義は、Azure AD ディレクトリに、**ユーザー**と**グループ**という名前のオブジェクトがあり、それらのオブジェクトに対してサポートされている属性、およびそれらの属性の種類があることを同期エンジンに通知します。</span><span class="sxs-lookup"><span data-stu-id="c1aa4-112">For example, the directory definition tells the synchronization engine that an Azure AD directory has objects named **user** and **group**, which attributes are supported for those objects, and the types for those attributes.</span></span> <span data-ttu-id="c1aa4-113">同期ルール/オブジェクトマッピングで特定のオブジェクトおよび属性を使用するためには、それらをディレクトリ定義の一部として定義する必要があります。</span><span class="sxs-lookup"><span data-stu-id="c1aa4-113">In order for a particular object and attribute to be used in synchronization rules/object mappings, they have to be defined as part of the directory definition.</span></span>

## <a name="synchronization-rules"></a><span data-ttu-id="c1aa4-114">同期ルール</span><span class="sxs-lookup"><span data-stu-id="c1aa4-114">Synchronization rules</span></span>

<span data-ttu-id="c1aa4-115">[同期ルール](synchronization-synchronizationrule.md)は、同期のセットアップの中核となります。</span><span class="sxs-lookup"><span data-stu-id="c1aa4-115">[Synchronization rules](synchronization-synchronizationrule.md) are the core of the synchronization setup.</span></span> <span data-ttu-id="c1aa4-116">同期を実行する方法、同期する必要のあるオブジェクト、ソースディレクトリのオブジェクトとターゲットディレクトリのオブジェクトとの比較、属性の適用方法など、同期エンジンを定義します。ソースからターゲットディレクトリへの同期時に変換されます。</span><span class="sxs-lookup"><span data-stu-id="c1aa4-116">They define for the synchronization engine how the synchronization should be performed, including what objects should be synchronized, how objects from the source directory should be matched with objects in the target directory, and how attributes should be transformed when they're synchronized from the source to the target directory.</span></span> 

## <a name="object-mappings"></a><span data-ttu-id="c1aa4-117">オブジェクトマッピング</span><span class="sxs-lookup"><span data-stu-id="c1aa4-117">Object mappings</span></span>

<span data-ttu-id="c1aa4-118">[オブジェクトマッピング](synchronization-objectmapping.md)は、同期ルールの主な部分です。</span><span class="sxs-lookup"><span data-stu-id="c1aa4-118">[Object mappings](synchronization-objectmapping.md) are the main part of the synchronization rule.</span></span> <span data-ttu-id="c1aa4-119">各オブジェクトマッピングは、指定されたオブジェクトをソースからターゲットディレクトリへ同期する方法を定義します。</span><span class="sxs-lookup"><span data-stu-id="c1aa4-119">Each object mapping defines how a given object should be synchronized from the source to the target directory.</span></span> <span data-ttu-id="c1aa4-120">特に、マッピングでは、ソースディレクトリ内のオブジェクトをターゲットディレクトリのオブジェクトと照合する方法、オブジェクトをプロビジョニングするかどうか、およびオブジェクト属性をどのように変換するかを決定するために使用するスコープフィルターを定義します。ソースからターゲットディレクトリに同期されている場合。</span><span class="sxs-lookup"><span data-stu-id="c1aa4-120">In particular, the mapping defines how an object in the source directory should be matched with an object in the target directory, what (if any) scoping filters should be used to decide whether to provision an object, and how object attributes should be transformed when they're synchronized from the source to the target directory.</span></span>

## <a name="methods"></a><span data-ttu-id="c1aa4-121">メソッド</span><span class="sxs-lookup"><span data-stu-id="c1aa4-121">Methods</span></span>

| <span data-ttu-id="c1aa4-122">メソッド</span><span class="sxs-lookup"><span data-stu-id="c1aa4-122">Method</span></span>        | <span data-ttu-id="c1aa4-123">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="c1aa4-123">Return Type</span></span>               | <span data-ttu-id="c1aa4-124">説明</span><span class="sxs-lookup"><span data-stu-id="c1aa4-124">Description</span></span>                  |
|:--------------|:--------------------------|:-----------------------------|
|[<span data-ttu-id="c1aa4-125">スキーマを取得する</span><span class="sxs-lookup"><span data-stu-id="c1aa4-125">Get schema</span></span>](../api/synchronization-synchronizationschema-get.md)    |[<span data-ttu-id="c1aa4-126">同期スキーマ</span><span class="sxs-lookup"><span data-stu-id="c1aa4-126">synchronizationSchema</span></span>](synchronization-synchronizationschema.md)   |<span data-ttu-id="c1aa4-127">**同期スキーマ**オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="c1aa4-127">Read properties and relationships of the **synchronizationSchema** object.</span></span>|
|[<span data-ttu-id="c1aa4-128">スキーマを更新する</span><span class="sxs-lookup"><span data-stu-id="c1aa4-128">Update schema</span></span>](../api/synchronization-synchronizationschema-update.md)    |<span data-ttu-id="c1aa4-129">None</span><span class="sxs-lookup"><span data-stu-id="c1aa4-129">None</span></span>   |<span data-ttu-id="c1aa4-130">同期スキーマを更新します。</span><span class="sxs-lookup"><span data-stu-id="c1aa4-130">Update the synchronization schema.</span></span> |
|[<span data-ttu-id="c1aa4-131">スキーマの削除</span><span class="sxs-lookup"><span data-stu-id="c1aa4-131">Delete schema</span></span>](../api/synchronization-synchronizationschema-delete.md)    |<span data-ttu-id="c1aa4-132">None</span><span class="sxs-lookup"><span data-stu-id="c1aa4-132">None</span></span>   |<span data-ttu-id="c1aa4-133">カスタマイズしたスキーマを削除し、スキーマを既定の構成にリセットします。</span><span class="sxs-lookup"><span data-stu-id="c1aa4-133">Delete the customized schema, resetting the schema to the default configuration.</span></span> |
|[<span data-ttu-id="c1aa4-134">リストフィルター演算子</span><span class="sxs-lookup"><span data-stu-id="c1aa4-134">List filter operators</span></span>](../api/synchronization-synchronizationschema-filteroperators.md)    |<span data-ttu-id="c1aa4-135">[Filter演算子スキーマ](../resources/synchronization-filteroperatorschema.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="c1aa4-135">[filterOperatorSchema](../resources/synchronization-filteroperatorschema.md) colection</span></span>   |<span data-ttu-id="c1aa4-136">スコープフィルターでサポートされているすべての演算子を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="c1aa4-136">List all operators supported in the scoping filters.</span></span> |
|[<span data-ttu-id="c1aa4-137">リスト属性マッピング関数</span><span class="sxs-lookup"><span data-stu-id="c1aa4-137">List attribute mapping functions</span></span>](../api/synchronization-synchronizationschema-functions.md)    |<span data-ttu-id="c1aa4-138">[attributeMappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="c1aa4-138">[attributeMappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md) collection</span></span>   |<span data-ttu-id="c1aa4-139">属性マッピング式でサポートされているすべての関数を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="c1aa4-139">List all functions supported in the attribute mapping expressions.</span></span> |
|[<span data-ttu-id="c1aa4-140">解析属性マッピング式</span><span class="sxs-lookup"><span data-stu-id="c1aa4-140">Parse attribute mapping expression</span></span>](../api/synchronization-synchronizationschema-parseexpression.md)|[<span data-ttu-id="c1aa4-141">Parseexpression Response</span><span class="sxs-lookup"><span data-stu-id="c1aa4-141">parseExpressionResponse</span></span>](synchronization-parseexpressionresponse.md)|<span data-ttu-id="c1aa4-142">文字列式を解析し、[attributeMappingSource</span><span class="sxs-lookup"><span data-stu-id="c1aa4-142">Parse a string expression into an [attributeMappingSource</span></span>|<span data-ttu-id="c1aa4-143">(../resources/synchronization_attributemappingsource.md) オブジェクト。</span><span class="sxs-lookup"><span data-stu-id="c1aa4-143">(../resources/synchronization_attributemappingsource.md) object.</span></span>|


## <a name="properties"></a><span data-ttu-id="c1aa4-144">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c1aa4-144">Properties</span></span>

| <span data-ttu-id="c1aa4-145">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c1aa4-145">Property</span></span>      | <span data-ttu-id="c1aa4-146">型</span><span class="sxs-lookup"><span data-stu-id="c1aa4-146">Type</span></span>      | <span data-ttu-id="c1aa4-147">説明</span><span class="sxs-lookup"><span data-stu-id="c1aa4-147">Description</span></span>    |
|:--------------|:----------|:---------------|
|<span data-ttu-id="c1aa4-148">移動</span><span class="sxs-lookup"><span data-stu-id="c1aa4-148">directories</span></span>            |<span data-ttu-id="c1aa4-149">[Directorydefinition](synchronization-directorydefinition.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="c1aa4-149">[directoryDefinition](synchronization-directorydefinition.md) collection</span></span>   |<span data-ttu-id="c1aa4-150">[同期ジョブ](synchronization-synchronizationjob.md)または[同期のテンプレート](synchronization-synchronizationtemplate.md)の一部であるディレクトリとオブジェクトについて説明します。</span><span class="sxs-lookup"><span data-stu-id="c1aa4-150">Describes directories and objects that are part of the [synchronizationJob](synchronization-synchronizationjob.md) or [synchronizationTemplate](synchronization-synchronizationtemplate.md).</span></span> |
|<span data-ttu-id="c1aa4-151">同期規則</span><span class="sxs-lookup"><span data-stu-id="c1aa4-151">synchronizationRules</span></span>   |<span data-ttu-id="c1aa4-152">[同期ルール](synchronization-synchronizationrule.md)のコレクション</span><span class="sxs-lookup"><span data-stu-id="c1aa4-152">[synchronizationRule](synchronization-synchronizationrule.md) collection</span></span>   |<span data-ttu-id="c1aa4-153">同期ジョブまたは同期[ジョブ](synchronization-synchronizationjob.md)[テンプレート](synchronization-synchronizationtemplate.md)用に構成されている同期ルールのコレクション。</span><span class="sxs-lookup"><span data-stu-id="c1aa4-153">A collection of synchronization rules configured for the [synchronizationJob](synchronization-synchronizationjob.md) or [synchronizationTemplate](synchronization-synchronizationtemplate.md),</span></span> |
|<span data-ttu-id="c1aa4-154">version</span><span class="sxs-lookup"><span data-stu-id="c1aa4-154">version</span></span>                |<span data-ttu-id="c1aa4-155">String</span><span class="sxs-lookup"><span data-stu-id="c1aa4-155">String</span></span>                             |<span data-ttu-id="c1aa4-156">スキーマのバージョンは、すべてのスキーマ変更によって自動的に更新されます。</span><span class="sxs-lookup"><span data-stu-id="c1aa4-156">The version of the schema, updated automatically with every schema change.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="c1aa4-157">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c1aa4-157">JSON representation</span></span>

<span data-ttu-id="c1aa4-158">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="c1aa4-158">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": []
}
-->
