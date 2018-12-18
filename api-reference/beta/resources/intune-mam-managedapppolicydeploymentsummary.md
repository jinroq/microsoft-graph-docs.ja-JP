---
title: managedAppPolicyDeploymentSummary リソースの種類
description: ManagedAppEntity は、アプリ管理ワークフロー下にある他のすべてのエンティティ タイプの基本型です。
author: tfitzmac
ms.openlocfilehash: 872a5685cce5d7c422035670eb10d72185fd344f
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27305790"
---
# <a name="managedapppolicydeploymentsummary-resource-type"></a><span data-ttu-id="31382-103">managedAppPolicyDeploymentSummary リソースの種類</span><span class="sxs-lookup"><span data-stu-id="31382-103">managedAppPolicyDeploymentSummary resource type</span></span>

> <span data-ttu-id="31382-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="31382-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="31382-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="31382-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="31382-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="31382-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="31382-107">ManagedAppEntity は、アプリ管理ワークフロー下にある他のすべてのエンティティの種類の基本型です。</span><span class="sxs-lookup"><span data-stu-id="31382-107">The ManagedAppEntity is the base entity type for all other entity types under app management workflow.</span></span>
## <a name="methods"></a><span data-ttu-id="31382-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="31382-108">Methods</span></span>
|<span data-ttu-id="31382-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="31382-109">Method</span></span>|<span data-ttu-id="31382-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="31382-110">Return Type</span></span>|<span data-ttu-id="31382-111">説明</span><span class="sxs-lookup"><span data-stu-id="31382-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="31382-112">Get managedAppPolicyDeploymentSummary</span><span class="sxs-lookup"><span data-stu-id="31382-112">Get managedAppPolicyDeploymentSummary</span></span>](../api/intune-mam-managedapppolicydeploymentsummary-get.md)|[<span data-ttu-id="31382-113">managedAppPolicyDeploymentSummary</span><span class="sxs-lookup"><span data-stu-id="31382-113">managedAppPolicyDeploymentSummary</span></span>](../resources/intune-mam-managedapppolicydeploymentsummary.md)|<span data-ttu-id="31382-114">[managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="31382-114">Read properties and relationships of the [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) object.</span></span>|
|[<span data-ttu-id="31382-115">Update managedAppPolicyDeploymentSummary</span><span class="sxs-lookup"><span data-stu-id="31382-115">Update managedAppPolicyDeploymentSummary</span></span>](../api/intune-mam-managedapppolicydeploymentsummary-update.md)|[<span data-ttu-id="31382-116">managedAppPolicyDeploymentSummary</span><span class="sxs-lookup"><span data-stu-id="31382-116">managedAppPolicyDeploymentSummary</span></span>](../resources/intune-mam-managedapppolicydeploymentsummary.md)|<span data-ttu-id="31382-117">[managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="31382-117">Update the properties of a [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="31382-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="31382-118">Properties</span></span>
|<span data-ttu-id="31382-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="31382-119">Property</span></span>|<span data-ttu-id="31382-120">種類</span><span class="sxs-lookup"><span data-stu-id="31382-120">Type</span></span>|<span data-ttu-id="31382-121">説明</span><span class="sxs-lookup"><span data-stu-id="31382-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="31382-122">displayName</span><span class="sxs-lookup"><span data-stu-id="31382-122">displayName</span></span>|<span data-ttu-id="31382-123">String</span><span class="sxs-lookup"><span data-stu-id="31382-123">String</span></span>|<span data-ttu-id="31382-124">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="31382-124">Not yet documented</span></span>|
|<span data-ttu-id="31382-125">configurationDeployedUserCount</span><span class="sxs-lookup"><span data-stu-id="31382-125">configurationDeployedUserCount</span></span>|<span data-ttu-id="31382-126">Int32</span><span class="sxs-lookup"><span data-stu-id="31382-126">Int32</span></span>|<span data-ttu-id="31382-127">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="31382-127">Not yet documented</span></span>|
|<span data-ttu-id="31382-128">lastRefreshTime</span><span class="sxs-lookup"><span data-stu-id="31382-128">lastRefreshTime</span></span>|<span data-ttu-id="31382-129">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="31382-129">DateTimeOffset</span></span>|<span data-ttu-id="31382-130">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="31382-130">Not yet documented</span></span>|
|<span data-ttu-id="31382-131">configurationDeploymentSummaryPerApp</span><span class="sxs-lookup"><span data-stu-id="31382-131">configurationDeploymentSummaryPerApp</span></span>|<span data-ttu-id="31382-132">[managedAppPolicyDeploymentSummaryPerApp](../resources/intune-mam-managedapppolicydeploymentsummaryperapp.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="31382-132">[managedAppPolicyDeploymentSummaryPerApp](../resources/intune-mam-managedapppolicydeploymentsummaryperapp.md) collection</span></span>|<span data-ttu-id="31382-133">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="31382-133">Not yet documented</span></span>|
|<span data-ttu-id="31382-134">id</span><span class="sxs-lookup"><span data-stu-id="31382-134">id</span></span>|<span data-ttu-id="31382-135">String</span><span class="sxs-lookup"><span data-stu-id="31382-135">String</span></span>|<span data-ttu-id="31382-136">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="31382-136">Key of the entity.</span></span>|
|<span data-ttu-id="31382-137">version</span><span class="sxs-lookup"><span data-stu-id="31382-137">version</span></span>|<span data-ttu-id="31382-138">String</span><span class="sxs-lookup"><span data-stu-id="31382-138">String</span></span>|<span data-ttu-id="31382-139">エンティティのバージョン。</span><span class="sxs-lookup"><span data-stu-id="31382-139">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="31382-140">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="31382-140">Relationships</span></span>
<span data-ttu-id="31382-141">なし</span><span class="sxs-lookup"><span data-stu-id="31382-141">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="31382-142">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="31382-142">JSON Representation</span></span>
<span data-ttu-id="31382-143">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="31382-143">Here is a JSON representation of the resource.</span></span>
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





