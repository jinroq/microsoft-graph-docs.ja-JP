---
title: managedAppPolicyDeploymentSummaryPerApp リソースの種類
description: アプリごとのポリシーの展開の概要を表します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 149a578f60ba5953f77c83ca2fbc3810931dffff
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32465301"
---
# <a name="managedapppolicydeploymentsummaryperapp-resource-type"></a><span data-ttu-id="fe35d-103">managedAppPolicyDeploymentSummaryPerApp リソースの種類</span><span class="sxs-lookup"><span data-stu-id="fe35d-103">managedAppPolicyDeploymentSummaryPerApp resource type</span></span>

> <span data-ttu-id="fe35d-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="fe35d-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fe35d-105">アプリごとのポリシーの展開の概要を表します。</span><span class="sxs-lookup"><span data-stu-id="fe35d-105">Represents policy deployment summary per app.</span></span>

## <a name="properties"></a><span data-ttu-id="fe35d-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fe35d-106">Properties</span></span>
|<span data-ttu-id="fe35d-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fe35d-107">Property</span></span>|<span data-ttu-id="fe35d-108">型</span><span class="sxs-lookup"><span data-stu-id="fe35d-108">Type</span></span>|<span data-ttu-id="fe35d-109">説明</span><span class="sxs-lookup"><span data-stu-id="fe35d-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fe35d-110">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="fe35d-110">mobileAppIdentifier</span></span>|[<span data-ttu-id="fe35d-111">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="fe35d-111">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="fe35d-112">アプリの展開</span><span class="sxs-lookup"><span data-stu-id="fe35d-112">Deployment of an app.</span></span>|
|<span data-ttu-id="fe35d-113">configurationAppliedUserCount</span><span class="sxs-lookup"><span data-stu-id="fe35d-113">configurationAppliedUserCount</span></span>|<span data-ttu-id="fe35d-114">Int32</span><span class="sxs-lookup"><span data-stu-id="fe35d-114">Int32</span></span>|<span data-ttu-id="fe35d-115">ポリシーが適用されているユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="fe35d-115">Number of users the policy is applied.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fe35d-116">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="fe35d-116">Relationships</span></span>
<span data-ttu-id="fe35d-117">なし</span><span class="sxs-lookup"><span data-stu-id="fe35d-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fe35d-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="fe35d-118">JSON Representation</span></span>
<span data-ttu-id="fe35d-119">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="fe35d-119">Here is a JSON representation of the resource.</span></span>
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



