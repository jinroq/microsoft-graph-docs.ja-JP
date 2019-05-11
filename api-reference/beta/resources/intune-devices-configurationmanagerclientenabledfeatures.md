---
title: configurationManagerClientEnabledFeatures リソースの種類
description: 構成マネージャーのクライアントに対応した機能
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 37c098910ec532a1ab23ae8464c03e43cf7a9e29
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33943040"
---
# <a name="configurationmanagerclientenabledfeatures-resource-type"></a><span data-ttu-id="151c9-103">configurationManagerClientEnabledFeatures リソースの種類</span><span class="sxs-lookup"><span data-stu-id="151c9-103">configurationManagerClientEnabledFeatures resource type</span></span>

> <span data-ttu-id="151c9-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="151c9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="151c9-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="151c9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="151c9-106">構成マネージャーのクライアントに対応した機能</span><span class="sxs-lookup"><span data-stu-id="151c9-106">configuration Manager client enabled features</span></span>

## <a name="properties"></a><span data-ttu-id="151c9-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="151c9-107">Properties</span></span>
|<span data-ttu-id="151c9-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="151c9-108">Property</span></span>|<span data-ttu-id="151c9-109">型</span><span class="sxs-lookup"><span data-stu-id="151c9-109">Type</span></span>|<span data-ttu-id="151c9-110">説明</span><span class="sxs-lookup"><span data-stu-id="151c9-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="151c9-111">inventory</span><span class="sxs-lookup"><span data-stu-id="151c9-111">inventory</span></span>|<span data-ttu-id="151c9-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="151c9-112">Boolean</span></span>|<span data-ttu-id="151c9-113">在庫が Intune によって管理されているかどうか</span><span class="sxs-lookup"><span data-stu-id="151c9-113">Whether inventory is managed by Intune</span></span>|
|<span data-ttu-id="151c9-114">modernApps</span><span class="sxs-lookup"><span data-stu-id="151c9-114">modernApps</span></span>|<span data-ttu-id="151c9-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="151c9-115">Boolean</span></span>|<span data-ttu-id="151c9-116">モダン アプリケーションが Intune によって管理されているかどうか</span><span class="sxs-lookup"><span data-stu-id="151c9-116">Whether modern application is managed by Intune</span></span>|
|<span data-ttu-id="151c9-117">resourceAccess</span><span class="sxs-lookup"><span data-stu-id="151c9-117">resourceAccess</span></span>|<span data-ttu-id="151c9-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="151c9-118">Boolean</span></span>|<span data-ttu-id="151c9-119">リソース アクセスが Intune によって管理されているかどうか</span><span class="sxs-lookup"><span data-stu-id="151c9-119">Whether resource access is managed by Intune</span></span>|
|<span data-ttu-id="151c9-120">deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="151c9-120">deviceConfiguration</span></span>|<span data-ttu-id="151c9-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="151c9-121">Boolean</span></span>|<span data-ttu-id="151c9-122">デバイス構成が Intune によって管理されているかどうか</span><span class="sxs-lookup"><span data-stu-id="151c9-122">Whether device configuration is managed by Intune</span></span>|
|<span data-ttu-id="151c9-123">compliancePolicy</span><span class="sxs-lookup"><span data-stu-id="151c9-123">compliancePolicy</span></span>|<span data-ttu-id="151c9-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="151c9-124">Boolean</span></span>|<span data-ttu-id="151c9-125">コンプライアンス ポリシーが Intune によって管理されているかどうか</span><span class="sxs-lookup"><span data-stu-id="151c9-125">Whether compliance policy is managed by Intune</span></span>|
|<span data-ttu-id="151c9-126">windowsUpdateForBusiness</span><span class="sxs-lookup"><span data-stu-id="151c9-126">windowsUpdateForBusiness</span></span>|<span data-ttu-id="151c9-127">Boolean</span><span class="sxs-lookup"><span data-stu-id="151c9-127">Boolean</span></span>|<span data-ttu-id="151c9-128">Windows Update for Business が Intune によって管理されているかどうか</span><span class="sxs-lookup"><span data-stu-id="151c9-128">Whether Windows Update for Business is managed by Intune</span></span>|
|<span data-ttu-id="151c9-129">endpointProtection</span><span class="sxs-lookup"><span data-stu-id="151c9-129">endpointProtection</span></span>|<span data-ttu-id="151c9-130">Boolean</span><span class="sxs-lookup"><span data-stu-id="151c9-130">Boolean</span></span>|<span data-ttu-id="151c9-131">エンドポイント保護が Intune によって管理されているかどうか</span><span class="sxs-lookup"><span data-stu-id="151c9-131">Whether Endpoint Protection is managed by Intune</span></span>|
|<span data-ttu-id="151c9-132">Officeoffice</span><span class="sxs-lookup"><span data-stu-id="151c9-132">officeApps</span></span>|<span data-ttu-id="151c9-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="151c9-133">Boolean</span></span>|<span data-ttu-id="151c9-134">Office アプリケーションが Intune によって管理されているかどうか</span><span class="sxs-lookup"><span data-stu-id="151c9-134">Whether Office application is managed by Intune</span></span>|

## <a name="relationships"></a><span data-ttu-id="151c9-135">関係</span><span class="sxs-lookup"><span data-stu-id="151c9-135">Relationships</span></span>
<span data-ttu-id="151c9-136">なし</span><span class="sxs-lookup"><span data-stu-id="151c9-136">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="151c9-137">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="151c9-137">JSON Representation</span></span>
<span data-ttu-id="151c9-138">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="151c9-138">Here is a JSON representation of the resource.</span></span>
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
  "windowsUpdateForBusiness": true,
  "endpointProtection": true,
  "officeApps": true
}
```




