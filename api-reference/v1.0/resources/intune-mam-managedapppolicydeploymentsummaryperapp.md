---
title: managedAppPolicyDeploymentSummaryPerApp リソースの種類
description: アプリごとのポリシーの展開の概要を表します。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 025103e40e3babde67437952fe8730b0f04410d2
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27855168"
---
# <a name="managedapppolicydeploymentsummaryperapp-resource-type"></a><span data-ttu-id="d732d-103">managedAppPolicyDeploymentSummaryPerApp リソースの種類</span><span class="sxs-lookup"><span data-stu-id="d732d-103">managedAppPolicyDeploymentSummaryPerApp resource type</span></span>

> <span data-ttu-id="d732d-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="d732d-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d732d-105">アプリごとのポリシーの展開の概要を表します。</span><span class="sxs-lookup"><span data-stu-id="d732d-105">Represents policy deployment summary per app.</span></span>
## <a name="properties"></a><span data-ttu-id="d732d-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d732d-106">Properties</span></span>
|<span data-ttu-id="d732d-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d732d-107">Property</span></span>|<span data-ttu-id="d732d-108">種類</span><span class="sxs-lookup"><span data-stu-id="d732d-108">Type</span></span>|<span data-ttu-id="d732d-109">説明</span><span class="sxs-lookup"><span data-stu-id="d732d-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d732d-110">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="d732d-110">mobileAppIdentifier</span></span>|[<span data-ttu-id="d732d-111">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="d732d-111">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="d732d-112">アプリの展開</span><span class="sxs-lookup"><span data-stu-id="d732d-112">Deployment of an app.</span></span>|
|<span data-ttu-id="d732d-113">configurationAppliedUserCount</span><span class="sxs-lookup"><span data-stu-id="d732d-113">configurationAppliedUserCount</span></span>|<span data-ttu-id="d732d-114">Int32</span><span class="sxs-lookup"><span data-stu-id="d732d-114">Int32</span></span>|<span data-ttu-id="d732d-115">ポリシーが適用されているユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="d732d-115">Number of users the policy is applied.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d732d-116">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="d732d-116">Relationships</span></span>
<span data-ttu-id="d732d-117">なし</span><span class="sxs-lookup"><span data-stu-id="d732d-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="d732d-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d732d-118">JSON Representation</span></span>
<span data-ttu-id="d732d-119">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="d732d-119">Here is a JSON representation of the resource.</span></span>
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



