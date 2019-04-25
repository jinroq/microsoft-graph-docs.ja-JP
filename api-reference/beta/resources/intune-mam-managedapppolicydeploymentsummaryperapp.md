---
title: managedAppPolicyDeploymentSummaryPerApp リソースの種類
description: アプリごとのポリシーの展開の概要を表します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 23fb9b2658bb15a851fca169c37bcf080d1c7c1c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32573893"
---
# <a name="managedapppolicydeploymentsummaryperapp-resource-type"></a><span data-ttu-id="b4bb6-103">managedAppPolicyDeploymentSummaryPerApp リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b4bb6-103">managedAppPolicyDeploymentSummaryPerApp resource type</span></span>

> <span data-ttu-id="b4bb6-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b4bb6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b4bb6-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="b4bb6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b4bb6-106">アプリごとのポリシーの展開の概要を表します。</span><span class="sxs-lookup"><span data-stu-id="b4bb6-106">Represents policy deployment summary per app.</span></span>

## <a name="properties"></a><span data-ttu-id="b4bb6-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b4bb6-107">Properties</span></span>
|<span data-ttu-id="b4bb6-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b4bb6-108">Property</span></span>|<span data-ttu-id="b4bb6-109">型</span><span class="sxs-lookup"><span data-stu-id="b4bb6-109">Type</span></span>|<span data-ttu-id="b4bb6-110">説明</span><span class="sxs-lookup"><span data-stu-id="b4bb6-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b4bb6-111">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="b4bb6-111">mobileAppIdentifier</span></span>|[<span data-ttu-id="b4bb6-112">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="b4bb6-112">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="b4bb6-113">アプリの展開</span><span class="sxs-lookup"><span data-stu-id="b4bb6-113">Deployment of an app.</span></span>|
|<span data-ttu-id="b4bb6-114">configurationAppliedUserCount</span><span class="sxs-lookup"><span data-stu-id="b4bb6-114">configurationAppliedUserCount</span></span>|<span data-ttu-id="b4bb6-115">Int32</span><span class="sxs-lookup"><span data-stu-id="b4bb6-115">Int32</span></span>|<span data-ttu-id="b4bb6-116">ポリシーが適用されているユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="b4bb6-116">Number of users the policy is applied.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b4bb6-117">関係</span><span class="sxs-lookup"><span data-stu-id="b4bb6-117">Relationships</span></span>
<span data-ttu-id="b4bb6-118">なし</span><span class="sxs-lookup"><span data-stu-id="b4bb6-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b4bb6-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b4bb6-119">JSON Representation</span></span>
<span data-ttu-id="b4bb6-120">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="b4bb6-120">Here is a JSON representation of the resource.</span></span>
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





