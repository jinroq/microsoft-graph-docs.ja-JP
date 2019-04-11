---
title: managedAppPolicyDeploymentSummaryPerApp リソースの種類
description: アプリごとのポリシーの展開の概要を表します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 23fb9b2658bb15a851fca169c37bcf080d1c7c1c
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31803711"
---
# <a name="managedapppolicydeploymentsummaryperapp-resource-type"></a><span data-ttu-id="fb4bb-103">managedAppPolicyDeploymentSummaryPerApp リソースの種類</span><span class="sxs-lookup"><span data-stu-id="fb4bb-103">managedAppPolicyDeploymentSummaryPerApp resource type</span></span>

> <span data-ttu-id="fb4bb-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fb4bb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fb4bb-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="fb4bb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fb4bb-106">アプリごとのポリシーの展開の概要を表します。</span><span class="sxs-lookup"><span data-stu-id="fb4bb-106">Represents policy deployment summary per app.</span></span>

## <a name="properties"></a><span data-ttu-id="fb4bb-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fb4bb-107">Properties</span></span>
|<span data-ttu-id="fb4bb-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fb4bb-108">Property</span></span>|<span data-ttu-id="fb4bb-109">型</span><span class="sxs-lookup"><span data-stu-id="fb4bb-109">Type</span></span>|<span data-ttu-id="fb4bb-110">説明</span><span class="sxs-lookup"><span data-stu-id="fb4bb-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fb4bb-111">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="fb4bb-111">mobileAppIdentifier</span></span>|[<span data-ttu-id="fb4bb-112">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="fb4bb-112">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="fb4bb-113">アプリの展開</span><span class="sxs-lookup"><span data-stu-id="fb4bb-113">Deployment of an app.</span></span>|
|<span data-ttu-id="fb4bb-114">configurationAppliedUserCount</span><span class="sxs-lookup"><span data-stu-id="fb4bb-114">configurationAppliedUserCount</span></span>|<span data-ttu-id="fb4bb-115">Int32</span><span class="sxs-lookup"><span data-stu-id="fb4bb-115">Int32</span></span>|<span data-ttu-id="fb4bb-116">ポリシーが適用されているユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="fb4bb-116">Number of users the policy is applied.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fb4bb-117">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="fb4bb-117">Relationships</span></span>
<span data-ttu-id="fb4bb-118">なし</span><span class="sxs-lookup"><span data-stu-id="fb4bb-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fb4bb-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="fb4bb-119">JSON Representation</span></span>
<span data-ttu-id="fb4bb-120">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="fb4bb-120">Here is a JSON representation of the resource.</span></span>
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





