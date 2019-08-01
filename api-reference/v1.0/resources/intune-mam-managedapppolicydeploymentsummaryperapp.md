---
title: managedAppPolicyDeploymentSummaryPerApp リソースの種類
description: アプリごとのポリシーの展開の概要を表します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 84befe8b98b2e0e6883328c09bdee16e2720300d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36037941"
---
# <a name="managedapppolicydeploymentsummaryperapp-resource-type"></a><span data-ttu-id="34c7a-103">managedAppPolicyDeploymentSummaryPerApp リソースの種類</span><span class="sxs-lookup"><span data-stu-id="34c7a-103">managedAppPolicyDeploymentSummaryPerApp resource type</span></span>

> <span data-ttu-id="34c7a-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="34c7a-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="34c7a-105">アプリごとのポリシーの展開の概要を表します。</span><span class="sxs-lookup"><span data-stu-id="34c7a-105">Represents policy deployment summary per app.</span></span>

## <a name="properties"></a><span data-ttu-id="34c7a-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="34c7a-106">Properties</span></span>
|<span data-ttu-id="34c7a-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="34c7a-107">Property</span></span>|<span data-ttu-id="34c7a-108">型</span><span class="sxs-lookup"><span data-stu-id="34c7a-108">Type</span></span>|<span data-ttu-id="34c7a-109">説明</span><span class="sxs-lookup"><span data-stu-id="34c7a-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="34c7a-110">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="34c7a-110">mobileAppIdentifier</span></span>|[<span data-ttu-id="34c7a-111">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="34c7a-111">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="34c7a-112">アプリの展開</span><span class="sxs-lookup"><span data-stu-id="34c7a-112">Deployment of an app.</span></span>|
|<span data-ttu-id="34c7a-113">configurationAppliedUserCount</span><span class="sxs-lookup"><span data-stu-id="34c7a-113">configurationAppliedUserCount</span></span>|<span data-ttu-id="34c7a-114">Int32</span><span class="sxs-lookup"><span data-stu-id="34c7a-114">Int32</span></span>|<span data-ttu-id="34c7a-115">ポリシーが適用されているユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="34c7a-115">Number of users the policy is applied.</span></span>|

## <a name="relationships"></a><span data-ttu-id="34c7a-116">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="34c7a-116">Relationships</span></span>
<span data-ttu-id="34c7a-117">なし</span><span class="sxs-lookup"><span data-stu-id="34c7a-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="34c7a-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="34c7a-118">JSON Representation</span></span>
<span data-ttu-id="34c7a-119">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="34c7a-119">Here is a JSON representation of the resource.</span></span>
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



