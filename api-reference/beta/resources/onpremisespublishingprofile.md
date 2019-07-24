---
title: onPremisesPublishingProfile リソースの種類
description: onPremisesPublishingProfile リソースの種類。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 1eb442b6f3317ac7c0e2f130442e4a62c7f9c152
ms.sourcegitcommit: 8844023e15b7649a5c03603aee243acf85930ef2
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/24/2019
ms.locfileid: "35841326"
---
# <a name="onpremisespublishingprofile-resource-type"></a><span data-ttu-id="e434a-103">onPremisesPublishingProfile リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e434a-103">onPremisesPublishingProfile resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e434a-104">さまざまな Azure サービス (たとえば、Azue Active Directory Connect パススルー認証、Workday to Azure AD ユーザープロビジョニング) は、企業ネットワークの外部からさまざまな社内リソースへの条件付きアクセスを許可します。</span><span class="sxs-lookup"><span data-stu-id="e434a-104">Various Azure services (for example, Azue Active Directory Connect Passthrough Authentication, Workday to Azure AD users provisioning) allow a conditional access to various on-premises resources from outside the corporate network.</span></span> <span data-ttu-id="e434a-105">テナント管理者によってインストールされた[社内エージェント](onpremisesagent.md)は、発行された特定の[リソース](publishedresource.md)への要求にアクセスしたり、処理したりするように構成できます。</span><span class="sxs-lookup"><span data-stu-id="e434a-105">[On-premises agents](onpremisesagent.md) installed by a tenant administrator can be configured to access/handle requests to a particular [published resource](publishedresource.md).</span></span>
<span data-ttu-id="e434a-106">[エージェントグループ](onpremisesagentgroup.md)を使用すると、テナント管理者は特定のエージェントを割り当てて、発行された特定の社内リソースを提供できます。</span><span class="sxs-lookup"><span data-stu-id="e434a-106">[Agent groups](onpremisesagentgroup.md) enable a tenant admin to assign specific agents to serve specific published on-premises resources.</span></span> <span data-ttu-id="e434a-107">テナント管理者は、複数のエージェントをまとめてグループ化し、発行された各リソースをグループに割り当てることができます。</span><span class="sxs-lookup"><span data-stu-id="e434a-107">Tenant admins can group a number of agents together, and then assign each published resource to a group.</span></span> <span data-ttu-id="e434a-108">同じオンプレミスの発行タイプのエンティティセット全体が**onPremisesPublishingProfile**によって表されます。</span><span class="sxs-lookup"><span data-stu-id="e434a-108">The entire set of entities of the same on-premises publishing type is represented by **onPremisesPublishingProfile**.</span></span>

## <a name="methods"></a><span data-ttu-id="e434a-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="e434a-109">Methods</span></span>

| <span data-ttu-id="e434a-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="e434a-110">Method</span></span>       | <span data-ttu-id="e434a-111">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="e434a-111">Return Type</span></span> | <span data-ttu-id="e434a-112">説明</span><span class="sxs-lookup"><span data-stu-id="e434a-112">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="e434a-113">OnPremisesPublishingProfile を取得する</span><span class="sxs-lookup"><span data-stu-id="e434a-113">Get onPremisesPublishingProfile</span></span>](../api/onpremisespublishingprofile-get.md) | [<span data-ttu-id="e434a-114">onPremisesPublishingProfile</span><span class="sxs-lookup"><span data-stu-id="e434a-114">onPremisesPublishingProfile</span></span>](onpremisespublishingprofile.md) | <span data-ttu-id="e434a-115">**OnPremisesPublishingProfile**オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="e434a-115">Read the properties and relationships of an **onPremisesPublishingProfile** object.</span></span> |
| [<span data-ttu-id="e434a-116">OnPremisesPublishingProfile の更新</span><span class="sxs-lookup"><span data-stu-id="e434a-116">Update onPremisesPublishingProfile</span></span>](../api/onpremisespublishingprofile-update.md) | <span data-ttu-id="e434a-117">None</span><span class="sxs-lookup"><span data-stu-id="e434a-117">None</span></span> | <span data-ttu-id="e434a-118">[OnPremisesPublishingProfile](onpremisespublishingprofile.md)オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="e434a-118">Update an [onPremisesPublishingProfile](onpremisespublishingprofile.md) object.</span></span>

## <a name="properties"></a><span data-ttu-id="e434a-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e434a-119">Properties</span></span>

| <span data-ttu-id="e434a-120">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e434a-120">Property</span></span>     | <span data-ttu-id="e434a-121">型</span><span class="sxs-lookup"><span data-stu-id="e434a-121">Type</span></span>        | <span data-ttu-id="e434a-122">説明</span><span class="sxs-lookup"><span data-stu-id="e434a-122">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="e434a-123">hybridAgentUpdaterConfiguration</span><span class="sxs-lookup"><span data-stu-id="e434a-123">hybridAgentUpdaterConfiguration</span></span>|[<span data-ttu-id="e434a-124">hybridAgentUpdaterConfiguration</span><span class="sxs-lookup"><span data-stu-id="e434a-124">hybridAgentUpdaterConfiguration</span></span>](hybridagentupdaterconfiguration.md)| <span data-ttu-id="e434a-125">**HybridAgentUpdaterConfiguration**オブジェクトを表します。</span><span class="sxs-lookup"><span data-stu-id="e434a-125">Represents a **hybridAgentUpdaterConfiguration** object.</span></span>|
|<span data-ttu-id="e434a-126">id</span><span class="sxs-lookup"><span data-stu-id="e434a-126">id</span></span>|<span data-ttu-id="e434a-127">String</span><span class="sxs-lookup"><span data-stu-id="e434a-127">String</span></span>| <span data-ttu-id="e434a-128">発行の種類を表します。</span><span class="sxs-lookup"><span data-stu-id="e434a-128">Represents a publishing type.</span></span> <span data-ttu-id="e434a-129">可能な値は、`appProxy`、`exchangeOnline`、`authentication`、`provisioning`、`adAdministration` です。</span><span class="sxs-lookup"><span data-stu-id="e434a-129">Possible values are: `appProxy`, `exchangeOnline`, `authentication`, `provisioning`, `adAdministration`.</span></span> <span data-ttu-id="e434a-130">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="e434a-130">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e434a-131">関係</span><span class="sxs-lookup"><span data-stu-id="e434a-131">Relationships</span></span>

| <span data-ttu-id="e434a-132">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="e434a-132">Relationship</span></span> | <span data-ttu-id="e434a-133">型</span><span class="sxs-lookup"><span data-stu-id="e434a-133">Type</span></span>        | <span data-ttu-id="e434a-134">説明</span><span class="sxs-lookup"><span data-stu-id="e434a-134">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="e434a-135">agentGroups</span><span class="sxs-lookup"><span data-stu-id="e434a-135">agentGroups</span></span>|<span data-ttu-id="e434a-136">[onPremisesAgentGroup](onpremisesagentgroup.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="e434a-136">[onPremisesAgentGroup](onpremisesagentgroup.md) collection</span></span>| <span data-ttu-id="e434a-137">既存の**onPremisesAgentGroup**オブジェクトのリスト。</span><span class="sxs-lookup"><span data-stu-id="e434a-137">List of existing **onPremisesAgentGroup** objects.</span></span> <span data-ttu-id="e434a-138">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="e434a-138">Read-only.</span></span> <span data-ttu-id="e434a-139">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="e434a-139">Nullable.</span></span>|
|<span data-ttu-id="e434a-140">エージェント</span><span class="sxs-lookup"><span data-stu-id="e434a-140">agents</span></span>|<span data-ttu-id="e434a-141">[onPremisesAgent](onpremisesagent.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="e434a-141">[onPremisesAgent](onpremisesagent.md) collection</span></span>| <span data-ttu-id="e434a-142">存在していた**onPremisesAgent**オブジェクトのリスト。</span><span class="sxs-lookup"><span data-stu-id="e434a-142">List of existed **onPremisesAgent** objects.</span></span> <span data-ttu-id="e434a-143">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="e434a-143">Read-only.</span></span> <span data-ttu-id="e434a-144">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="e434a-144">Nullable.</span></span>|
|<span data-ttu-id="e434a-145">publishedResources</span><span class="sxs-lookup"><span data-stu-id="e434a-145">publishedResources</span></span>|<span data-ttu-id="e434a-146">[Publishedresource](publishedresource.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="e434a-146">[publishedResource](publishedresource.md) collection</span></span>| <span data-ttu-id="e434a-147">既存の**Publishedresource**オブジェクトのリスト。</span><span class="sxs-lookup"><span data-stu-id="e434a-147">List of existing **publishedResource** objects.</span></span> <span data-ttu-id="e434a-148">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="e434a-148">Read-only.</span></span> <span data-ttu-id="e434a-149">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="e434a-149">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e434a-150">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e434a-150">JSON representation</span></span>

<span data-ttu-id="e434a-151">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e434a-151">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onPremisesPublishingProfile",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "hybridAgentUpdaterConfiguration": {"@odata.type": "microsoft.graph.hybridAgentUpdaterConfiguration"},
  "id": "String (identifier)"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onPremisesPublishingProfile resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
