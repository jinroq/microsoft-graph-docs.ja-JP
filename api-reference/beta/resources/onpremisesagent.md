---
title: onPremisesAgent リソースの種類
description: onPremisesAgent リソースの種類。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 1bcff659cf30b946654f14190b2cf5f693d27bc4
ms.sourcegitcommit: 8844023e15b7649a5c03603aee243acf85930ef2
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/24/2019
ms.locfileid: "35841263"
---
# <a name="onpremisesagent-resource-type"></a><span data-ttu-id="8a58d-103">onPremisesAgent リソースの種類</span><span class="sxs-lookup"><span data-stu-id="8a58d-103">onPremisesAgent resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8a58d-104">オンプレミスのエージェントを表します。</span><span class="sxs-lookup"><span data-stu-id="8a58d-104">Represents on-premises agent.</span></span> <span data-ttu-id="8a58d-105">テナント管理者によってインストールされた社内エージェントは、発行された特定の[リソース](publishedresource.md)への要求にアクセスしたり、処理したりするように構成できます。</span><span class="sxs-lookup"><span data-stu-id="8a58d-105">On-premises agents installed by a tenant administrator can be configured to access/handle requests to a particular [published resource](publishedresource.md).</span></span>

## <a name="methods"></a><span data-ttu-id="8a58d-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="8a58d-106">Methods</span></span>

| <span data-ttu-id="8a58d-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="8a58d-107">Method</span></span>       | <span data-ttu-id="8a58d-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="8a58d-108">Return Type</span></span> | <span data-ttu-id="8a58d-109">説明</span><span class="sxs-lookup"><span data-stu-id="8a58d-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="8a58d-110">リスト onPremisesAgents</span><span class="sxs-lookup"><span data-stu-id="8a58d-110">List onPremisesAgents</span></span>](../api/onpremisesagent-list.md) | <span data-ttu-id="8a58d-111">[onPremisesAgent](onpremisesagent.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="8a58d-111">[onPremisesAgent](onpremisesagent.md) collection</span></span> | <span data-ttu-id="8a58d-112">**OnPremisesAgents**オブジェクトのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="8a58d-112">Get an **onPremisesAgents** object collection.</span></span> |
| [<span data-ttu-id="8a58d-113">OnPremisesAgent を取得する</span><span class="sxs-lookup"><span data-stu-id="8a58d-113">Get onPremisesAgent</span></span>](../api/onpremisesagent-get.md) | [<span data-ttu-id="8a58d-114">onPremisesAgent</span><span class="sxs-lookup"><span data-stu-id="8a58d-114">onPremisesAgent</span></span>](onpremisesagent.md) | <span data-ttu-id="8a58d-115">**OnPremisesAgent**オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="8a58d-115">Read the properties and relationships of an **onPremisesAgent** object.</span></span> |
| [<span data-ttu-id="8a58d-116">OnPremisesAgent を onPremisesAgentGroup に割り当てる</span><span class="sxs-lookup"><span data-stu-id="8a58d-116">Assign onPremisesAgent to onPremisesAgentGroup</span></span>](../api/onpremisesagent-post-agentgroups.md) | <span data-ttu-id="8a58d-117">None</span><span class="sxs-lookup"><span data-stu-id="8a58d-117">None</span></span> | <span data-ttu-id="8a58d-118">**OnPremisesAgent**を**onPremisesAgentGroup**に割り当てます。</span><span class="sxs-lookup"><span data-stu-id="8a58d-118">Assign an **onPremisesAgent** to an **onPremisesAgentGroup**.</span></span>|
| [<span data-ttu-id="8a58d-119">OnPremisesAgentGroup から onpremisesAgent を削除する</span><span class="sxs-lookup"><span data-stu-id="8a58d-119">Remove onpremisesAgent from an onPremisesAgentGroup</span></span>](../api/onpremisesagent-delete-agentgroups.md) | <span data-ttu-id="8a58d-120">None</span><span class="sxs-lookup"><span data-stu-id="8a58d-120">None</span></span> | <span data-ttu-id="8a58d-121">**OnPremisesAgentGroup**から**onPremisesAgent**を削除します。</span><span class="sxs-lookup"><span data-stu-id="8a58d-121">Remove an **onPremisesAgent** from an **onPremisesAgentGroup**.</span></span> |

## <a name="properties"></a><span data-ttu-id="8a58d-122">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8a58d-122">Properties</span></span>

| <span data-ttu-id="8a58d-123">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8a58d-123">Property</span></span>     | <span data-ttu-id="8a58d-124">型</span><span class="sxs-lookup"><span data-stu-id="8a58d-124">Type</span></span>        | <span data-ttu-id="8a58d-125">説明</span><span class="sxs-lookup"><span data-stu-id="8a58d-125">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="8a58d-126">externalIp</span><span class="sxs-lookup"><span data-stu-id="8a58d-126">externalIp</span></span>|<span data-ttu-id="8a58d-127">String</span><span class="sxs-lookup"><span data-stu-id="8a58d-127">String</span></span>|<span data-ttu-id="8a58d-128">エージェントコンピューターのサービスによって検出された外部 IP アドレス。</span><span class="sxs-lookup"><span data-stu-id="8a58d-128">The external IP address as detected by the service for the agent machine.</span></span> <span data-ttu-id="8a58d-129">読み取り専用</span><span class="sxs-lookup"><span data-stu-id="8a58d-129">Read-only</span></span>|
|<span data-ttu-id="8a58d-130">id</span><span class="sxs-lookup"><span data-stu-id="8a58d-130">id</span></span>|<span data-ttu-id="8a58d-131">文字列</span><span class="sxs-lookup"><span data-stu-id="8a58d-131">String</span></span>| <span data-ttu-id="8a58d-132">OnPremisesAgent のオブジェクト id。</span><span class="sxs-lookup"><span data-stu-id="8a58d-132">The object id of the onPremisesAgent.</span></span> <span data-ttu-id="8a58d-133">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="8a58d-133">Read-only.</span></span>|
|<span data-ttu-id="8a58d-134">マシン</span><span class="sxs-lookup"><span data-stu-id="8a58d-134">machineName</span></span>|<span data-ttu-id="8a58d-135">String</span><span class="sxs-lookup"><span data-stu-id="8a58d-135">String</span></span>|<span data-ttu-id="8a58d-136">Aggent が実行されているコンピューターの名前。</span><span class="sxs-lookup"><span data-stu-id="8a58d-136">The name of the machine that the aggent is running on.</span></span> <span data-ttu-id="8a58d-137">読み取り専用</span><span class="sxs-lookup"><span data-stu-id="8a58d-137">Read-only</span></span>|
|<span data-ttu-id="8a58d-138">status</span><span class="sxs-lookup"><span data-stu-id="8a58d-138">status</span></span>|<span data-ttu-id="8a58d-139">string</span><span class="sxs-lookup"><span data-stu-id="8a58d-139">string</span></span>| <span data-ttu-id="8a58d-140">可能な値は、`active`、`inactive` です。</span><span class="sxs-lookup"><span data-stu-id="8a58d-140">Possible values are: `active`, `inactive`.</span></span>|
|<span data-ttu-id="8a58d-141">発行の種類</span><span class="sxs-lookup"><span data-stu-id="8a58d-141">publishingType</span></span>|<span data-ttu-id="8a58d-142">string</span><span class="sxs-lookup"><span data-stu-id="8a58d-142">string</span></span>| <span data-ttu-id="8a58d-143">可能な値は、`appProxy`、`exchangeOnline`、`authentication`、`provisioning`、`adAdministration` です。</span><span class="sxs-lookup"><span data-stu-id="8a58d-143">Possible values are: `appProxy`, `exchangeOnline`, `authentication`, `provisioning`, `adAdministration`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8a58d-144">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="8a58d-144">Relationships</span></span>

| <span data-ttu-id="8a58d-145">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="8a58d-145">Relationship</span></span> | <span data-ttu-id="8a58d-146">型</span><span class="sxs-lookup"><span data-stu-id="8a58d-146">Type</span></span>        | <span data-ttu-id="8a58d-147">説明</span><span class="sxs-lookup"><span data-stu-id="8a58d-147">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="8a58d-148">agentGroups</span><span class="sxs-lookup"><span data-stu-id="8a58d-148">agentGroups</span></span>|<span data-ttu-id="8a58d-149">[onPremisesAgentGroup](onpremisesagentgroup.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="8a58d-149">[onPremisesAgentGroup](onpremisesagentgroup.md) collection</span></span>| <span data-ttu-id="8a58d-150">**OnPremisesAgent**が割り当てられている**onPremisesAgentGroups**のリスト。</span><span class="sxs-lookup"><span data-stu-id="8a58d-150">List of **onPremisesAgentGroups** that an **onPremisesAgent** is assigned to.</span></span> <span data-ttu-id="8a58d-151">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="8a58d-151">Read-only.</span></span> <span data-ttu-id="8a58d-152">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="8a58d-152">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8a58d-153">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="8a58d-153">JSON representation</span></span>

<span data-ttu-id="8a58d-154">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="8a58d-154">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onPremisesAgent",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "externalIp": "String",
  "id": "String (identifier)",
  "machineName": "String",
  "status": "string",
  "supportedPublishingTypes": ["string"]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onPremisesAgent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
