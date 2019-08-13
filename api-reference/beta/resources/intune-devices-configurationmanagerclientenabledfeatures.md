---
title: configurationManagerClientEnabledFeatures リソースの種類
description: 構成マネージャーのクライアントに対応した機能
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: d9407e1d035a5cd50db7b071f562acb4eb2d007b
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36371986"
---
# <a name="configurationmanagerclientenabledfeatures-resource-type"></a><span data-ttu-id="e6b14-103">configurationManagerClientEnabledFeatures リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e6b14-103">configurationManagerClientEnabledFeatures resource type</span></span>

> <span data-ttu-id="e6b14-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e6b14-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e6b14-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="e6b14-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e6b14-106">構成マネージャーのクライアントに対応した機能</span><span class="sxs-lookup"><span data-stu-id="e6b14-106">configuration Manager client enabled features</span></span>

## <a name="properties"></a><span data-ttu-id="e6b14-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e6b14-107">Properties</span></span>
|<span data-ttu-id="e6b14-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e6b14-108">Property</span></span>|<span data-ttu-id="e6b14-109">型</span><span class="sxs-lookup"><span data-stu-id="e6b14-109">Type</span></span>|<span data-ttu-id="e6b14-110">説明</span><span class="sxs-lookup"><span data-stu-id="e6b14-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e6b14-111">inventory</span><span class="sxs-lookup"><span data-stu-id="e6b14-111">inventory</span></span>|<span data-ttu-id="e6b14-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="e6b14-112">Boolean</span></span>|<span data-ttu-id="e6b14-113">在庫が Intune によって管理されているかどうか</span><span class="sxs-lookup"><span data-stu-id="e6b14-113">Whether inventory is managed by Intune</span></span>|
|<span data-ttu-id="e6b14-114">modernApps</span><span class="sxs-lookup"><span data-stu-id="e6b14-114">modernApps</span></span>|<span data-ttu-id="e6b14-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="e6b14-115">Boolean</span></span>|<span data-ttu-id="e6b14-116">モダン アプリケーションが Intune によって管理されているかどうか</span><span class="sxs-lookup"><span data-stu-id="e6b14-116">Whether modern application is managed by Intune</span></span>|
|<span data-ttu-id="e6b14-117">resourceAccess</span><span class="sxs-lookup"><span data-stu-id="e6b14-117">resourceAccess</span></span>|<span data-ttu-id="e6b14-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="e6b14-118">Boolean</span></span>|<span data-ttu-id="e6b14-119">リソース アクセスが Intune によって管理されているかどうか</span><span class="sxs-lookup"><span data-stu-id="e6b14-119">Whether resource access is managed by Intune</span></span>|
|<span data-ttu-id="e6b14-120">deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="e6b14-120">deviceConfiguration</span></span>|<span data-ttu-id="e6b14-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="e6b14-121">Boolean</span></span>|<span data-ttu-id="e6b14-122">デバイス構成が Intune によって管理されているかどうか</span><span class="sxs-lookup"><span data-stu-id="e6b14-122">Whether device configuration is managed by Intune</span></span>|
|<span data-ttu-id="e6b14-123">compliancePolicy</span><span class="sxs-lookup"><span data-stu-id="e6b14-123">compliancePolicy</span></span>|<span data-ttu-id="e6b14-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="e6b14-124">Boolean</span></span>|<span data-ttu-id="e6b14-125">コンプライアンス ポリシーが Intune によって管理されているかどうか</span><span class="sxs-lookup"><span data-stu-id="e6b14-125">Whether compliance policy is managed by Intune</span></span>|
|<span data-ttu-id="e6b14-126">windowsUpdateForBusiness</span><span class="sxs-lookup"><span data-stu-id="e6b14-126">windowsUpdateForBusiness</span></span>|<span data-ttu-id="e6b14-127">Boolean</span><span class="sxs-lookup"><span data-stu-id="e6b14-127">Boolean</span></span>|<span data-ttu-id="e6b14-128">Windows Update for Business が Intune によって管理されているかどうか</span><span class="sxs-lookup"><span data-stu-id="e6b14-128">Whether Windows Update for Business is managed by Intune</span></span>|
|<span data-ttu-id="e6b14-129">endpointProtection</span><span class="sxs-lookup"><span data-stu-id="e6b14-129">endpointProtection</span></span>|<span data-ttu-id="e6b14-130">Boolean</span><span class="sxs-lookup"><span data-stu-id="e6b14-130">Boolean</span></span>|<span data-ttu-id="e6b14-131">エンドポイント保護が Intune によって管理されているかどうか</span><span class="sxs-lookup"><span data-stu-id="e6b14-131">Whether Endpoint Protection is managed by Intune</span></span>|
|<span data-ttu-id="e6b14-132">Officeoffice</span><span class="sxs-lookup"><span data-stu-id="e6b14-132">officeApps</span></span>|<span data-ttu-id="e6b14-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="e6b14-133">Boolean</span></span>|<span data-ttu-id="e6b14-134">Office アプリケーションが Intune によって管理されているかどうか</span><span class="sxs-lookup"><span data-stu-id="e6b14-134">Whether Office application is managed by Intune</span></span>|

## <a name="relationships"></a><span data-ttu-id="e6b14-135">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="e6b14-135">Relationships</span></span>
<span data-ttu-id="e6b14-136">なし</span><span class="sxs-lookup"><span data-stu-id="e6b14-136">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e6b14-137">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e6b14-137">JSON Representation</span></span>
<span data-ttu-id="e6b14-138">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="e6b14-138">Here is a JSON representation of the resource.</span></span>
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



