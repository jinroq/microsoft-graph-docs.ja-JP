---
title: publishedResource リソースの種類
description: publishedResource リソースの種類。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 54a2b1b610f30ec3ce7d9853916aad345142cbf0
ms.sourcegitcommit: 8844023e15b7649a5c03603aee243acf85930ef2
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/24/2019
ms.locfileid: "35841361"
---
# <a name="publishedresource-resource-type"></a><span data-ttu-id="a27e4-103">publishedResource リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a27e4-103">publishedResource resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a27e4-104">オンプレミスで発行されたリソースを表します。</span><span class="sxs-lookup"><span data-stu-id="a27e4-104">Represents on-premises published resource.</span></span> <span data-ttu-id="a27e4-105">テナント管理者は、テナント管理者によってインストールされたエンタープライズアプリケーション、ドメインコントローラー、サーバー、その他の[オンプレミスエージェント](onpremisesagent.md)を、さまざまな種類のオンプレミスのリソースに公開することができます。発行された特定のリソース。</span><span class="sxs-lookup"><span data-stu-id="a27e4-105">A tenant administrator could publish various types of on-premises resources - enterprise applications, domain controllers, servers, etc. [On-premises agents](onpremisesagent.md) installed by a tenant administrator can be configured to access/handle requests to a particular published resource.</span></span>

## <a name="methods"></a><span data-ttu-id="a27e4-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="a27e4-106">Methods</span></span>

| <span data-ttu-id="a27e4-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="a27e4-107">Method</span></span>       | <span data-ttu-id="a27e4-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="a27e4-108">Return Type</span></span> | <span data-ttu-id="a27e4-109">説明</span><span class="sxs-lookup"><span data-stu-id="a27e4-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="a27e4-110">PublishedResources のリスト</span><span class="sxs-lookup"><span data-stu-id="a27e4-110">List publishedResources</span></span>](../api/publishedresource-list.md) | <span data-ttu-id="a27e4-111">[Publishedresource](publishedresource.md) objects コレクション</span><span class="sxs-lookup"><span data-stu-id="a27e4-111">[publishedResource](publishedresource.md) objects collection</span></span> | <span data-ttu-id="a27e4-112">**Publishedresources**オブジェクトコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="a27e4-112">Get a **publishedResources** object collection.</span></span> |
| [<span data-ttu-id="a27e4-113">PublishedResource の取得</span><span class="sxs-lookup"><span data-stu-id="a27e4-113">Get publishedResource</span></span>](../api/publishedresource-get.md) | [<span data-ttu-id="a27e4-114">publishedResource</span><span class="sxs-lookup"><span data-stu-id="a27e4-114">publishedResource</span></span>](publishedresource.md) | <span data-ttu-id="a27e4-115">**Publishedresource**オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="a27e4-115">Read the properties and relationships of a **publishedResource** object.</span></span> |
| [<span data-ttu-id="a27e4-116">PublishedResource の作成</span><span class="sxs-lookup"><span data-stu-id="a27e4-116">Create publishedResource</span></span>](../api/publishedresource-post.md) |  [<span data-ttu-id="a27e4-117">publishedResource</span><span class="sxs-lookup"><span data-stu-id="a27e4-117">publishedResource</span></span>](publishedresource.md)  | <span data-ttu-id="a27e4-118">新しい**Publishedresource**を作成します。</span><span class="sxs-lookup"><span data-stu-id="a27e4-118">Create a new **publishedResource**.</span></span> |
| [<span data-ttu-id="a27e4-119">PublishedResource の更新</span><span class="sxs-lookup"><span data-stu-id="a27e4-119">Update publishedResource</span></span>](../api/publishedresource-update.md) | [<span data-ttu-id="a27e4-120">publishedResource</span><span class="sxs-lookup"><span data-stu-id="a27e4-120">publishedResource</span></span>](publishedresource.md) | <span data-ttu-id="a27e4-121">**Publishedresource**オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="a27e4-121">Update a **publishedResource** object.</span></span> |
| [<span data-ttu-id="a27e4-122">PublishedResource の削除</span><span class="sxs-lookup"><span data-stu-id="a27e4-122">Delete  publishedResource</span></span>](../api/publishedresource-delete.md) | <span data-ttu-id="a27e4-123">None</span><span class="sxs-lookup"><span data-stu-id="a27e4-123">None</span></span> | <span data-ttu-id="a27e4-124">**Publishedresource**オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="a27e4-124">Delete a **publishedResource** object.</span></span> |
| [<span data-ttu-id="a27e4-125">PublishedResource を onPremisesAgentGroup に割り当てます。</span><span class="sxs-lookup"><span data-stu-id="a27e4-125">Assign publishedResource to onPremisesAgentGroup</span></span>](../api/publishedresource-post-agentgroups.md) | <span data-ttu-id="a27e4-126">None</span><span class="sxs-lookup"><span data-stu-id="a27e4-126">None</span></span> | <span data-ttu-id="a27e4-127">**Publishedresource**オブジェクトを**onPremisesAgentGroup**に割り当てます。</span><span class="sxs-lookup"><span data-stu-id="a27e4-127">Assign a **publishedResource** object to an **onPremisesAgentGroup**.</span></span> |
| [<span data-ttu-id="a27e4-128">OnPremisesAgentGroup から publishedResource を削除する</span><span class="sxs-lookup"><span data-stu-id="a27e4-128">Remove publishedResource from onPremisesAgentGroup</span></span>](../api/publishedresource-delete-agentgroups.md) | <span data-ttu-id="a27e4-129">None</span><span class="sxs-lookup"><span data-stu-id="a27e4-129">None</span></span> |  <span data-ttu-id="a27e4-130">**OnPremisesAgentGroup**から**publishedresource**オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="a27e4-130">Remove a **publishedResource** object from an **onPremisesAgentGroup**.</span></span>|

## <a name="properties"></a><span data-ttu-id="a27e4-131">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a27e4-131">Properties</span></span>

| <span data-ttu-id="a27e4-132">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a27e4-132">Property</span></span>     | <span data-ttu-id="a27e4-133">型</span><span class="sxs-lookup"><span data-stu-id="a27e4-133">Type</span></span>        | <span data-ttu-id="a27e4-134">説明</span><span class="sxs-lookup"><span data-stu-id="a27e4-134">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="a27e4-135">displayName</span><span class="sxs-lookup"><span data-stu-id="a27e4-135">displayName</span></span>|<span data-ttu-id="a27e4-136">String</span><span class="sxs-lookup"><span data-stu-id="a27e4-136">String</span></span>| <span data-ttu-id="a27e4-137">PublishedResource の表示名。</span><span class="sxs-lookup"><span data-stu-id="a27e4-137">Display Name of the publishedResource.</span></span>|
|<span data-ttu-id="a27e4-138">id</span><span class="sxs-lookup"><span data-stu-id="a27e4-138">id</span></span>|<span data-ttu-id="a27e4-139">文字列</span><span class="sxs-lookup"><span data-stu-id="a27e4-139">String</span></span>| <span data-ttu-id="a27e4-140">PublishedResource のオブジェクト id。</span><span class="sxs-lookup"><span data-stu-id="a27e4-140">The object id of the publishedResource.</span></span> <span data-ttu-id="a27e4-141">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="a27e4-141">Read-only.</span></span>|
|<span data-ttu-id="a27e4-142">発行の種類</span><span class="sxs-lookup"><span data-stu-id="a27e4-142">publishingType</span></span>|<span data-ttu-id="a27e4-143">string</span><span class="sxs-lookup"><span data-stu-id="a27e4-143">string</span></span>| <span data-ttu-id="a27e4-144">可能な値は、`appProxy`、`exchangeOnline`、`authentication`、`provisioning`、`adAdministration` です。</span><span class="sxs-lookup"><span data-stu-id="a27e4-144">Possible values are: `appProxy`, `exchangeOnline`, `authentication`, `provisioning`, `adAdministration`.</span></span>|
|<span data-ttu-id="a27e4-145">resourceName</span><span class="sxs-lookup"><span data-stu-id="a27e4-145">resourceName</span></span>|<span data-ttu-id="a27e4-146">String</span><span class="sxs-lookup"><span data-stu-id="a27e4-146">String</span></span>|<span data-ttu-id="a27e4-147">PublishedResource の名前。</span><span class="sxs-lookup"><span data-stu-id="a27e4-147">Name of the publishedResource.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a27e4-148">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="a27e4-148">Relationships</span></span>

| <span data-ttu-id="a27e4-149">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="a27e4-149">Relationship</span></span> | <span data-ttu-id="a27e4-150">型</span><span class="sxs-lookup"><span data-stu-id="a27e4-150">Type</span></span>        | <span data-ttu-id="a27e4-151">説明</span><span class="sxs-lookup"><span data-stu-id="a27e4-151">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="a27e4-152">agentGroups</span><span class="sxs-lookup"><span data-stu-id="a27e4-152">agentGroups</span></span>|<span data-ttu-id="a27e4-153">[onPremisesAgentGroup](onpremisesagentgroup.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="a27e4-153">[onPremisesAgentGroup](onpremisesagentgroup.md) collection</span></span>| <span data-ttu-id="a27e4-154">**Publishedresource**が割り当てられている**onPremisesAgentGroups**のリスト。</span><span class="sxs-lookup"><span data-stu-id="a27e4-154">List of **onPremisesAgentGroups** that a **publishedResource** is assigned to.</span></span> <span data-ttu-id="a27e4-155">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="a27e4-155">Read-only.</span></span> <span data-ttu-id="a27e4-156">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="a27e4-156">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a27e4-157">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a27e4-157">JSON representation</span></span>

<span data-ttu-id="a27e4-158">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="a27e4-158">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.publishedResource",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "displayName": "String",
  "id": "String (identifier)",
  "publishingType": "string",
  "resourceName": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "publishedResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
