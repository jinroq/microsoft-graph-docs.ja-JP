---
title: 同期テンプレートリソースの種類
description: " すべてのユーザーがテンプレートを取得して、同期スキーマを含む既定の設定を確認できます。"
localization_priority: Normal
doc_type: resourcePageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: a9176c092d62b4ee43d15d29884a3882fd3c627e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964600"
---
# <a name="synchronizationtemplate-resource-type"></a><span data-ttu-id="27930-103">同期テンプレートリソースの種類</span><span class="sxs-lookup"><span data-stu-id="27930-103">synchronizationTemplate resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="27930-104">特定のアプリケーションに事前に構成された同期設定を提供します。</span><span class="sxs-lookup"><span data-stu-id="27930-104">Provides pre-configured synchronization settings for a particular application.</span></span> <span data-ttu-id="27930-105">これらの設定は、テンプレートに基づくすべての[同期ジョブ](synchronization-synchronizationjob.md)に対して既定で使用されます。</span><span class="sxs-lookup"><span data-stu-id="27930-105">These settings will be used by default for any [synchronization job](synchronization-synchronizationjob.md) that is based on the template.</span></span> <span data-ttu-id="27930-106">アプリケーション開発者は、テンプレートを指定します。すべてのユーザーがテンプレートを取得して、[同期スキーマ](synchronization-synchronizationschema.md)を含む既定の設定を確認できます。</span><span class="sxs-lookup"><span data-stu-id="27930-106">The application developer specifies the template; anyone can retrieve the template to see the default settings, including the [synchronization schema](synchronization-synchronizationschema.md).</span></span>

<span data-ttu-id="27930-107">アプリケーションに対して複数のテンプレートを提供し、既定のテンプレートを指定することができます。</span><span class="sxs-lookup"><span data-stu-id="27930-107">You can provide multiple templates for an application, and designate a default template.</span></span> <span data-ttu-id="27930-108">目的のアプリケーションで複数のテンプレートが使用可能な場合は、アプリケーション固有のガイダンスを検索して、ニーズに最適なものを決定します。</span><span class="sxs-lookup"><span data-stu-id="27930-108">If multiple templates are available for the application you're interested in, seek application-specific guidance to determine which one best meets your needs.</span></span>

## <a name="methods"></a><span data-ttu-id="27930-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="27930-109">Methods</span></span>

| <span data-ttu-id="27930-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="27930-110">Method</span></span>        | <span data-ttu-id="27930-111">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="27930-111">Return Type</span></span>               | <span data-ttu-id="27930-112">説明</span><span class="sxs-lookup"><span data-stu-id="27930-112">Description</span></span>                  |
|:--------------|:--------------------------|:-----------------------------|
|[<span data-ttu-id="27930-113">List</span><span class="sxs-lookup"><span data-stu-id="27930-113">List</span></span>](../api/synchronization-synchronizationtemplate-list.md)    |<span data-ttu-id="27930-114">[同期テンプレート](synchronization-synchronizationtemplate.md)のコレクション</span><span class="sxs-lookup"><span data-stu-id="27930-114">[synchronizationTemplate](synchronization-synchronizationtemplate.md) collection</span></span>  |<span data-ttu-id="27930-115">アプリケーションまたはアプリケーションインスタンス (サービスプリンシパル) に対して使用可能なテンプレートを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="27930-115">List the templates that are available for an application or application instance (service principal).</span></span>|
|[<span data-ttu-id="27930-116">Get</span><span class="sxs-lookup"><span data-stu-id="27930-116">Get</span></span>](../api/synchronization-synchronizationtemplate-get.md)      |[<span data-ttu-id="27930-117">同期テンプレート</span><span class="sxs-lookup"><span data-stu-id="27930-117">synchronizationTemplate</span></span>](synchronization-synchronizationtemplate.md)   |<span data-ttu-id="27930-118">**同期テンプレート**オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="27930-118">Read the properties and relationships of the **synchronizationTemplate** object.</span></span>|
<!-- 
|[Create](../api/synchronization-synchronizationtemplate-post.md) |[synchronizationTemplate](synchronization-synchronizationtemplate.md)   |Create a new template for an application.|
|[Update](../api/synchronization-synchronizationtemplate-put.md)   |[synchronizationTemplate](synchronization-synchronizationtemplate.md)   |Update the template.| 
-->

## <a name="properties"></a><span data-ttu-id="27930-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="27930-119">Properties</span></span>

| <span data-ttu-id="27930-120">プロパティ</span><span class="sxs-lookup"><span data-stu-id="27930-120">Property</span></span>      | <span data-ttu-id="27930-121">型</span><span class="sxs-lookup"><span data-stu-id="27930-121">Type</span></span>                      | <span data-ttu-id="27930-122">説明</span><span class="sxs-lookup"><span data-stu-id="27930-122">Description</span></span>                  |
|:--------------|:--------------------------|:-----------------------------|
|<span data-ttu-id="27930-123">id</span><span class="sxs-lookup"><span data-stu-id="27930-123">id</span></span>             |<span data-ttu-id="27930-124">String</span><span class="sxs-lookup"><span data-stu-id="27930-124">String</span></span>                     |<span data-ttu-id="27930-125">一意のテンプレート識別子。</span><span class="sxs-lookup"><span data-stu-id="27930-125">Unique template identifier.</span></span>|
|<span data-ttu-id="27930-126">applicationId</span><span class="sxs-lookup"><span data-stu-id="27930-126">applicationId</span></span>  |<span data-ttu-id="27930-127">String</span><span class="sxs-lookup"><span data-stu-id="27930-127">String</span></span>                     |<span data-ttu-id="27930-128">このテンプレートが属しているアプリケーションの識別子。</span><span class="sxs-lookup"><span data-stu-id="27930-128">Identifier of the application this template belongs to.</span></span>|
|<span data-ttu-id="27930-129">既定値です。</span><span class="sxs-lookup"><span data-stu-id="27930-129">default</span></span>        |<span data-ttu-id="27930-130">Boolean</span><span class="sxs-lookup"><span data-stu-id="27930-130">Boolean</span></span>                    |<span data-ttu-id="27930-131">`true`このテンプレートをアプリケーションの既定として使用することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="27930-131">`true` if this template is recommended to be the default for the application.</span></span>|
|<span data-ttu-id="27930-132">description</span><span class="sxs-lookup"><span data-stu-id="27930-132">description</span></span>    |<span data-ttu-id="27930-133">String</span><span class="sxs-lookup"><span data-stu-id="27930-133">String</span></span>                     |<span data-ttu-id="27930-134">テンプレートの説明。</span><span class="sxs-lookup"><span data-stu-id="27930-134">Description of the template.</span></span>|
|<span data-ttu-id="27930-135">発見</span><span class="sxs-lookup"><span data-stu-id="27930-135">discoverable</span></span>   |<span data-ttu-id="27930-136">String</span><span class="sxs-lookup"><span data-stu-id="27930-136">String</span></span>                     |<span data-ttu-id="27930-137">`true`このテンプレートをアプリケーションインスタンス (サービスプリンシパル) で使用可能なテンプレートのコレクションに表示する必要がある場合。</span><span class="sxs-lookup"><span data-stu-id="27930-137">`true` if this template should appear in the collection of templates available for the application instance (service principal).</span></span>|
|<span data-ttu-id="27930-138">factoryTag</span><span class="sxs-lookup"><span data-stu-id="27930-138">factoryTag</span></span>     |<span data-ttu-id="27930-139">String</span><span class="sxs-lookup"><span data-stu-id="27930-139">String</span></span>                     |<span data-ttu-id="27930-140">同期エンジンでサポートされている、既知の出荷済みのタグの1つ。</span><span class="sxs-lookup"><span data-stu-id="27930-140">One of the well-known factory tags supported by the synchronization engine.</span></span> <span data-ttu-id="27930-141">**FactoryTag**は、このテンプレートに基づいてジョブを処理するときに使用する実装を同期エンジンに通知します。</span><span class="sxs-lookup"><span data-stu-id="27930-141">The **factoryTag** tells the synchronization engine which implementation to use when processing jobs based on this template.</span></span>|
|<span data-ttu-id="27930-142">metadata</span><span class="sxs-lookup"><span data-stu-id="27930-142">metadata</span></span>       |<span data-ttu-id="27930-143">metadataEntry コレクション</span><span class="sxs-lookup"><span data-stu-id="27930-143">metadataEntry collection</span></span>   |<span data-ttu-id="27930-144">追加の拡張機能のプロパティ。</span><span class="sxs-lookup"><span data-stu-id="27930-144">Additional extension properties.</span></span> <span data-ttu-id="27930-145">明示的に記述されていない限り、メタデータ値は変更しないでください。</span><span class="sxs-lookup"><span data-stu-id="27930-145">Unless mentioned explicitly, metadata values should not be changed.</span></span>|

## <a name="relationships"></a><span data-ttu-id="27930-146">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="27930-146">Relationships</span></span>
| <span data-ttu-id="27930-147">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="27930-147">Relationship</span></span>      | <span data-ttu-id="27930-148">型</span><span class="sxs-lookup"><span data-stu-id="27930-148">Type</span></span>      |<span data-ttu-id="27930-149">説明</span><span class="sxs-lookup"><span data-stu-id="27930-149">Description</span></span>|
|:------------------|:----------|:----------|
|<span data-ttu-id="27930-150">スキーマ</span><span class="sxs-lookup"><span data-stu-id="27930-150">schema</span></span>             |[<span data-ttu-id="27930-151">同期スキーマ</span><span class="sxs-lookup"><span data-stu-id="27930-151">synchronizationSchema</span></span>](synchronization-synchronizationschema.md)     |<span data-ttu-id="27930-152">このテンプレートに基づくジョブの既定の同期スキーマ。</span><span class="sxs-lookup"><span data-stu-id="27930-152">Default synchronization schema for the jobs based on this template.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="27930-153">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="27930-153">JSON representation</span></span>

<span data-ttu-id="27930-154">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="27930-154">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.synchronizationTemplate"
}-->

```json
{
  "applicationId": "String (identifier)",
  "default": true,
  "description": "String",
  "discoverable": true,
  "factoryTag": "String",
  "id": "String (identifier)",
  "metadata": [{"@odata.type": "microsoft.graph.metadataEntry"}],
  "schema": {"@odata.type": "microsoft.graph.synchronizationSchema"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "synchronizationTemplate resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
