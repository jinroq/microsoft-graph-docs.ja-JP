---
title: configurationManagerClientEnabledFeatures リソースの種類
description: 構成マネージャーのクライアントに対応した機能
author: tfitzmac
ms.openlocfilehash: e0d704fddc084a455c83c5b55ea9b3911f3f232a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27343940"
---
# <a name="configurationmanagerclientenabledfeatures-resource-type"></a><span data-ttu-id="0946a-103">configurationManagerClientEnabledFeatures リソースの種類</span><span class="sxs-lookup"><span data-stu-id="0946a-103">configurationManagerClientEnabledFeatures resource type</span></span>

> <span data-ttu-id="0946a-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="0946a-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0946a-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0946a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0946a-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="0946a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0946a-107">構成マネージャーのクライアントに対応した機能</span><span class="sxs-lookup"><span data-stu-id="0946a-107">configuration Manager client enabled features</span></span>
## <a name="properties"></a><span data-ttu-id="0946a-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0946a-108">Properties</span></span>
|<span data-ttu-id="0946a-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0946a-109">Property</span></span>|<span data-ttu-id="0946a-110">種類</span><span class="sxs-lookup"><span data-stu-id="0946a-110">Type</span></span>|<span data-ttu-id="0946a-111">説明</span><span class="sxs-lookup"><span data-stu-id="0946a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0946a-112">inventory</span><span class="sxs-lookup"><span data-stu-id="0946a-112">inventory</span></span>|<span data-ttu-id="0946a-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="0946a-113">Boolean</span></span>|<span data-ttu-id="0946a-114">在庫が Intune によって管理されているかどうか</span><span class="sxs-lookup"><span data-stu-id="0946a-114">Whether inventory is managed by Intune</span></span>|
|<span data-ttu-id="0946a-115">modernApps</span><span class="sxs-lookup"><span data-stu-id="0946a-115">modernApps</span></span>|<span data-ttu-id="0946a-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="0946a-116">Boolean</span></span>|<span data-ttu-id="0946a-117">モダン アプリケーションが Intune によって管理されているかどうか</span><span class="sxs-lookup"><span data-stu-id="0946a-117">Whether modern application is managed by Intune</span></span>|
|<span data-ttu-id="0946a-118">resourceAccess</span><span class="sxs-lookup"><span data-stu-id="0946a-118">resourceAccess</span></span>|<span data-ttu-id="0946a-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="0946a-119">Boolean</span></span>|<span data-ttu-id="0946a-120">リソース アクセスが Intune によって管理されているかどうか</span><span class="sxs-lookup"><span data-stu-id="0946a-120">Whether resource access is managed by Intune</span></span>|
|<span data-ttu-id="0946a-121">deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="0946a-121">deviceConfiguration</span></span>|<span data-ttu-id="0946a-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="0946a-122">Boolean</span></span>|<span data-ttu-id="0946a-123">デバイス構成が Intune によって管理されているかどうか</span><span class="sxs-lookup"><span data-stu-id="0946a-123">Whether device configuration is managed by Intune</span></span>|
|<span data-ttu-id="0946a-124">compliancePolicy</span><span class="sxs-lookup"><span data-stu-id="0946a-124">compliancePolicy</span></span>|<span data-ttu-id="0946a-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="0946a-125">Boolean</span></span>|<span data-ttu-id="0946a-126">コンプライアンス ポリシーが Intune によって管理されているかどうか</span><span class="sxs-lookup"><span data-stu-id="0946a-126">Whether compliance policy is managed by Intune</span></span>|
|<span data-ttu-id="0946a-127">windowsUpdateForBusiness</span><span class="sxs-lookup"><span data-stu-id="0946a-127">windowsUpdateForBusiness</span></span>|<span data-ttu-id="0946a-128">Boolean</span><span class="sxs-lookup"><span data-stu-id="0946a-128">Boolean</span></span>|<span data-ttu-id="0946a-129">Windows Update for Business が Intune によって管理されているかどうか</span><span class="sxs-lookup"><span data-stu-id="0946a-129">Whether Windows Update for Business is managed by Intune</span></span>|

## <a name="relationships"></a><span data-ttu-id="0946a-130">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="0946a-130">Relationships</span></span>
<span data-ttu-id="0946a-131">なし</span><span class="sxs-lookup"><span data-stu-id="0946a-131">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="0946a-132">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0946a-132">JSON Representation</span></span>
<span data-ttu-id="0946a-133">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="0946a-133">Here is a JSON representation of the resource.</span></span>
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





