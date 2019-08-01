---
title: configurationManagerClientEnabledFeatures リソースの種類
description: 構成マネージャーのクライアントに対応した機能
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 520b21445d4c5a61755ddc78c65b9999a7e45ff0
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36027497"
---
# <a name="configurationmanagerclientenabledfeatures-resource-type"></a><span data-ttu-id="b5ff5-103">configurationManagerClientEnabledFeatures リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b5ff5-103">configurationManagerClientEnabledFeatures resource type</span></span>

> <span data-ttu-id="b5ff5-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="b5ff5-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b5ff5-105">構成マネージャーのクライアントに対応した機能</span><span class="sxs-lookup"><span data-stu-id="b5ff5-105">configuration Manager client enabled features</span></span>

## <a name="properties"></a><span data-ttu-id="b5ff5-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b5ff5-106">Properties</span></span>
|<span data-ttu-id="b5ff5-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b5ff5-107">Property</span></span>|<span data-ttu-id="b5ff5-108">型</span><span class="sxs-lookup"><span data-stu-id="b5ff5-108">Type</span></span>|<span data-ttu-id="b5ff5-109">説明</span><span class="sxs-lookup"><span data-stu-id="b5ff5-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b5ff5-110">inventory</span><span class="sxs-lookup"><span data-stu-id="b5ff5-110">inventory</span></span>|<span data-ttu-id="b5ff5-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5ff5-111">Boolean</span></span>|<span data-ttu-id="b5ff5-112">在庫が Intune によって管理されているかどうか</span><span class="sxs-lookup"><span data-stu-id="b5ff5-112">Whether inventory is managed by Intune</span></span>|
|<span data-ttu-id="b5ff5-113">modernApps</span><span class="sxs-lookup"><span data-stu-id="b5ff5-113">modernApps</span></span>|<span data-ttu-id="b5ff5-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5ff5-114">Boolean</span></span>|<span data-ttu-id="b5ff5-115">モダン アプリケーションが Intune によって管理されているかどうか</span><span class="sxs-lookup"><span data-stu-id="b5ff5-115">Whether modern application is managed by Intune</span></span>|
|<span data-ttu-id="b5ff5-116">resourceAccess</span><span class="sxs-lookup"><span data-stu-id="b5ff5-116">resourceAccess</span></span>|<span data-ttu-id="b5ff5-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5ff5-117">Boolean</span></span>|<span data-ttu-id="b5ff5-118">リソース アクセスが Intune によって管理されているかどうか</span><span class="sxs-lookup"><span data-stu-id="b5ff5-118">Whether resource access is managed by Intune</span></span>|
|<span data-ttu-id="b5ff5-119">deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="b5ff5-119">deviceConfiguration</span></span>|<span data-ttu-id="b5ff5-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5ff5-120">Boolean</span></span>|<span data-ttu-id="b5ff5-121">デバイス構成が Intune によって管理されているかどうか</span><span class="sxs-lookup"><span data-stu-id="b5ff5-121">Whether device configuration is managed by Intune</span></span>|
|<span data-ttu-id="b5ff5-122">compliancePolicy</span><span class="sxs-lookup"><span data-stu-id="b5ff5-122">compliancePolicy</span></span>|<span data-ttu-id="b5ff5-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5ff5-123">Boolean</span></span>|<span data-ttu-id="b5ff5-124">コンプライアンス ポリシーが Intune によって管理されているかどうか</span><span class="sxs-lookup"><span data-stu-id="b5ff5-124">Whether compliance policy is managed by Intune</span></span>|
|<span data-ttu-id="b5ff5-125">windowsUpdateForBusiness</span><span class="sxs-lookup"><span data-stu-id="b5ff5-125">windowsUpdateForBusiness</span></span>|<span data-ttu-id="b5ff5-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5ff5-126">Boolean</span></span>|<span data-ttu-id="b5ff5-127">Windows Update for Business が Intune によって管理されているかどうか</span><span class="sxs-lookup"><span data-stu-id="b5ff5-127">Whether Windows Update for Business is managed by Intune</span></span>|

## <a name="relationships"></a><span data-ttu-id="b5ff5-128">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="b5ff5-128">Relationships</span></span>
<span data-ttu-id="b5ff5-129">なし</span><span class="sxs-lookup"><span data-stu-id="b5ff5-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b5ff5-130">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b5ff5-130">JSON Representation</span></span>
<span data-ttu-id="b5ff5-131">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="b5ff5-131">Here is a JSON representation of the resource.</span></span>
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



