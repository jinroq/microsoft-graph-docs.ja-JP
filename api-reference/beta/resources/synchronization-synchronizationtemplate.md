---
title: synchronizationTemplate リソースの種類
description: " すべてのユーザーは、同期スキーマを含む、既定の設定を表示するテンプレートを取得できます。"
localization_priority: Normal
ms.openlocfilehash: 75df13d55cfb58aafe8a751279e103424aa29367
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29516554"
---
# <a name="synchronizationtemplate-resource-type"></a><span data-ttu-id="dca11-103">synchronizationTemplate リソースの種類</span><span class="sxs-lookup"><span data-stu-id="dca11-103">synchronizationTemplate resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dca11-104">特定のアプリケーションの構成済みの同期設定を提供します。</span><span class="sxs-lookup"><span data-stu-id="dca11-104">Provides pre-configured synchronization settings for a particular application.</span></span> <span data-ttu-id="dca11-105">これらの設定は、テンプレートに基づくすべての[同期ジョブ](synchronization-synchronizationjob.md)の既定で使用されます。</span><span class="sxs-lookup"><span data-stu-id="dca11-105">These settings will be used by default for any [synchronization job](synchronization-synchronizationjob.md) that is based on the template.</span></span> <span data-ttu-id="dca11-106">アプリケーション開発者は、テンプレートを指定します。すべてのユーザーは、[同期スキーマ](synchronization-synchronizationschema.md)を含む、既定の設定を表示するテンプレートを取得できます。</span><span class="sxs-lookup"><span data-stu-id="dca11-106">The application developer specifies the template; anyone can retrieve the template to see the default settings, including the [synchronization schema](synchronization-synchronizationschema.md).</span></span>

<span data-ttu-id="dca11-107">アプリケーションは、複数のテンプレートを提供し、既定のテンプレートを指定できます。</span><span class="sxs-lookup"><span data-stu-id="dca11-107">You can provide multiple templates for an application, and designate a default template.</span></span> <span data-ttu-id="dca11-108">関心のアプリケーションの複数のテンプレートがある場合は、お客様のニーズに最も適したどちらかを決定するアプリケーション固有のガイダンスをシークします。</span><span class="sxs-lookup"><span data-stu-id="dca11-108">If multiple templates are available for the application you're interested in, seek application-specific guidance to determine which one best meets your needs.</span></span>

## <a name="methods"></a><span data-ttu-id="dca11-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="dca11-109">Methods</span></span>

| <span data-ttu-id="dca11-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="dca11-110">Method</span></span>        | <span data-ttu-id="dca11-111">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="dca11-111">Return Type</span></span>               | <span data-ttu-id="dca11-112">説明</span><span class="sxs-lookup"><span data-stu-id="dca11-112">Description</span></span>                  |
|:--------------|:--------------------------|:-----------------------------|
|[<span data-ttu-id="dca11-113">List</span><span class="sxs-lookup"><span data-stu-id="dca11-113">List</span></span>](../api/synchronization-synchronizationtemplate-list.md)    |<span data-ttu-id="dca11-114">[synchronizationTemplate](synchronization-synchronizationtemplate.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="dca11-114">[synchronizationTemplate](synchronization-synchronizationtemplate.md) collection</span></span>  |<span data-ttu-id="dca11-115">アプリケーションまたはアプリケーションのインスタンス (サービス主体) の使用可能なテンプレートの一覧を表示します。</span><span class="sxs-lookup"><span data-stu-id="dca11-115">List the templates that are available for an application or application instance (service principal).</span></span>|
|[<span data-ttu-id="dca11-116">Get</span><span class="sxs-lookup"><span data-stu-id="dca11-116">Get</span></span>](../api/synchronization-synchronizationtemplate-get.md)      |[<span data-ttu-id="dca11-117">synchronizationTemplate</span><span class="sxs-lookup"><span data-stu-id="dca11-117">synchronizationTemplate</span></span>](synchronization-synchronizationtemplate.md)   |<span data-ttu-id="dca11-118">プロパティと**synchronizationTemplate**オブジェクトの関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="dca11-118">Read the properties and relationships of the **synchronizationTemplate** object.</span></span>|
<!-- 
|[Create](../api/synchronization-synchronizationtemplate-post.md) |[synchronizationTemplate](synchronization-synchronizationtemplate.md)   |Create a new template for an application.|
|[Update](../api/synchronization-synchronizationtemplate-put.md)   |[synchronizationTemplate](synchronization-synchronizationtemplate.md)   |Update the template.| 
-->

## <a name="properties"></a><span data-ttu-id="dca11-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="dca11-119">Properties</span></span>

| <span data-ttu-id="dca11-120">プロパティ</span><span class="sxs-lookup"><span data-stu-id="dca11-120">Property</span></span>      | <span data-ttu-id="dca11-121">型</span><span class="sxs-lookup"><span data-stu-id="dca11-121">Type</span></span>                      | <span data-ttu-id="dca11-122">説明</span><span class="sxs-lookup"><span data-stu-id="dca11-122">Description</span></span>                  |
|:--------------|:--------------------------|:-----------------------------|
|<span data-ttu-id="dca11-123">id</span><span class="sxs-lookup"><span data-stu-id="dca11-123">id</span></span>             |<span data-ttu-id="dca11-124">文字列</span><span class="sxs-lookup"><span data-stu-id="dca11-124">String</span></span>                     |<span data-ttu-id="dca11-125">テンプレートの一意の識別子です。</span><span class="sxs-lookup"><span data-stu-id="dca11-125">Unique template identifier.</span></span>|
|<span data-ttu-id="dca11-126">applicationId</span><span class="sxs-lookup"><span data-stu-id="dca11-126">applicationId</span></span>  |<span data-ttu-id="dca11-127">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="dca11-127">String</span></span>                     |<span data-ttu-id="dca11-128">このテンプレートが属するアプリケーションの識別子です。</span><span class="sxs-lookup"><span data-stu-id="dca11-128">Identifier of the application this template belongs to.</span></span>|
|<span data-ttu-id="dca11-129">既定値です。</span><span class="sxs-lookup"><span data-stu-id="dca11-129">default</span></span>        |<span data-ttu-id="dca11-130">ブール値</span><span class="sxs-lookup"><span data-stu-id="dca11-130">Boolean</span></span>                    |<span data-ttu-id="dca11-131">`true`場合は、アプリケーションの既定の設定をするのには、このテンプレートをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="dca11-131">`true` if this template is recommended to be the default for the application.</span></span>|
|<span data-ttu-id="dca11-132">説明</span><span class="sxs-lookup"><span data-stu-id="dca11-132">description</span></span>    |<span data-ttu-id="dca11-133">String</span><span class="sxs-lookup"><span data-stu-id="dca11-133">String</span></span>                     |<span data-ttu-id="dca11-134">テンプレートの説明です。</span><span class="sxs-lookup"><span data-stu-id="dca11-134">Description of the template.</span></span>|
|<span data-ttu-id="dca11-135">検出可能</span><span class="sxs-lookup"><span data-stu-id="dca11-135">discoverable</span></span>   |<span data-ttu-id="dca11-136">String</span><span class="sxs-lookup"><span data-stu-id="dca11-136">String</span></span>                     |<span data-ttu-id="dca11-137">`true`このテンプレートは、アプリケーションのインスタンス (サービス主体) の使用可能なテンプレートのコレクションに表示されます。 場合、</span><span class="sxs-lookup"><span data-stu-id="dca11-137">`true` if this template should appear in the collection of templates available for the application instance (service principal).</span></span>|
|<span data-ttu-id="dca11-138">factoryTag</span><span class="sxs-lookup"><span data-stu-id="dca11-138">factoryTag</span></span>     |<span data-ttu-id="dca11-139">String</span><span class="sxs-lookup"><span data-stu-id="dca11-139">String</span></span>                     |<span data-ttu-id="dca11-140">同期エンジンでサポートされている既知の工場出荷時のタグの 1 つです。</span><span class="sxs-lookup"><span data-stu-id="dca11-140">One of the well-known factory tags supported by the synchronization engine.</span></span> <span data-ttu-id="dca11-141">**FactoryTag**は、このテンプレートに基づいてジョブを処理するときに使用する実装を同期エンジンを指示します。</span><span class="sxs-lookup"><span data-stu-id="dca11-141">The **factoryTag** tells the synchronization engine which implementation to use when processing jobs based on this template.</span></span>|
|<span data-ttu-id="dca11-142">metadata</span><span class="sxs-lookup"><span data-stu-id="dca11-142">metadata</span></span>       |<span data-ttu-id="dca11-143">metadataEntry コレクション</span><span class="sxs-lookup"><span data-stu-id="dca11-143">metadataEntry collection</span></span>   |<span data-ttu-id="dca11-144">プロパティをさらに拡張します。</span><span class="sxs-lookup"><span data-stu-id="dca11-144">Additional extension properties.</span></span> <span data-ttu-id="dca11-145">明示的に記載されている、しない限り、メタデータの値を変更できませんする必要があります。</span><span class="sxs-lookup"><span data-stu-id="dca11-145">Unless mentioned explicitly, metadata values should not be changed.</span></span>|

## <a name="relationships"></a><span data-ttu-id="dca11-146">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="dca11-146">Relationships</span></span>
| <span data-ttu-id="dca11-147">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="dca11-147">Relationship</span></span>      | <span data-ttu-id="dca11-148">型</span><span class="sxs-lookup"><span data-stu-id="dca11-148">Type</span></span>      |<span data-ttu-id="dca11-149">説明</span><span class="sxs-lookup"><span data-stu-id="dca11-149">Description</span></span>|
|:------------------|:----------|:----------|
|<span data-ttu-id="dca11-150">スキーマ</span><span class="sxs-lookup"><span data-stu-id="dca11-150">schema</span></span>             |[<span data-ttu-id="dca11-151">synchronizationSchema</span><span class="sxs-lookup"><span data-stu-id="dca11-151">synchronizationSchema</span></span>](synchronization-synchronizationschema.md)     |<span data-ttu-id="dca11-152">このテンプレートに基づいて、ジョブの既定の同期スキーマです。</span><span class="sxs-lookup"><span data-stu-id="dca11-152">Default synchronization schema for the jobs based on this template.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="dca11-153">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="dca11-153">JSON representation</span></span>

<span data-ttu-id="dca11-154">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="dca11-154">The following is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "synchronizationTemplate resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-synchronizationtemplate.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
