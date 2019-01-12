---
title: configurationManagerClientEnabledFeatures リソースの種類
description: 構成マネージャーのクライアントに対応した機能
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: dc1b994615c89b1a6e73785a5ebcdc85f0638953
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27987594"
---
# <a name="configurationmanagerclientenabledfeatures-resource-type"></a><span data-ttu-id="03e4e-103">configurationManagerClientEnabledFeatures リソースの種類</span><span class="sxs-lookup"><span data-stu-id="03e4e-103">configurationManagerClientEnabledFeatures resource type</span></span>

> <span data-ttu-id="03e4e-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="03e4e-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="03e4e-105">構成マネージャーのクライアントに対応した機能</span><span class="sxs-lookup"><span data-stu-id="03e4e-105">configuration Manager client enabled features</span></span>
## <a name="properties"></a><span data-ttu-id="03e4e-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="03e4e-106">Properties</span></span>
|<span data-ttu-id="03e4e-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="03e4e-107">Property</span></span>|<span data-ttu-id="03e4e-108">種類</span><span class="sxs-lookup"><span data-stu-id="03e4e-108">Type</span></span>|<span data-ttu-id="03e4e-109">説明</span><span class="sxs-lookup"><span data-stu-id="03e4e-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="03e4e-110">inventory</span><span class="sxs-lookup"><span data-stu-id="03e4e-110">inventory</span></span>|<span data-ttu-id="03e4e-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="03e4e-111">Boolean</span></span>|<span data-ttu-id="03e4e-112">在庫が Intune によって管理されているかどうか</span><span class="sxs-lookup"><span data-stu-id="03e4e-112">Whether inventory is managed by Intune</span></span>|
|<span data-ttu-id="03e4e-113">modernApps</span><span class="sxs-lookup"><span data-stu-id="03e4e-113">modernApps</span></span>|<span data-ttu-id="03e4e-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="03e4e-114">Boolean</span></span>|<span data-ttu-id="03e4e-115">モダン アプリケーションが Intune によって管理されているかどうか</span><span class="sxs-lookup"><span data-stu-id="03e4e-115">Whether modern application is managed by Intune</span></span>|
|<span data-ttu-id="03e4e-116">resourceAccess</span><span class="sxs-lookup"><span data-stu-id="03e4e-116">resourceAccess</span></span>|<span data-ttu-id="03e4e-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="03e4e-117">Boolean</span></span>|<span data-ttu-id="03e4e-118">リソース アクセスが Intune によって管理されているかどうか</span><span class="sxs-lookup"><span data-stu-id="03e4e-118">Whether resource access is managed by Intune</span></span>|
|<span data-ttu-id="03e4e-119">deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="03e4e-119">deviceConfiguration</span></span>|<span data-ttu-id="03e4e-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="03e4e-120">Boolean</span></span>|<span data-ttu-id="03e4e-121">デバイス構成が Intune によって管理されているかどうか</span><span class="sxs-lookup"><span data-stu-id="03e4e-121">Whether device configuration is managed by Intune</span></span>|
|<span data-ttu-id="03e4e-122">compliancePolicy</span><span class="sxs-lookup"><span data-stu-id="03e4e-122">compliancePolicy</span></span>|<span data-ttu-id="03e4e-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="03e4e-123">Boolean</span></span>|<span data-ttu-id="03e4e-124">コンプライアンス ポリシーが Intune によって管理されているかどうか</span><span class="sxs-lookup"><span data-stu-id="03e4e-124">Whether compliance policy is managed by Intune</span></span>|
|<span data-ttu-id="03e4e-125">windowsUpdateForBusiness</span><span class="sxs-lookup"><span data-stu-id="03e4e-125">windowsUpdateForBusiness</span></span>|<span data-ttu-id="03e4e-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="03e4e-126">Boolean</span></span>|<span data-ttu-id="03e4e-127">Windows Update for Business が Intune によって管理されているかどうか</span><span class="sxs-lookup"><span data-stu-id="03e4e-127">Whether Windows Update for Business is managed by Intune</span></span>|

## <a name="relationships"></a><span data-ttu-id="03e4e-128">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="03e4e-128">Relationships</span></span>
<span data-ttu-id="03e4e-129">なし</span><span class="sxs-lookup"><span data-stu-id="03e4e-129">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="03e4e-130">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="03e4e-130">JSON Representation</span></span>
<span data-ttu-id="03e4e-131">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="03e4e-131">Here is a JSON representation of the resource.</span></span>
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



