---
title: managedAppPolicy リソースの種類
description: ManagedAppPolicy リソースは、プラットフォーム特有のポリシーの基本型を表します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c050415fc9402bdeb064ca6426bfe291e790940b
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34994749"
---
# <a name="managedapppolicy-resource-type"></a><span data-ttu-id="19139-103">managedAppPolicy リソースの種類</span><span class="sxs-lookup"><span data-stu-id="19139-103">managedAppPolicy resource type</span></span>

> <span data-ttu-id="19139-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="19139-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="19139-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="19139-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="19139-106">ManagedAppPolicy リソースは、プラットフォーム特有のポリシーの基本型を表します。</span><span class="sxs-lookup"><span data-stu-id="19139-106">The ManagedAppPolicy resource represents a base type for platform specific policies.</span></span>

## <a name="methods"></a><span data-ttu-id="19139-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="19139-107">Methods</span></span>
|<span data-ttu-id="19139-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="19139-108">Method</span></span>|<span data-ttu-id="19139-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="19139-109">Return Type</span></span>|<span data-ttu-id="19139-110">説明</span><span class="sxs-lookup"><span data-stu-id="19139-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="19139-111">List managedAppPolicies</span><span class="sxs-lookup"><span data-stu-id="19139-111">List managedAppPolicies</span></span>](../api/intune-mam-managedapppolicy-list.md)|<span data-ttu-id="19139-112">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="19139-112">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="19139-113">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="19139-113">List properties and relationships of the [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) objects.</span></span>|
|[<span data-ttu-id="19139-114">Get managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="19139-114">Get managedAppPolicy</span></span>](../api/intune-mam-managedapppolicy-get.md)|[<span data-ttu-id="19139-115">managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="19139-115">managedAppPolicy</span></span>](../resources/intune-mam-managedapppolicy.md)|<span data-ttu-id="19139-116">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="19139-116">Read properties and relationships of the [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) object.</span></span>|
|[<span data-ttu-id="19139-117">targetApps アクション</span><span class="sxs-lookup"><span data-stu-id="19139-117">targetApps action</span></span>](../api/intune-mam-managedapppolicy-targetapps.md)|<span data-ttu-id="19139-118">なし</span><span class="sxs-lookup"><span data-stu-id="19139-118">None</span></span>|<span data-ttu-id="19139-119">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="19139-119">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="19139-120">プロパティ</span><span class="sxs-lookup"><span data-stu-id="19139-120">Properties</span></span>
|<span data-ttu-id="19139-121">プロパティ</span><span class="sxs-lookup"><span data-stu-id="19139-121">Property</span></span>|<span data-ttu-id="19139-122">型</span><span class="sxs-lookup"><span data-stu-id="19139-122">Type</span></span>|<span data-ttu-id="19139-123">説明</span><span class="sxs-lookup"><span data-stu-id="19139-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="19139-124">displayName</span><span class="sxs-lookup"><span data-stu-id="19139-124">displayName</span></span>|<span data-ttu-id="19139-125">String</span><span class="sxs-lookup"><span data-stu-id="19139-125">String</span></span>|<span data-ttu-id="19139-126">ポリシーの表示名。</span><span class="sxs-lookup"><span data-stu-id="19139-126">Policy display name.</span></span>|
|<span data-ttu-id="19139-127">description</span><span class="sxs-lookup"><span data-stu-id="19139-127">description</span></span>|<span data-ttu-id="19139-128">String</span><span class="sxs-lookup"><span data-stu-id="19139-128">String</span></span>|<span data-ttu-id="19139-129">ポリシーの説明。</span><span class="sxs-lookup"><span data-stu-id="19139-129">The policy's description.</span></span>|
|<span data-ttu-id="19139-130">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="19139-130">createdDateTime</span></span>|<span data-ttu-id="19139-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="19139-131">DateTimeOffset</span></span>|<span data-ttu-id="19139-132">ポリシーが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="19139-132">The date and time the policy was created.</span></span>|
|<span data-ttu-id="19139-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="19139-133">lastModifiedDateTime</span></span>|<span data-ttu-id="19139-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="19139-134">DateTimeOffset</span></span>|<span data-ttu-id="19139-135">ポリシーが変更された最終日時。</span><span class="sxs-lookup"><span data-stu-id="19139-135">Last time the policy was modified.</span></span>|
|<span data-ttu-id="19139-136">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="19139-136">roleScopeTagIds</span></span>|<span data-ttu-id="19139-137">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="19139-137">String collection</span></span>|<span data-ttu-id="19139-138">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="19139-138">List of Scope Tags for this Entity instance.</span></span>|
|<span data-ttu-id="19139-139">id</span><span class="sxs-lookup"><span data-stu-id="19139-139">id</span></span>|<span data-ttu-id="19139-140">文字列</span><span class="sxs-lookup"><span data-stu-id="19139-140">String</span></span>|<span data-ttu-id="19139-141">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="19139-141">Key of the entity.</span></span>|
|<span data-ttu-id="19139-142">version</span><span class="sxs-lookup"><span data-stu-id="19139-142">version</span></span>|<span data-ttu-id="19139-143">String</span><span class="sxs-lookup"><span data-stu-id="19139-143">String</span></span>|<span data-ttu-id="19139-144">エンティティのバージョン。</span><span class="sxs-lookup"><span data-stu-id="19139-144">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="19139-145">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="19139-145">Relationships</span></span>
<span data-ttu-id="19139-146">なし</span><span class="sxs-lookup"><span data-stu-id="19139-146">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="19139-147">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="19139-147">JSON Representation</span></span>
<span data-ttu-id="19139-148">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="19139-148">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedAppPolicy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppPolicy",
  "displayName": "String",
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "roleScopeTagIds": [
    "String"
  ],
  "id": "String (identifier)",
  "version": "String"
}
```





