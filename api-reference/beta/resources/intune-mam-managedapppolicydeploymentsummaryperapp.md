---
title: managedAppPolicyDeploymentSummaryPerApp リソースの種類
description: アプリごとのポリシーの展開の概要を表します。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 23966e2017780d3dcfde592d7159576403fe3192
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27829751"
---
# <a name="managedapppolicydeploymentsummaryperapp-resource-type"></a><span data-ttu-id="9552e-103">managedAppPolicyDeploymentSummaryPerApp リソースの種類</span><span class="sxs-lookup"><span data-stu-id="9552e-103">managedAppPolicyDeploymentSummaryPerApp resource type</span></span>

> <span data-ttu-id="9552e-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="9552e-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9552e-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9552e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9552e-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="9552e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9552e-107">アプリごとのポリシーの展開の概要を表します。</span><span class="sxs-lookup"><span data-stu-id="9552e-107">Represents policy deployment summary per app.</span></span>
## <a name="properties"></a><span data-ttu-id="9552e-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9552e-108">Properties</span></span>
|<span data-ttu-id="9552e-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9552e-109">Property</span></span>|<span data-ttu-id="9552e-110">種類</span><span class="sxs-lookup"><span data-stu-id="9552e-110">Type</span></span>|<span data-ttu-id="9552e-111">説明</span><span class="sxs-lookup"><span data-stu-id="9552e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9552e-112">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="9552e-112">mobileAppIdentifier</span></span>|[<span data-ttu-id="9552e-113">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="9552e-113">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="9552e-114">アプリの展開</span><span class="sxs-lookup"><span data-stu-id="9552e-114">Deployment of an app.</span></span>|
|<span data-ttu-id="9552e-115">configurationAppliedUserCount</span><span class="sxs-lookup"><span data-stu-id="9552e-115">configurationAppliedUserCount</span></span>|<span data-ttu-id="9552e-116">Int32</span><span class="sxs-lookup"><span data-stu-id="9552e-116">Int32</span></span>|<span data-ttu-id="9552e-117">ポリシーが適用されているユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="9552e-117">Number of users the policy is applied.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9552e-118">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="9552e-118">Relationships</span></span>
<span data-ttu-id="9552e-119">なし</span><span class="sxs-lookup"><span data-stu-id="9552e-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="9552e-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="9552e-120">JSON Representation</span></span>
<span data-ttu-id="9552e-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="9552e-121">Here is a JSON representation of the resource.</span></span>
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





