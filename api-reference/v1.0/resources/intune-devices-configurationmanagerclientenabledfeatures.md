---
title: configurationManagerClientEnabledFeatures リソースの種類
description: 構成マネージャーのクライアントに対応した機能
ms.openlocfilehash: 54d5d40a50b2946fec1c69c619dc76bec1f32502
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27023006"
---
# <a name="configurationmanagerclientenabledfeatures-resource-type"></a><span data-ttu-id="71153-103">configurationManagerClientEnabledFeatures リソースの種類</span><span class="sxs-lookup"><span data-stu-id="71153-103">configurationManagerClientEnabledFeatures resource type</span></span>

> <span data-ttu-id="71153-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="71153-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="71153-105">構成マネージャーのクライアントに対応した機能</span><span class="sxs-lookup"><span data-stu-id="71153-105">configuration Manager client enabled features</span></span>
## <a name="properties"></a><span data-ttu-id="71153-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="71153-106">Properties</span></span>
|<span data-ttu-id="71153-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="71153-107">Property</span></span>|<span data-ttu-id="71153-108">型</span><span class="sxs-lookup"><span data-stu-id="71153-108">Type</span></span>|<span data-ttu-id="71153-109">説明</span><span class="sxs-lookup"><span data-stu-id="71153-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="71153-110">inventory</span><span class="sxs-lookup"><span data-stu-id="71153-110">inventory</span></span>|<span data-ttu-id="71153-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="71153-111">Boolean</span></span>|<span data-ttu-id="71153-112">在庫が Intune によって管理されているかどうか</span><span class="sxs-lookup"><span data-stu-id="71153-112">Whether inventory is managed by Intune</span></span>|
|<span data-ttu-id="71153-113">modernApps</span><span class="sxs-lookup"><span data-stu-id="71153-113">modernApps</span></span>|<span data-ttu-id="71153-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="71153-114">Boolean</span></span>|<span data-ttu-id="71153-115">モダン アプリケーションが Intune によって管理されているかどうか</span><span class="sxs-lookup"><span data-stu-id="71153-115">Whether modern application is managed by Intune</span></span>|
|<span data-ttu-id="71153-116">resourceAccess</span><span class="sxs-lookup"><span data-stu-id="71153-116">resourceAccess</span></span>|<span data-ttu-id="71153-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="71153-117">Boolean</span></span>|<span data-ttu-id="71153-118">リソース アクセスが Intune によって管理されているかどうか</span><span class="sxs-lookup"><span data-stu-id="71153-118">Whether resource access is managed by Intune</span></span>|
|<span data-ttu-id="71153-119">deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="71153-119">deviceConfiguration</span></span>|<span data-ttu-id="71153-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="71153-120">Boolean</span></span>|<span data-ttu-id="71153-121">デバイス構成が Intune によって管理されているかどうか</span><span class="sxs-lookup"><span data-stu-id="71153-121">Whether device configuration is managed by Intune</span></span>|
|<span data-ttu-id="71153-122">compliancePolicy</span><span class="sxs-lookup"><span data-stu-id="71153-122">compliancePolicy</span></span>|<span data-ttu-id="71153-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="71153-123">Boolean</span></span>|<span data-ttu-id="71153-124">コンプライアンス ポリシーが Intune によって管理されているかどうか</span><span class="sxs-lookup"><span data-stu-id="71153-124">Whether compliance policy is managed by Intune</span></span>|
|<span data-ttu-id="71153-125">windowsUpdateForBusiness</span><span class="sxs-lookup"><span data-stu-id="71153-125">windowsUpdateForBusiness</span></span>|<span data-ttu-id="71153-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="71153-126">Boolean</span></span>|<span data-ttu-id="71153-127">Windows Update for Business が Intune によって管理されているかどうか</span><span class="sxs-lookup"><span data-stu-id="71153-127">Whether Windows Update for Business is managed by Intune</span></span>|

## <a name="relationships"></a><span data-ttu-id="71153-128">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="71153-128">Relationships</span></span>
<span data-ttu-id="71153-129">なし</span><span class="sxs-lookup"><span data-stu-id="71153-129">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="71153-130">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="71153-130">JSON Representation</span></span>
<span data-ttu-id="71153-131">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="71153-131">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.configurationManagerClientEnabledFeatures"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.configurationManagerClientEnabledFeatures",
  "inventory": true,
  "modernApps": true,
  "resourceAccess": true,
  "deviceConfiguration": true,
  "compliancePolicy": true,
  "windowsUpdateForBusiness": true
}
```



