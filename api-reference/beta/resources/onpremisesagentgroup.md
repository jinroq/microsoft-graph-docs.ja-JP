---
title: onPremisesAgentGroup リソースの種類
description: onPremisesAgentGroup リソースの種類。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 9e74a49a9a8c4b57232ed90cef232fa8b7feb998
ms.sourcegitcommit: 8844023e15b7649a5c03603aee243acf85930ef2
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/24/2019
ms.locfileid: "35841319"
---
# <a name="onpremisesagentgroup-resource-type"></a><span data-ttu-id="0c159-103">onPremisesAgentGroup リソースの種類</span><span class="sxs-lookup"><span data-stu-id="0c159-103">onPremisesAgentGroup resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0c159-104">オンプレミスのエージェントグループを表します。</span><span class="sxs-lookup"><span data-stu-id="0c159-104">Represents on-premises agents group.</span></span> <span data-ttu-id="0c159-105">エージェントグループを使用すると、テナント管理者は特定の[エージェント](onpremisesagent.md)を割り当てて、発行された特定[の社内リソース](publishedresource.md)を提供できます。</span><span class="sxs-lookup"><span data-stu-id="0c159-105">Agent groups enable a tenant admin to assign specific [agents](onpremisesagent.md) to serve specific [published on-premises resources](publishedresource.md).</span></span>

## <a name="methods"></a><span data-ttu-id="0c159-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="0c159-106">Methods</span></span>

| <span data-ttu-id="0c159-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="0c159-107">Method</span></span>       | <span data-ttu-id="0c159-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="0c159-108">Return Type</span></span> | <span data-ttu-id="0c159-109">説明</span><span class="sxs-lookup"><span data-stu-id="0c159-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="0c159-110">リスト onPremisesAgentGroups</span><span class="sxs-lookup"><span data-stu-id="0c159-110">List onPremisesAgentGroups</span></span>](../api/onpremisesagentgroup-list.md) | <span data-ttu-id="0c159-111">onPremisesAgentGroups コレクション</span><span class="sxs-lookup"><span data-stu-id="0c159-111">onPremisesAgentGroups collection</span></span> | <span data-ttu-id="0c159-112">**OnPremisesAgentGroup** objects コレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="0c159-112">Get an **onPremisesAgentGroup** objects collection.</span></span> |
| [<span data-ttu-id="0c159-113">OnPremisesAgentGroup を取得する</span><span class="sxs-lookup"><span data-stu-id="0c159-113">Get onPremisesAgentGroup</span></span>](../api/onpremisesagentgroup-get.md) | [<span data-ttu-id="0c159-114">onPremisesAgentGroup</span><span class="sxs-lookup"><span data-stu-id="0c159-114">onPremisesAgentGroup</span></span>](onpremisesagentgroup.md) | <span data-ttu-id="0c159-115">**OnPremisesAgentGroup**オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="0c159-115">Read the properties and relationships of an **onPremisesAgentGroup** object.</span></span> |
| [<span data-ttu-id="0c159-116">OnPremisesAgentGroup を作成する</span><span class="sxs-lookup"><span data-stu-id="0c159-116">Create onPremisesAgentGroup</span></span>](../api/onpremisesagentgroup-post.md)  | [<span data-ttu-id="0c159-117">onPremisesAgentGroup</span><span class="sxs-lookup"><span data-stu-id="0c159-117">onPremisesAgentGroup</span></span>](onpremisesagentgroup.md) | <span data-ttu-id="0c159-118">新しい**onPremisesAgentGroup**を作成します。</span><span class="sxs-lookup"><span data-stu-id="0c159-118">Create a new **onPremisesAgentGroup**.</span></span> |
| [<span data-ttu-id="0c159-119">OnPremisesAgentGroup の更新</span><span class="sxs-lookup"><span data-stu-id="0c159-119">Update onPremisesAgentGroup</span></span>](../api/onpremisesagentgroup-update.md) | [<span data-ttu-id="0c159-120">onPremisesAgentGroup</span><span class="sxs-lookup"><span data-stu-id="0c159-120">onPremisesAgentGroup</span></span>](onpremisesagentgroup.md) | <span data-ttu-id="0c159-121">**OnPremisesAgentGroup**オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="0c159-121">Update an **onPremisesAgentGroup** object.</span></span> |
| [<span data-ttu-id="0c159-122">OnPremisesAgentGroup の削除</span><span class="sxs-lookup"><span data-stu-id="0c159-122">Delete  onPremisesAgentGroup</span></span>](../api/onpremisesagentgroup-delete.md) | <span data-ttu-id="0c159-123">None</span><span class="sxs-lookup"><span data-stu-id="0c159-123">None</span></span> | <span data-ttu-id="0c159-124">**OnPremisesAgentGroup**オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="0c159-124">Delete an **onPremisesAgentGroup** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="0c159-125">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0c159-125">Properties</span></span>

| <span data-ttu-id="0c159-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0c159-126">Property</span></span>     | <span data-ttu-id="0c159-127">型</span><span class="sxs-lookup"><span data-stu-id="0c159-127">Type</span></span>        | <span data-ttu-id="0c159-128">説明</span><span class="sxs-lookup"><span data-stu-id="0c159-128">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="0c159-129">displayName</span><span class="sxs-lookup"><span data-stu-id="0c159-129">displayName</span></span>|<span data-ttu-id="0c159-130">String</span><span class="sxs-lookup"><span data-stu-id="0c159-130">String</span></span>|<span data-ttu-id="0c159-131">**OnPremisesAgentGroup**の表示名。</span><span class="sxs-lookup"><span data-stu-id="0c159-131">Display name of the **onPremisesAgentGroup**.</span></span>|
|<span data-ttu-id="0c159-132">id</span><span class="sxs-lookup"><span data-stu-id="0c159-132">id</span></span>|<span data-ttu-id="0c159-133">文字列</span><span class="sxs-lookup"><span data-stu-id="0c159-133">String</span></span>| <span data-ttu-id="0c159-134">**OnPremisesAgentGroup**のオブジェクト ID。</span><span class="sxs-lookup"><span data-stu-id="0c159-134">The object ID of the **onPremisesAgentGroup**.</span></span> <span data-ttu-id="0c159-135">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="0c159-135">Read-only.</span></span>|
|<span data-ttu-id="0c159-136">isDefault</span><span class="sxs-lookup"><span data-stu-id="0c159-136">isDefault</span></span>|<span data-ttu-id="0c159-137">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="0c159-137">Boolean</span></span>|<span data-ttu-id="0c159-138">**OnPremisesAgentGroup**が既定のエージェントグループであるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="0c159-138">Indicates if the **onPremisesAgentGroup** is the default agent group.</span></span> <span data-ttu-id="0c159-139">既定の**onPremisesAgentGroup**にすることができ、システムによって設定されるのは、1つのエージェントグループのみです。</span><span class="sxs-lookup"><span data-stu-id="0c159-139">Only a single agent group can be the default **onPremisesAgentGroup** and is set by the system.</span></span>|
|<span data-ttu-id="0c159-140">発行の種類</span><span class="sxs-lookup"><span data-stu-id="0c159-140">publishingType</span></span>|<span data-ttu-id="0c159-141">string</span><span class="sxs-lookup"><span data-stu-id="0c159-141">string</span></span>| <span data-ttu-id="0c159-142">可能な値は、`appProxy`、`exchangeOnline`、`authentication`、`provisioning`、`adAdministration` です。</span><span class="sxs-lookup"><span data-stu-id="0c159-142">Possible values are: `appProxy`, `exchangeOnline`, `authentication`, `provisioning`, `adAdministration`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0c159-143">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="0c159-143">Relationships</span></span>

| <span data-ttu-id="0c159-144">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="0c159-144">Relationship</span></span> | <span data-ttu-id="0c159-145">型</span><span class="sxs-lookup"><span data-stu-id="0c159-145">Type</span></span>        | <span data-ttu-id="0c159-146">説明</span><span class="sxs-lookup"><span data-stu-id="0c159-146">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="0c159-147">エージェント</span><span class="sxs-lookup"><span data-stu-id="0c159-147">agents</span></span>|<span data-ttu-id="0c159-148">[onPremisesAgent](onpremisesagent.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="0c159-148">[onPremisesAgent](onpremisesagent.md) collection</span></span>| <span data-ttu-id="0c159-149">**OnPremisesAgentGroup**に割り当てられている**onPremisesAgent**のリスト。</span><span class="sxs-lookup"><span data-stu-id="0c159-149">List of **onPremisesAgent** that are assigned to an **onPremisesAgentGroup**.</span></span> <span data-ttu-id="0c159-150">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="0c159-150">Read-only.</span></span> <span data-ttu-id="0c159-151">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="0c159-151">Nullable.</span></span>|
|<span data-ttu-id="0c159-152">publishedResources</span><span class="sxs-lookup"><span data-stu-id="0c159-152">publishedResources</span></span>|<span data-ttu-id="0c159-153">[Publishedresource](publishedresource.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="0c159-153">[publishedResource](publishedresource.md) collection</span></span>| <span data-ttu-id="0c159-154">**OnPremisesAgentGroup**に割り当てられている**publishedresource**のリスト。</span><span class="sxs-lookup"><span data-stu-id="0c159-154">List of **publishedResource** that are assigned to an **onPremisesAgentGroup**.</span></span> <span data-ttu-id="0c159-155">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="0c159-155">Read-only.</span></span> <span data-ttu-id="0c159-156">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="0c159-156">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0c159-157">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0c159-157">JSON representation</span></span>

<span data-ttu-id="0c159-158">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="0c159-158">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onPremisesAgentGroup",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "displayName": "String",
  "id": "String (identifier)",
  "isDefault": true,
  "publishingType": "string"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onPremisesAgentGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
