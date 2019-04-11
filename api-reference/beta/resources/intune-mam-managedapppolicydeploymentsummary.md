---
title: managedAppPolicyDeploymentSummary リソースの種類
description: ManagedAppEntity は、アプリ管理ワークフロー下にある他のすべてのエンティティ タイプの基本型です。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8ad282723cf32602f626b92d65d6e023c4995596
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31784489"
---
# <a name="managedapppolicydeploymentsummary-resource-type"></a><span data-ttu-id="87e59-103">managedAppPolicyDeploymentSummary リソースの種類</span><span class="sxs-lookup"><span data-stu-id="87e59-103">managedAppPolicyDeploymentSummary resource type</span></span>

> <span data-ttu-id="87e59-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="87e59-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="87e59-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="87e59-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="87e59-106">ManagedAppEntity は、アプリ管理ワークフロー下にある他のすべてのエンティティの種類の基本型です。</span><span class="sxs-lookup"><span data-stu-id="87e59-106">The ManagedAppEntity is the base entity type for all other entity types under app management workflow.</span></span>

## <a name="methods"></a><span data-ttu-id="87e59-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="87e59-107">Methods</span></span>
|<span data-ttu-id="87e59-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="87e59-108">Method</span></span>|<span data-ttu-id="87e59-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="87e59-109">Return Type</span></span>|<span data-ttu-id="87e59-110">説明</span><span class="sxs-lookup"><span data-stu-id="87e59-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="87e59-111">managedAppPolicyDeploymentSummary の取得</span><span class="sxs-lookup"><span data-stu-id="87e59-111">Get managedAppPolicyDeploymentSummary</span></span>](../api/intune-mam-managedapppolicydeploymentsummary-get.md)|[<span data-ttu-id="87e59-112">managedAppPolicyDeploymentSummary</span><span class="sxs-lookup"><span data-stu-id="87e59-112">managedAppPolicyDeploymentSummary</span></span>](../resources/intune-mam-managedapppolicydeploymentsummary.md)|<span data-ttu-id="87e59-113">[managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="87e59-113">Read properties and relationships of the [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) object.</span></span>|
|[<span data-ttu-id="87e59-114">managedAppPolicyDeploymentSummary の更新</span><span class="sxs-lookup"><span data-stu-id="87e59-114">Update managedAppPolicyDeploymentSummary</span></span>](../api/intune-mam-managedapppolicydeploymentsummary-update.md)|[<span data-ttu-id="87e59-115">managedAppPolicyDeploymentSummary</span><span class="sxs-lookup"><span data-stu-id="87e59-115">managedAppPolicyDeploymentSummary</span></span>](../resources/intune-mam-managedapppolicydeploymentsummary.md)|<span data-ttu-id="87e59-116">[managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="87e59-116">Update the properties of a [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="87e59-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="87e59-117">Properties</span></span>
|<span data-ttu-id="87e59-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="87e59-118">Property</span></span>|<span data-ttu-id="87e59-119">型</span><span class="sxs-lookup"><span data-stu-id="87e59-119">Type</span></span>|<span data-ttu-id="87e59-120">説明</span><span class="sxs-lookup"><span data-stu-id="87e59-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="87e59-121">displayName</span><span class="sxs-lookup"><span data-stu-id="87e59-121">displayName</span></span>|<span data-ttu-id="87e59-122">String</span><span class="sxs-lookup"><span data-stu-id="87e59-122">String</span></span>|<span data-ttu-id="87e59-123">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="87e59-123">Not yet documented</span></span>|
|<span data-ttu-id="87e59-124">configurationDeployedUserCount</span><span class="sxs-lookup"><span data-stu-id="87e59-124">configurationDeployedUserCount</span></span>|<span data-ttu-id="87e59-125">Int32</span><span class="sxs-lookup"><span data-stu-id="87e59-125">Int32</span></span>|<span data-ttu-id="87e59-126">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="87e59-126">Not yet documented</span></span>|
|<span data-ttu-id="87e59-127">lastRefreshTime</span><span class="sxs-lookup"><span data-stu-id="87e59-127">lastRefreshTime</span></span>|<span data-ttu-id="87e59-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="87e59-128">DateTimeOffset</span></span>|<span data-ttu-id="87e59-129">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="87e59-129">Not yet documented</span></span>|
|<span data-ttu-id="87e59-130">configurationDeploymentSummaryPerApp</span><span class="sxs-lookup"><span data-stu-id="87e59-130">configurationDeploymentSummaryPerApp</span></span>|<span data-ttu-id="87e59-131">[managedAppPolicyDeploymentSummaryPerApp](../resources/intune-mam-managedapppolicydeploymentsummaryperapp.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="87e59-131">[managedAppPolicyDeploymentSummaryPerApp](../resources/intune-mam-managedapppolicydeploymentsummaryperapp.md) collection</span></span>|<span data-ttu-id="87e59-132">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="87e59-132">Not yet documented</span></span>|
|<span data-ttu-id="87e59-133">id</span><span class="sxs-lookup"><span data-stu-id="87e59-133">id</span></span>|<span data-ttu-id="87e59-134">String</span><span class="sxs-lookup"><span data-stu-id="87e59-134">String</span></span>|<span data-ttu-id="87e59-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="87e59-135">Key of the entity.</span></span>|
|<span data-ttu-id="87e59-136">version</span><span class="sxs-lookup"><span data-stu-id="87e59-136">version</span></span>|<span data-ttu-id="87e59-137">String</span><span class="sxs-lookup"><span data-stu-id="87e59-137">String</span></span>|<span data-ttu-id="87e59-138">エンティティのバージョン。</span><span class="sxs-lookup"><span data-stu-id="87e59-138">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="87e59-139">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="87e59-139">Relationships</span></span>
<span data-ttu-id="87e59-140">なし</span><span class="sxs-lookup"><span data-stu-id="87e59-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="87e59-141">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="87e59-141">JSON Representation</span></span>
<span data-ttu-id="87e59-142">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="87e59-142">Here is a JSON representation of the resource.</span></span>
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





