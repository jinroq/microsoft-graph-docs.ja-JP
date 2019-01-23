---
title: managedAppPolicyDeploymentSummaryPerApp リソースの種類
description: アプリごとのポリシーの展開の概要を表します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 0e6053a1d690a68359fa30d5e5ac4c0ce5520bc6
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29411093"
---
# <a name="managedapppolicydeploymentsummaryperapp-resource-type"></a><span data-ttu-id="e439c-103">managedAppPolicyDeploymentSummaryPerApp リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e439c-103">managedAppPolicyDeploymentSummaryPerApp resource type</span></span>

> <span data-ttu-id="e439c-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="e439c-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="e439c-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e439c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e439c-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="e439c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e439c-107">アプリごとのポリシーの展開の概要を表します。</span><span class="sxs-lookup"><span data-stu-id="e439c-107">Represents policy deployment summary per app.</span></span>

## <a name="properties"></a><span data-ttu-id="e439c-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e439c-108">Properties</span></span>
|<span data-ttu-id="e439c-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e439c-109">Property</span></span>|<span data-ttu-id="e439c-110">型</span><span class="sxs-lookup"><span data-stu-id="e439c-110">Type</span></span>|<span data-ttu-id="e439c-111">説明</span><span class="sxs-lookup"><span data-stu-id="e439c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e439c-112">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="e439c-112">mobileAppIdentifier</span></span>|[<span data-ttu-id="e439c-113">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="e439c-113">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="e439c-114">アプリの展開</span><span class="sxs-lookup"><span data-stu-id="e439c-114">Deployment of an app.</span></span>|
|<span data-ttu-id="e439c-115">configurationAppliedUserCount</span><span class="sxs-lookup"><span data-stu-id="e439c-115">configurationAppliedUserCount</span></span>|<span data-ttu-id="e439c-116">Int32</span><span class="sxs-lookup"><span data-stu-id="e439c-116">Int32</span></span>|<span data-ttu-id="e439c-117">ポリシーが適用されているユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="e439c-117">Number of users the policy is applied.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e439c-118">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="e439c-118">Relationships</span></span>
<span data-ttu-id="e439c-119">なし</span><span class="sxs-lookup"><span data-stu-id="e439c-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e439c-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e439c-120">JSON Representation</span></span>
<span data-ttu-id="e439c-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="e439c-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedAppPolicyDeploymentSummaryPerApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppPolicyDeploymentSummaryPerApp",
  "mobileAppIdentifier": {
    "@odata.type": "microsoft.graph.mobileAppIdentifier"
  },
  "configurationAppliedUserCount": 1024
}
```




