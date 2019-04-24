---
title: configurationManagerClientEnabledFeatures リソースの種類
description: 構成マネージャーのクライアントに対応した機能
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 91ffd0180660b33e9ead5210f9b23870af18e29a
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32467310"
---
# <a name="configurationmanagerclientenabledfeatures-resource-type"></a><span data-ttu-id="69cb6-103">configurationManagerClientEnabledFeatures リソースの種類</span><span class="sxs-lookup"><span data-stu-id="69cb6-103">configurationManagerClientEnabledFeatures resource type</span></span>

> <span data-ttu-id="69cb6-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="69cb6-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="69cb6-105">構成マネージャーのクライアントに対応した機能</span><span class="sxs-lookup"><span data-stu-id="69cb6-105">configuration Manager client enabled features</span></span>

## <a name="properties"></a><span data-ttu-id="69cb6-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="69cb6-106">Properties</span></span>
|<span data-ttu-id="69cb6-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="69cb6-107">Property</span></span>|<span data-ttu-id="69cb6-108">型</span><span class="sxs-lookup"><span data-stu-id="69cb6-108">Type</span></span>|<span data-ttu-id="69cb6-109">説明</span><span class="sxs-lookup"><span data-stu-id="69cb6-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="69cb6-110">inventory</span><span class="sxs-lookup"><span data-stu-id="69cb6-110">inventory</span></span>|<span data-ttu-id="69cb6-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="69cb6-111">Boolean</span></span>|<span data-ttu-id="69cb6-112">在庫が Intune によって管理されているかどうか</span><span class="sxs-lookup"><span data-stu-id="69cb6-112">Whether inventory is managed by Intune</span></span>|
|<span data-ttu-id="69cb6-113">modernApps</span><span class="sxs-lookup"><span data-stu-id="69cb6-113">modernApps</span></span>|<span data-ttu-id="69cb6-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="69cb6-114">Boolean</span></span>|<span data-ttu-id="69cb6-115">モダン アプリケーションが Intune によって管理されているかどうか</span><span class="sxs-lookup"><span data-stu-id="69cb6-115">Whether modern application is managed by Intune</span></span>|
|<span data-ttu-id="69cb6-116">resourceAccess</span><span class="sxs-lookup"><span data-stu-id="69cb6-116">resourceAccess</span></span>|<span data-ttu-id="69cb6-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="69cb6-117">Boolean</span></span>|<span data-ttu-id="69cb6-118">リソース アクセスが Intune によって管理されているかどうか</span><span class="sxs-lookup"><span data-stu-id="69cb6-118">Whether resource access is managed by Intune</span></span>|
|<span data-ttu-id="69cb6-119">deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="69cb6-119">deviceConfiguration</span></span>|<span data-ttu-id="69cb6-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="69cb6-120">Boolean</span></span>|<span data-ttu-id="69cb6-121">デバイス構成が Intune によって管理されているかどうか</span><span class="sxs-lookup"><span data-stu-id="69cb6-121">Whether device configuration is managed by Intune</span></span>|
|<span data-ttu-id="69cb6-122">compliancePolicy</span><span class="sxs-lookup"><span data-stu-id="69cb6-122">compliancePolicy</span></span>|<span data-ttu-id="69cb6-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="69cb6-123">Boolean</span></span>|<span data-ttu-id="69cb6-124">コンプライアンス ポリシーが Intune によって管理されているかどうか</span><span class="sxs-lookup"><span data-stu-id="69cb6-124">Whether compliance policy is managed by Intune</span></span>|
|<span data-ttu-id="69cb6-125">windowsUpdateForBusiness</span><span class="sxs-lookup"><span data-stu-id="69cb6-125">windowsUpdateForBusiness</span></span>|<span data-ttu-id="69cb6-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="69cb6-126">Boolean</span></span>|<span data-ttu-id="69cb6-127">Windows Update for Business が Intune によって管理されているかどうか</span><span class="sxs-lookup"><span data-stu-id="69cb6-127">Whether Windows Update for Business is managed by Intune</span></span>|

## <a name="relationships"></a><span data-ttu-id="69cb6-128">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="69cb6-128">Relationships</span></span>
<span data-ttu-id="69cb6-129">なし</span><span class="sxs-lookup"><span data-stu-id="69cb6-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="69cb6-130">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="69cb6-130">JSON Representation</span></span>
<span data-ttu-id="69cb6-131">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="69cb6-131">Here is a JSON representation of the resource.</span></span>
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



