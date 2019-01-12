---
title: managedAppPolicyDeploymentSummary リソースの種類
description: ManagedAppEntity は、アプリ管理ワークフロー下にある他のすべてのエンティティ タイプの基本型です。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 4ded5ab6bfb4cbd744bfab9a614f3122c8d1ab53
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27957481"
---
# <a name="managedapppolicydeploymentsummary-resource-type"></a><span data-ttu-id="cb185-103">managedAppPolicyDeploymentSummary リソースの種類</span><span class="sxs-lookup"><span data-stu-id="cb185-103">managedAppPolicyDeploymentSummary resource type</span></span>

> <span data-ttu-id="cb185-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="cb185-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cb185-105">ManagedAppEntity は、アプリ管理ワークフロー下にある他のすべてのエンティティの種類の基本型です。</span><span class="sxs-lookup"><span data-stu-id="cb185-105">The ManagedAppEntity is the base entity type for all other entity types under app management workflow.</span></span>
## <a name="methods"></a><span data-ttu-id="cb185-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="cb185-106">Methods</span></span>
|<span data-ttu-id="cb185-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="cb185-107">Method</span></span>|<span data-ttu-id="cb185-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="cb185-108">Return Type</span></span>|<span data-ttu-id="cb185-109">説明</span><span class="sxs-lookup"><span data-stu-id="cb185-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="cb185-110">Get managedAppPolicyDeploymentSummary</span><span class="sxs-lookup"><span data-stu-id="cb185-110">Get managedAppPolicyDeploymentSummary</span></span>](../api/intune-mam-managedapppolicydeploymentsummary-get.md)|[<span data-ttu-id="cb185-111">managedAppPolicyDeploymentSummary</span><span class="sxs-lookup"><span data-stu-id="cb185-111">managedAppPolicyDeploymentSummary</span></span>](../resources/intune-mam-managedapppolicydeploymentsummary.md)|<span data-ttu-id="cb185-112">[managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="cb185-112">Read properties and relationships of the [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) object.</span></span>|
|[<span data-ttu-id="cb185-113">Update managedAppPolicyDeploymentSummary</span><span class="sxs-lookup"><span data-stu-id="cb185-113">Update managedAppPolicyDeploymentSummary</span></span>](../api/intune-mam-managedapppolicydeploymentsummary-update.md)|[<span data-ttu-id="cb185-114">managedAppPolicyDeploymentSummary</span><span class="sxs-lookup"><span data-stu-id="cb185-114">managedAppPolicyDeploymentSummary</span></span>](../resources/intune-mam-managedapppolicydeploymentsummary.md)|<span data-ttu-id="cb185-115">[managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="cb185-115">Update the properties of a [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="cb185-116">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cb185-116">Properties</span></span>
|<span data-ttu-id="cb185-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cb185-117">Property</span></span>|<span data-ttu-id="cb185-118">型</span><span class="sxs-lookup"><span data-stu-id="cb185-118">Type</span></span>|<span data-ttu-id="cb185-119">説明</span><span class="sxs-lookup"><span data-stu-id="cb185-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cb185-120">displayName</span><span class="sxs-lookup"><span data-stu-id="cb185-120">displayName</span></span>|<span data-ttu-id="cb185-121">String</span><span class="sxs-lookup"><span data-stu-id="cb185-121">String</span></span>|<span data-ttu-id="cb185-122">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="cb185-122">Not yet documented</span></span>|
|<span data-ttu-id="cb185-123">configurationDeployedUserCount</span><span class="sxs-lookup"><span data-stu-id="cb185-123">configurationDeployedUserCount</span></span>|<span data-ttu-id="cb185-124">Int32</span><span class="sxs-lookup"><span data-stu-id="cb185-124">Int32</span></span>|<span data-ttu-id="cb185-125">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="cb185-125">Not yet documented</span></span>|
|<span data-ttu-id="cb185-126">lastRefreshTime</span><span class="sxs-lookup"><span data-stu-id="cb185-126">lastRefreshTime</span></span>|<span data-ttu-id="cb185-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cb185-127">DateTimeOffset</span></span>|<span data-ttu-id="cb185-128">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="cb185-128">Not yet documented</span></span>|
|<span data-ttu-id="cb185-129">configurationDeploymentSummaryPerApp</span><span class="sxs-lookup"><span data-stu-id="cb185-129">configurationDeploymentSummaryPerApp</span></span>|<span data-ttu-id="cb185-130">[managedAppPolicyDeploymentSummaryPerApp](../resources/intune-mam-managedapppolicydeploymentsummaryperapp.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="cb185-130">[managedAppPolicyDeploymentSummaryPerApp](../resources/intune-mam-managedapppolicydeploymentsummaryperapp.md) collection</span></span>|<span data-ttu-id="cb185-131">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="cb185-131">Not yet documented</span></span>|
|<span data-ttu-id="cb185-132">id</span><span class="sxs-lookup"><span data-stu-id="cb185-132">id</span></span>|<span data-ttu-id="cb185-133">String</span><span class="sxs-lookup"><span data-stu-id="cb185-133">String</span></span>|<span data-ttu-id="cb185-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="cb185-134">Key of the entity.</span></span>|
|<span data-ttu-id="cb185-135">version</span><span class="sxs-lookup"><span data-stu-id="cb185-135">version</span></span>|<span data-ttu-id="cb185-136">String</span><span class="sxs-lookup"><span data-stu-id="cb185-136">String</span></span>|<span data-ttu-id="cb185-137">エンティティのバージョン。</span><span class="sxs-lookup"><span data-stu-id="cb185-137">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cb185-138">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="cb185-138">Relationships</span></span>
<span data-ttu-id="cb185-139">なし</span><span class="sxs-lookup"><span data-stu-id="cb185-139">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="cb185-140">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="cb185-140">JSON Representation</span></span>
<span data-ttu-id="cb185-141">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="cb185-141">Here is a JSON representation of the resource.</span></span>
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



