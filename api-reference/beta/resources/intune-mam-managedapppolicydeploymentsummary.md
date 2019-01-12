---
title: managedAppPolicyDeploymentSummary リソースの種類
description: ManagedAppEntity は、アプリ管理ワークフロー下にある他のすべてのエンティティ タイプの基本型です。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 4ab34deb28349e1860d4970c14171efedf44267f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27976339"
---
# <a name="managedapppolicydeploymentsummary-resource-type"></a><span data-ttu-id="e99b1-103">managedAppPolicyDeploymentSummary リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e99b1-103">managedAppPolicyDeploymentSummary resource type</span></span>

> <span data-ttu-id="e99b1-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="e99b1-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e99b1-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e99b1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e99b1-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="e99b1-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e99b1-107">ManagedAppEntity は、アプリ管理ワークフロー下にある他のすべてのエンティティの種類の基本型です。</span><span class="sxs-lookup"><span data-stu-id="e99b1-107">The ManagedAppEntity is the base entity type for all other entity types under app management workflow.</span></span>
## <a name="methods"></a><span data-ttu-id="e99b1-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="e99b1-108">Methods</span></span>
|<span data-ttu-id="e99b1-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="e99b1-109">Method</span></span>|<span data-ttu-id="e99b1-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="e99b1-110">Return Type</span></span>|<span data-ttu-id="e99b1-111">説明</span><span class="sxs-lookup"><span data-stu-id="e99b1-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="e99b1-112">Get managedAppPolicyDeploymentSummary</span><span class="sxs-lookup"><span data-stu-id="e99b1-112">Get managedAppPolicyDeploymentSummary</span></span>](../api/intune-mam-managedapppolicydeploymentsummary-get.md)|[<span data-ttu-id="e99b1-113">managedAppPolicyDeploymentSummary</span><span class="sxs-lookup"><span data-stu-id="e99b1-113">managedAppPolicyDeploymentSummary</span></span>](../resources/intune-mam-managedapppolicydeploymentsummary.md)|<span data-ttu-id="e99b1-114">[managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="e99b1-114">Read properties and relationships of the [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) object.</span></span>|
|[<span data-ttu-id="e99b1-115">Update managedAppPolicyDeploymentSummary</span><span class="sxs-lookup"><span data-stu-id="e99b1-115">Update managedAppPolicyDeploymentSummary</span></span>](../api/intune-mam-managedapppolicydeploymentsummary-update.md)|[<span data-ttu-id="e99b1-116">managedAppPolicyDeploymentSummary</span><span class="sxs-lookup"><span data-stu-id="e99b1-116">managedAppPolicyDeploymentSummary</span></span>](../resources/intune-mam-managedapppolicydeploymentsummary.md)|<span data-ttu-id="e99b1-117">[managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="e99b1-117">Update the properties of a [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="e99b1-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e99b1-118">Properties</span></span>
|<span data-ttu-id="e99b1-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e99b1-119">Property</span></span>|<span data-ttu-id="e99b1-120">型</span><span class="sxs-lookup"><span data-stu-id="e99b1-120">Type</span></span>|<span data-ttu-id="e99b1-121">説明</span><span class="sxs-lookup"><span data-stu-id="e99b1-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e99b1-122">displayName</span><span class="sxs-lookup"><span data-stu-id="e99b1-122">displayName</span></span>|<span data-ttu-id="e99b1-123">String</span><span class="sxs-lookup"><span data-stu-id="e99b1-123">String</span></span>|<span data-ttu-id="e99b1-124">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="e99b1-124">Not yet documented</span></span>|
|<span data-ttu-id="e99b1-125">configurationDeployedUserCount</span><span class="sxs-lookup"><span data-stu-id="e99b1-125">configurationDeployedUserCount</span></span>|<span data-ttu-id="e99b1-126">Int32</span><span class="sxs-lookup"><span data-stu-id="e99b1-126">Int32</span></span>|<span data-ttu-id="e99b1-127">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="e99b1-127">Not yet documented</span></span>|
|<span data-ttu-id="e99b1-128">lastRefreshTime</span><span class="sxs-lookup"><span data-stu-id="e99b1-128">lastRefreshTime</span></span>|<span data-ttu-id="e99b1-129">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e99b1-129">DateTimeOffset</span></span>|<span data-ttu-id="e99b1-130">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="e99b1-130">Not yet documented</span></span>|
|<span data-ttu-id="e99b1-131">configurationDeploymentSummaryPerApp</span><span class="sxs-lookup"><span data-stu-id="e99b1-131">configurationDeploymentSummaryPerApp</span></span>|<span data-ttu-id="e99b1-132">[managedAppPolicyDeploymentSummaryPerApp](../resources/intune-mam-managedapppolicydeploymentsummaryperapp.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="e99b1-132">[managedAppPolicyDeploymentSummaryPerApp](../resources/intune-mam-managedapppolicydeploymentsummaryperapp.md) collection</span></span>|<span data-ttu-id="e99b1-133">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="e99b1-133">Not yet documented</span></span>|
|<span data-ttu-id="e99b1-134">id</span><span class="sxs-lookup"><span data-stu-id="e99b1-134">id</span></span>|<span data-ttu-id="e99b1-135">String</span><span class="sxs-lookup"><span data-stu-id="e99b1-135">String</span></span>|<span data-ttu-id="e99b1-136">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="e99b1-136">Key of the entity.</span></span>|
|<span data-ttu-id="e99b1-137">version</span><span class="sxs-lookup"><span data-stu-id="e99b1-137">version</span></span>|<span data-ttu-id="e99b1-138">String</span><span class="sxs-lookup"><span data-stu-id="e99b1-138">String</span></span>|<span data-ttu-id="e99b1-139">エンティティのバージョン。</span><span class="sxs-lookup"><span data-stu-id="e99b1-139">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e99b1-140">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="e99b1-140">Relationships</span></span>
<span data-ttu-id="e99b1-141">なし</span><span class="sxs-lookup"><span data-stu-id="e99b1-141">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="e99b1-142">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e99b1-142">JSON Representation</span></span>
<span data-ttu-id="e99b1-143">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="e99b1-143">Here is a JSON representation of the resource.</span></span>
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





