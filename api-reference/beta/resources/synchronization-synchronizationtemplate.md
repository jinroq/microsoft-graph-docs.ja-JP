---
title: synchronizationTemplate リソースの種類
description: " すべてのユーザーは、同期スキーマを含む、既定の設定を表示するテンプレートを取得できます。"
ms.openlocfilehash: 90850ad43fdd14fc38ff6ae8cfa97f47806a289d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27070566"
---
# <a name="synchronizationtemplate-resource-type"></a><span data-ttu-id="5f1ef-103">synchronizationTemplate リソースの種類</span><span class="sxs-lookup"><span data-stu-id="5f1ef-103">synchronizationTemplate resource type</span></span>

> <span data-ttu-id="5f1ef-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="5f1ef-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5f1ef-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5f1ef-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5f1ef-106">特定のアプリケーションの構成済みの同期設定を提供します。</span><span class="sxs-lookup"><span data-stu-id="5f1ef-106">Provides pre-configured synchronization settings for a particular application.</span></span> <span data-ttu-id="5f1ef-107">これらの設定は、テンプレートに基づくすべての[同期ジョブ](synchronization-synchronizationjob.md)の既定で使用されます。</span><span class="sxs-lookup"><span data-stu-id="5f1ef-107">These settings will be used by default for any [synchronization job](synchronization-synchronizationjob.md) that is based on the template.</span></span> <span data-ttu-id="5f1ef-108">アプリケーション開発者は、テンプレートを指定します。すべてのユーザーは、[同期スキーマ](synchronization-synchronizationschema.md)を含む、既定の設定を表示するテンプレートを取得できます。</span><span class="sxs-lookup"><span data-stu-id="5f1ef-108">The application developer specifies the template; anyone can retrieve the template to see the default settings, including the [synchronization schema](synchronization-synchronizationschema.md).</span></span>

<span data-ttu-id="5f1ef-109">アプリケーションは、複数のテンプレートを提供し、既定のテンプレートを指定できます。</span><span class="sxs-lookup"><span data-stu-id="5f1ef-109">You can provide multiple templates for an application, and designate a default template.</span></span> <span data-ttu-id="5f1ef-110">関心のアプリケーションの複数のテンプレートがある場合は、お客様のニーズに最も適したどちらかを決定するアプリケーション固有のガイダンスをシークします。</span><span class="sxs-lookup"><span data-stu-id="5f1ef-110">If multiple templates are available for the application you're interested in, seek application-specific guidance to determine which one best meets your needs.</span></span>

## <a name="methods"></a><span data-ttu-id="5f1ef-111">メソッド</span><span class="sxs-lookup"><span data-stu-id="5f1ef-111">Methods</span></span>

| <span data-ttu-id="5f1ef-112">メソッド</span><span class="sxs-lookup"><span data-stu-id="5f1ef-112">Method</span></span>        | <span data-ttu-id="5f1ef-113">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="5f1ef-113">Return Type</span></span>               | <span data-ttu-id="5f1ef-114">説明</span><span class="sxs-lookup"><span data-stu-id="5f1ef-114">Description</span></span>                  |
|:--------------|:--------------------------|:-----------------------------|
|[<span data-ttu-id="5f1ef-115">List</span><span class="sxs-lookup"><span data-stu-id="5f1ef-115">List</span></span>](../api/synchronization-synchronizationtemplate-list.md)    |<span data-ttu-id="5f1ef-116">[synchronizationTemplate](synchronization-synchronizationtemplate.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="5f1ef-116">[synchronizationTemplate](synchronization-synchronizationtemplate.md) collection</span></span>  |<span data-ttu-id="5f1ef-117">アプリケーションまたはアプリケーションのインスタンス (サービス主体) の使用可能なテンプレートの一覧を表示します。</span><span class="sxs-lookup"><span data-stu-id="5f1ef-117">List the templates that are available for an application or application instance (service principal).</span></span>|
|[<span data-ttu-id="5f1ef-118">Get</span><span class="sxs-lookup"><span data-stu-id="5f1ef-118">Get</span></span>](../api/synchronization-synchronizationtemplate-get.md)      |[<span data-ttu-id="5f1ef-119">synchronizationTemplate</span><span class="sxs-lookup"><span data-stu-id="5f1ef-119">synchronizationTemplate</span></span>](synchronization-synchronizationtemplate.md)   |<span data-ttu-id="5f1ef-120">プロパティと**synchronizationTemplate**オブジェクトの関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5f1ef-120">Read the properties and relationships of the **synchronizationTemplate** object.</span></span>|
<!-- 
|[Create](../api/synchronization-synchronizationtemplate-post.md) |[synchronizationTemplate](synchronization-synchronizationtemplate.md)   |Create a new template for an application.|
|[Update](../api/synchronization-synchronizationtemplate-put.md)   |[synchronizationTemplate](synchronization-synchronizationtemplate.md)   |Update the template.| 
-->

## <a name="properties"></a><span data-ttu-id="5f1ef-121">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5f1ef-121">Properties</span></span>

| <span data-ttu-id="5f1ef-122">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5f1ef-122">Property</span></span>      | <span data-ttu-id="5f1ef-123">型</span><span class="sxs-lookup"><span data-stu-id="5f1ef-123">Type</span></span>                      | <span data-ttu-id="5f1ef-124">説明</span><span class="sxs-lookup"><span data-stu-id="5f1ef-124">Description</span></span>                  |
|:--------------|:--------------------------|:-----------------------------|
|<span data-ttu-id="5f1ef-125">id</span><span class="sxs-lookup"><span data-stu-id="5f1ef-125">id</span></span>             |<span data-ttu-id="5f1ef-126">String</span><span class="sxs-lookup"><span data-stu-id="5f1ef-126">String</span></span>                     |<span data-ttu-id="5f1ef-127">テンプレートの一意の識別子です。</span><span class="sxs-lookup"><span data-stu-id="5f1ef-127">Unique template identifier.</span></span>|
|<span data-ttu-id="5f1ef-128">applicationId</span><span class="sxs-lookup"><span data-stu-id="5f1ef-128">applicationId</span></span>  |<span data-ttu-id="5f1ef-129">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="5f1ef-129">String</span></span>                     |<span data-ttu-id="5f1ef-130">このテンプレートが属するアプリケーションの識別子です。</span><span class="sxs-lookup"><span data-stu-id="5f1ef-130">Identifier of the application this template belongs to.</span></span>|
|<span data-ttu-id="5f1ef-131">既定値です。</span><span class="sxs-lookup"><span data-stu-id="5f1ef-131">default</span></span>        |<span data-ttu-id="5f1ef-132">ブール値</span><span class="sxs-lookup"><span data-stu-id="5f1ef-132">Boolean</span></span>                    |<span data-ttu-id="5f1ef-133">`true`場合は、アプリケーションの既定の設定をするのには、このテンプレートをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="5f1ef-133">`true` if this template is recommended to be the default for the application.</span></span>|
|<span data-ttu-id="5f1ef-134">説明</span><span class="sxs-lookup"><span data-stu-id="5f1ef-134">description</span></span>    |<span data-ttu-id="5f1ef-135">文字列</span><span class="sxs-lookup"><span data-stu-id="5f1ef-135">String</span></span>                     |<span data-ttu-id="5f1ef-136">テンプレートの説明です。</span><span class="sxs-lookup"><span data-stu-id="5f1ef-136">Description of the template.</span></span>|
|<span data-ttu-id="5f1ef-137">検出可能</span><span class="sxs-lookup"><span data-stu-id="5f1ef-137">discoverable</span></span>   |<span data-ttu-id="5f1ef-138">String</span><span class="sxs-lookup"><span data-stu-id="5f1ef-138">String</span></span>                     |<span data-ttu-id="5f1ef-139">`true`このテンプレートは、アプリケーションのインスタンス (サービス主体) の使用可能なテンプレートのコレクションに表示されます。 場合、</span><span class="sxs-lookup"><span data-stu-id="5f1ef-139">`true` if this template should appear in the collection of templates available for the application instance (service principal).</span></span>|
|<span data-ttu-id="5f1ef-140">factoryTag</span><span class="sxs-lookup"><span data-stu-id="5f1ef-140">factoryTag</span></span>     |<span data-ttu-id="5f1ef-141">String</span><span class="sxs-lookup"><span data-stu-id="5f1ef-141">String</span></span>                     |<span data-ttu-id="5f1ef-142">同期エンジンでサポートされている既知の工場出荷時のタグの 1 つです。</span><span class="sxs-lookup"><span data-stu-id="5f1ef-142">One of the well-known factory tags supported by the synchronization engine.</span></span> <span data-ttu-id="5f1ef-143">**FactoryTag**は、このテンプレートに基づいてジョブを処理するときに使用する実装を同期エンジンを指示します。</span><span class="sxs-lookup"><span data-stu-id="5f1ef-143">The **factoryTag** tells the synchronization engine which implementation to use when processing jobs based on this template.</span></span>|
|<span data-ttu-id="5f1ef-144">metadata</span><span class="sxs-lookup"><span data-stu-id="5f1ef-144">metadata</span></span>       |<span data-ttu-id="5f1ef-145">metadataEntry コレクション</span><span class="sxs-lookup"><span data-stu-id="5f1ef-145">metadataEntry collection</span></span>   |<span data-ttu-id="5f1ef-146">プロパティをさらに拡張します。</span><span class="sxs-lookup"><span data-stu-id="5f1ef-146">Additional extension properties.</span></span> <span data-ttu-id="5f1ef-147">明示的に記載されている、しない限り、メタデータの値を変更できませんする必要があります。</span><span class="sxs-lookup"><span data-stu-id="5f1ef-147">Unless mentioned explicitly, metadata values should not be changed.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5f1ef-148">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="5f1ef-148">Relationships</span></span>
| <span data-ttu-id="5f1ef-149">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="5f1ef-149">Relationship</span></span>      | <span data-ttu-id="5f1ef-150">型</span><span class="sxs-lookup"><span data-stu-id="5f1ef-150">Type</span></span>      |<span data-ttu-id="5f1ef-151">説明</span><span class="sxs-lookup"><span data-stu-id="5f1ef-151">Description</span></span>|
|:------------------|:----------|:----------|
|<span data-ttu-id="5f1ef-152">スキーマ</span><span class="sxs-lookup"><span data-stu-id="5f1ef-152">schema</span></span>             |[<span data-ttu-id="5f1ef-153">synchronizationSchema</span><span class="sxs-lookup"><span data-stu-id="5f1ef-153">synchronizationSchema</span></span>](synchronization-synchronizationschema.md)     |<span data-ttu-id="5f1ef-154">このテンプレートに基づいて、ジョブの既定の同期スキーマです。</span><span class="sxs-lookup"><span data-stu-id="5f1ef-154">Default synchronization schema for the jobs based on this template.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5f1ef-155">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="5f1ef-155">JSON representation</span></span>

<span data-ttu-id="5f1ef-156">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="5f1ef-156">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
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
<!-- {
  "type": "#page.annotation",
  "description": "synchronizationTemplate resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->