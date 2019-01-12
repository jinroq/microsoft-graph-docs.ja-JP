---
title: managedAppPolicyDeploymentSummaryPerApp リソースの種類
description: アプリごとのポリシーの展開の概要を表します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 211b40c397ec7e3fb4000c8f4459056edec2a6f1
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27972202"
---
# <a name="managedapppolicydeploymentsummaryperapp-resource-type"></a><span data-ttu-id="64ba2-103">managedAppPolicyDeploymentSummaryPerApp リソースの種類</span><span class="sxs-lookup"><span data-stu-id="64ba2-103">managedAppPolicyDeploymentSummaryPerApp resource type</span></span>

> <span data-ttu-id="64ba2-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="64ba2-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="64ba2-105">アプリごとのポリシーの展開の概要を表します。</span><span class="sxs-lookup"><span data-stu-id="64ba2-105">Represents policy deployment summary per app.</span></span>
## <a name="properties"></a><span data-ttu-id="64ba2-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="64ba2-106">Properties</span></span>
|<span data-ttu-id="64ba2-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="64ba2-107">Property</span></span>|<span data-ttu-id="64ba2-108">種類</span><span class="sxs-lookup"><span data-stu-id="64ba2-108">Type</span></span>|<span data-ttu-id="64ba2-109">説明</span><span class="sxs-lookup"><span data-stu-id="64ba2-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="64ba2-110">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="64ba2-110">mobileAppIdentifier</span></span>|[<span data-ttu-id="64ba2-111">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="64ba2-111">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="64ba2-112">アプリの展開</span><span class="sxs-lookup"><span data-stu-id="64ba2-112">Deployment of an app.</span></span>|
|<span data-ttu-id="64ba2-113">configurationAppliedUserCount</span><span class="sxs-lookup"><span data-stu-id="64ba2-113">configurationAppliedUserCount</span></span>|<span data-ttu-id="64ba2-114">Int32</span><span class="sxs-lookup"><span data-stu-id="64ba2-114">Int32</span></span>|<span data-ttu-id="64ba2-115">ポリシーが適用されているユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="64ba2-115">Number of users the policy is applied.</span></span>|

## <a name="relationships"></a><span data-ttu-id="64ba2-116">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="64ba2-116">Relationships</span></span>
<span data-ttu-id="64ba2-117">なし</span><span class="sxs-lookup"><span data-stu-id="64ba2-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="64ba2-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="64ba2-118">JSON Representation</span></span>
<span data-ttu-id="64ba2-119">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="64ba2-119">Here is a JSON representation of the resource.</span></span>
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



