---
title: configurationManagerClientEnabledFeatures リソースの種類
description: 構成マネージャーのクライアントに対応した機能
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 07b143a8d61335c44c83d1d88b9a67d2d3c2e4dc
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27962087"
---
# <a name="configurationmanagerclientenabledfeatures-resource-type"></a><span data-ttu-id="c713a-103">configurationManagerClientEnabledFeatures リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c713a-103">configurationManagerClientEnabledFeatures resource type</span></span>

> <span data-ttu-id="c713a-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="c713a-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c713a-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c713a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c713a-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="c713a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c713a-107">構成マネージャーのクライアントに対応した機能</span><span class="sxs-lookup"><span data-stu-id="c713a-107">configuration Manager client enabled features</span></span>
## <a name="properties"></a><span data-ttu-id="c713a-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c713a-108">Properties</span></span>
|<span data-ttu-id="c713a-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c713a-109">Property</span></span>|<span data-ttu-id="c713a-110">種類</span><span class="sxs-lookup"><span data-stu-id="c713a-110">Type</span></span>|<span data-ttu-id="c713a-111">説明</span><span class="sxs-lookup"><span data-stu-id="c713a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c713a-112">inventory</span><span class="sxs-lookup"><span data-stu-id="c713a-112">inventory</span></span>|<span data-ttu-id="c713a-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="c713a-113">Boolean</span></span>|<span data-ttu-id="c713a-114">在庫が Intune によって管理されているかどうか</span><span class="sxs-lookup"><span data-stu-id="c713a-114">Whether inventory is managed by Intune</span></span>|
|<span data-ttu-id="c713a-115">modernApps</span><span class="sxs-lookup"><span data-stu-id="c713a-115">modernApps</span></span>|<span data-ttu-id="c713a-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="c713a-116">Boolean</span></span>|<span data-ttu-id="c713a-117">モダン アプリケーションが Intune によって管理されているかどうか</span><span class="sxs-lookup"><span data-stu-id="c713a-117">Whether modern application is managed by Intune</span></span>|
|<span data-ttu-id="c713a-118">resourceAccess</span><span class="sxs-lookup"><span data-stu-id="c713a-118">resourceAccess</span></span>|<span data-ttu-id="c713a-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="c713a-119">Boolean</span></span>|<span data-ttu-id="c713a-120">リソース アクセスが Intune によって管理されているかどうか</span><span class="sxs-lookup"><span data-stu-id="c713a-120">Whether resource access is managed by Intune</span></span>|
|<span data-ttu-id="c713a-121">deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="c713a-121">deviceConfiguration</span></span>|<span data-ttu-id="c713a-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="c713a-122">Boolean</span></span>|<span data-ttu-id="c713a-123">デバイス構成が Intune によって管理されているかどうか</span><span class="sxs-lookup"><span data-stu-id="c713a-123">Whether device configuration is managed by Intune</span></span>|
|<span data-ttu-id="c713a-124">compliancePolicy</span><span class="sxs-lookup"><span data-stu-id="c713a-124">compliancePolicy</span></span>|<span data-ttu-id="c713a-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="c713a-125">Boolean</span></span>|<span data-ttu-id="c713a-126">コンプライアンス ポリシーが Intune によって管理されているかどうか</span><span class="sxs-lookup"><span data-stu-id="c713a-126">Whether compliance policy is managed by Intune</span></span>|
|<span data-ttu-id="c713a-127">windowsUpdateForBusiness</span><span class="sxs-lookup"><span data-stu-id="c713a-127">windowsUpdateForBusiness</span></span>|<span data-ttu-id="c713a-128">Boolean</span><span class="sxs-lookup"><span data-stu-id="c713a-128">Boolean</span></span>|<span data-ttu-id="c713a-129">Windows Update for Business が Intune によって管理されているかどうか</span><span class="sxs-lookup"><span data-stu-id="c713a-129">Whether Windows Update for Business is managed by Intune</span></span>|

## <a name="relationships"></a><span data-ttu-id="c713a-130">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="c713a-130">Relationships</span></span>
<span data-ttu-id="c713a-131">なし</span><span class="sxs-lookup"><span data-stu-id="c713a-131">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="c713a-132">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c713a-132">JSON Representation</span></span>
<span data-ttu-id="c713a-133">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="c713a-133">Here is a JSON representation of the resource.</span></span>
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





