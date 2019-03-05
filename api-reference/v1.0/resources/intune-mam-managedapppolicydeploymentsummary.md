---
title: managedAppPolicyDeploymentSummary リソースの種類
description: ManagedAppEntity は、アプリ管理ワークフロー下にある他のすべてのエンティティ タイプの基本型です。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 84ca52db1321bc3a2fa356de50e1446f662e725b
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30256372"
---
# <a name="managedapppolicydeploymentsummary-resource-type"></a><span data-ttu-id="38726-103">managedAppPolicyDeploymentSummary リソースの種類</span><span class="sxs-lookup"><span data-stu-id="38726-103">managedAppPolicyDeploymentSummary resource type</span></span>

> <span data-ttu-id="38726-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="38726-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="38726-105">ManagedAppEntity は、アプリ管理ワークフロー下にある他のすべてのエンティティの種類の基本型です。</span><span class="sxs-lookup"><span data-stu-id="38726-105">The ManagedAppEntity is the base entity type for all other entity types under app management workflow.</span></span>

## <a name="methods"></a><span data-ttu-id="38726-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="38726-106">Methods</span></span>
|<span data-ttu-id="38726-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="38726-107">Method</span></span>|<span data-ttu-id="38726-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="38726-108">Return Type</span></span>|<span data-ttu-id="38726-109">説明</span><span class="sxs-lookup"><span data-stu-id="38726-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="38726-110">Get managedAppPolicyDeploymentSummary</span><span class="sxs-lookup"><span data-stu-id="38726-110">Get managedAppPolicyDeploymentSummary</span></span>](../api/intune-mam-managedapppolicydeploymentsummary-get.md)|[<span data-ttu-id="38726-111">managedAppPolicyDeploymentSummary</span><span class="sxs-lookup"><span data-stu-id="38726-111">managedAppPolicyDeploymentSummary</span></span>](../resources/intune-mam-managedapppolicydeploymentsummary.md)|<span data-ttu-id="38726-112">[managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="38726-112">Read properties and relationships of the [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) object.</span></span>|
|[<span data-ttu-id="38726-113">Update managedAppPolicyDeploymentSummary</span><span class="sxs-lookup"><span data-stu-id="38726-113">Update managedAppPolicyDeploymentSummary</span></span>](../api/intune-mam-managedapppolicydeploymentsummary-update.md)|[<span data-ttu-id="38726-114">managedAppPolicyDeploymentSummary</span><span class="sxs-lookup"><span data-stu-id="38726-114">managedAppPolicyDeploymentSummary</span></span>](../resources/intune-mam-managedapppolicydeploymentsummary.md)|<span data-ttu-id="38726-115">[managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="38726-115">Update the properties of a [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="38726-116">プロパティ</span><span class="sxs-lookup"><span data-stu-id="38726-116">Properties</span></span>
|<span data-ttu-id="38726-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="38726-117">Property</span></span>|<span data-ttu-id="38726-118">型</span><span class="sxs-lookup"><span data-stu-id="38726-118">Type</span></span>|<span data-ttu-id="38726-119">説明</span><span class="sxs-lookup"><span data-stu-id="38726-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="38726-120">displayName</span><span class="sxs-lookup"><span data-stu-id="38726-120">displayName</span></span>|<span data-ttu-id="38726-121">String</span><span class="sxs-lookup"><span data-stu-id="38726-121">String</span></span>|<span data-ttu-id="38726-122">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="38726-122">Not yet documented</span></span>|
|<span data-ttu-id="38726-123">configurationDeployedUserCount</span><span class="sxs-lookup"><span data-stu-id="38726-123">configurationDeployedUserCount</span></span>|<span data-ttu-id="38726-124">Int32</span><span class="sxs-lookup"><span data-stu-id="38726-124">Int32</span></span>|<span data-ttu-id="38726-125">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="38726-125">Not yet documented</span></span>|
|<span data-ttu-id="38726-126">lastRefreshTime</span><span class="sxs-lookup"><span data-stu-id="38726-126">lastRefreshTime</span></span>|<span data-ttu-id="38726-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="38726-127">DateTimeOffset</span></span>|<span data-ttu-id="38726-128">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="38726-128">Not yet documented</span></span>|
|<span data-ttu-id="38726-129">configurationDeploymentSummaryPerApp</span><span class="sxs-lookup"><span data-stu-id="38726-129">configurationDeploymentSummaryPerApp</span></span>|<span data-ttu-id="38726-130">[managedAppPolicyDeploymentSummaryPerApp](../resources/intune-mam-managedapppolicydeploymentsummaryperapp.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="38726-130">[managedAppPolicyDeploymentSummaryPerApp](../resources/intune-mam-managedapppolicydeploymentsummaryperapp.md) collection</span></span>|<span data-ttu-id="38726-131">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="38726-131">Not yet documented</span></span>|
|<span data-ttu-id="38726-132">id</span><span class="sxs-lookup"><span data-stu-id="38726-132">id</span></span>|<span data-ttu-id="38726-133">文字列</span><span class="sxs-lookup"><span data-stu-id="38726-133">String</span></span>|<span data-ttu-id="38726-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="38726-134">Key of the entity.</span></span>|
|<span data-ttu-id="38726-135">version</span><span class="sxs-lookup"><span data-stu-id="38726-135">version</span></span>|<span data-ttu-id="38726-136">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="38726-136">String</span></span>|<span data-ttu-id="38726-137">エンティティのバージョン。</span><span class="sxs-lookup"><span data-stu-id="38726-137">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="38726-138">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="38726-138">Relationships</span></span>
<span data-ttu-id="38726-139">なし</span><span class="sxs-lookup"><span data-stu-id="38726-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="38726-140">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="38726-140">JSON Representation</span></span>
<span data-ttu-id="38726-141">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="38726-141">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedAppPolicyDeploymentSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppPolicyDeploymentSummary",
  "displayName": "String",
  "configurationDeployedUserCount": 1024,
  "lastRefreshTime": "String (timestamp)",
  "configurationDeploymentSummaryPerApp": [
    {
      "@odata.type": "microsoft.graph.managedAppPolicyDeploymentSummaryPerApp",
      "mobileAppIdentifier": {
        "@odata.type": "microsoft.graph.androidMobileAppIdentifier",
        "packageId": "String"
      },
      "configurationAppliedUserCount": 1024
    }
  ],
  "id": "String (identifier)",
  "version": "String"
}
```



