---
title: managedAppPolicy リソースの種類
description: ManagedAppPolicy リソースは、プラットフォーム特有のポリシーの基本型を表します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 6bc4a7bbc4bc0dc85da8759ad95162712b1deb13
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29422979"
---
# <a name="managedapppolicy-resource-type"></a><span data-ttu-id="2b722-103">managedAppPolicy リソースの種類</span><span class="sxs-lookup"><span data-stu-id="2b722-103">managedAppPolicy resource type</span></span>

> <span data-ttu-id="2b722-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="2b722-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="2b722-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2b722-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2b722-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="2b722-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2b722-107">ManagedAppPolicy リソースは、プラットフォーム特有のポリシーの基本型を表します。</span><span class="sxs-lookup"><span data-stu-id="2b722-107">The ManagedAppPolicy resource represents a base type for platform specific policies.</span></span>

## <a name="methods"></a><span data-ttu-id="2b722-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="2b722-108">Methods</span></span>
|<span data-ttu-id="2b722-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="2b722-109">Method</span></span>|<span data-ttu-id="2b722-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="2b722-110">Return Type</span></span>|<span data-ttu-id="2b722-111">説明</span><span class="sxs-lookup"><span data-stu-id="2b722-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="2b722-112">List managedAppPolicies</span><span class="sxs-lookup"><span data-stu-id="2b722-112">List managedAppPolicies</span></span>](../api/intune-mam-managedapppolicy-list.md)|<span data-ttu-id="2b722-113">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="2b722-113">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="2b722-114">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="2b722-114">List properties and relationships of the [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) objects.</span></span>|
|[<span data-ttu-id="2b722-115">Get managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="2b722-115">Get managedAppPolicy</span></span>](../api/intune-mam-managedapppolicy-get.md)|[<span data-ttu-id="2b722-116">managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="2b722-116">managedAppPolicy</span></span>](../resources/intune-mam-managedapppolicy.md)|<span data-ttu-id="2b722-117">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="2b722-117">Read properties and relationships of the [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) object.</span></span>|
|[<span data-ttu-id="2b722-118">targetApps アクション</span><span class="sxs-lookup"><span data-stu-id="2b722-118">targetApps action</span></span>](../api/intune-mam-managedapppolicy-targetapps.md)|<span data-ttu-id="2b722-119">なし</span><span class="sxs-lookup"><span data-stu-id="2b722-119">None</span></span>|<span data-ttu-id="2b722-120">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="2b722-120">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="2b722-121">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2b722-121">Properties</span></span>
|<span data-ttu-id="2b722-122">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2b722-122">Property</span></span>|<span data-ttu-id="2b722-123">型</span><span class="sxs-lookup"><span data-stu-id="2b722-123">Type</span></span>|<span data-ttu-id="2b722-124">説明</span><span class="sxs-lookup"><span data-stu-id="2b722-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2b722-125">displayName</span><span class="sxs-lookup"><span data-stu-id="2b722-125">displayName</span></span>|<span data-ttu-id="2b722-126">String</span><span class="sxs-lookup"><span data-stu-id="2b722-126">String</span></span>|<span data-ttu-id="2b722-127">ポリシーの表示名。</span><span class="sxs-lookup"><span data-stu-id="2b722-127">Policy display name.</span></span>|
|<span data-ttu-id="2b722-128">説明</span><span class="sxs-lookup"><span data-stu-id="2b722-128">description</span></span>|<span data-ttu-id="2b722-129">String</span><span class="sxs-lookup"><span data-stu-id="2b722-129">String</span></span>|<span data-ttu-id="2b722-130">ポリシーの説明。</span><span class="sxs-lookup"><span data-stu-id="2b722-130">The policy's description.</span></span>|
|<span data-ttu-id="2b722-131">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2b722-131">createdDateTime</span></span>|<span data-ttu-id="2b722-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2b722-132">DateTimeOffset</span></span>|<span data-ttu-id="2b722-133">ポリシーが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="2b722-133">The date and time the policy was created.</span></span>|
|<span data-ttu-id="2b722-134">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2b722-134">lastModifiedDateTime</span></span>|<span data-ttu-id="2b722-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2b722-135">DateTimeOffset</span></span>|<span data-ttu-id="2b722-136">ポリシーが変更された最終日時。</span><span class="sxs-lookup"><span data-stu-id="2b722-136">Last time the policy was modified.</span></span>|
|<span data-ttu-id="2b722-137">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="2b722-137">roleScopeTagIds</span></span>|<span data-ttu-id="2b722-138">String コレクション</span><span class="sxs-lookup"><span data-stu-id="2b722-138">String collection</span></span>|<span data-ttu-id="2b722-139">このエンティティ インスタンスのスコープのタグのリストです。</span><span class="sxs-lookup"><span data-stu-id="2b722-139">List of Scope Tags for this Entity instance.</span></span>|
|<span data-ttu-id="2b722-140">id</span><span class="sxs-lookup"><span data-stu-id="2b722-140">id</span></span>|<span data-ttu-id="2b722-141">String</span><span class="sxs-lookup"><span data-stu-id="2b722-141">String</span></span>|<span data-ttu-id="2b722-142">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="2b722-142">Key of the entity.</span></span>|
|<span data-ttu-id="2b722-143">version</span><span class="sxs-lookup"><span data-stu-id="2b722-143">version</span></span>|<span data-ttu-id="2b722-144">String</span><span class="sxs-lookup"><span data-stu-id="2b722-144">String</span></span>|<span data-ttu-id="2b722-145">エンティティのバージョン。</span><span class="sxs-lookup"><span data-stu-id="2b722-145">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2b722-146">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="2b722-146">Relationships</span></span>
<span data-ttu-id="2b722-147">なし</span><span class="sxs-lookup"><span data-stu-id="2b722-147">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2b722-148">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="2b722-148">JSON Representation</span></span>
<span data-ttu-id="2b722-149">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="2b722-149">Here is a JSON representation of the resource.</span></span>
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




