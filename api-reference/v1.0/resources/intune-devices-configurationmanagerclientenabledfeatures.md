---
title: configurationManagerClientEnabledFeatures リソースの種類
description: 構成マネージャーのクライアントに対応した機能
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 91ffd0180660b33e9ead5210f9b23870af18e29a
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30264422"
---
# <a name="configurationmanagerclientenabledfeatures-resource-type"></a><span data-ttu-id="b5658-103">configurationManagerClientEnabledFeatures リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b5658-103">configurationManagerClientEnabledFeatures resource type</span></span>

> <span data-ttu-id="b5658-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="b5658-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b5658-105">構成マネージャーのクライアントに対応した機能</span><span class="sxs-lookup"><span data-stu-id="b5658-105">configuration Manager client enabled features</span></span>

## <a name="properties"></a><span data-ttu-id="b5658-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b5658-106">Properties</span></span>
|<span data-ttu-id="b5658-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b5658-107">Property</span></span>|<span data-ttu-id="b5658-108">型</span><span class="sxs-lookup"><span data-stu-id="b5658-108">Type</span></span>|<span data-ttu-id="b5658-109">説明</span><span class="sxs-lookup"><span data-stu-id="b5658-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b5658-110">inventory</span><span class="sxs-lookup"><span data-stu-id="b5658-110">inventory</span></span>|<span data-ttu-id="b5658-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5658-111">Boolean</span></span>|<span data-ttu-id="b5658-112">在庫が Intune によって管理されているかどうか</span><span class="sxs-lookup"><span data-stu-id="b5658-112">Whether inventory is managed by Intune</span></span>|
|<span data-ttu-id="b5658-113">modernApps</span><span class="sxs-lookup"><span data-stu-id="b5658-113">modernApps</span></span>|<span data-ttu-id="b5658-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5658-114">Boolean</span></span>|<span data-ttu-id="b5658-115">モダン アプリケーションが Intune によって管理されているかどうか</span><span class="sxs-lookup"><span data-stu-id="b5658-115">Whether modern application is managed by Intune</span></span>|
|<span data-ttu-id="b5658-116">resourceAccess</span><span class="sxs-lookup"><span data-stu-id="b5658-116">resourceAccess</span></span>|<span data-ttu-id="b5658-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5658-117">Boolean</span></span>|<span data-ttu-id="b5658-118">リソース アクセスが Intune によって管理されているかどうか</span><span class="sxs-lookup"><span data-stu-id="b5658-118">Whether resource access is managed by Intune</span></span>|
|<span data-ttu-id="b5658-119">deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="b5658-119">deviceConfiguration</span></span>|<span data-ttu-id="b5658-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5658-120">Boolean</span></span>|<span data-ttu-id="b5658-121">デバイス構成が Intune によって管理されているかどうか</span><span class="sxs-lookup"><span data-stu-id="b5658-121">Whether device configuration is managed by Intune</span></span>|
|<span data-ttu-id="b5658-122">compliancePolicy</span><span class="sxs-lookup"><span data-stu-id="b5658-122">compliancePolicy</span></span>|<span data-ttu-id="b5658-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5658-123">Boolean</span></span>|<span data-ttu-id="b5658-124">コンプライアンス ポリシーが Intune によって管理されているかどうか</span><span class="sxs-lookup"><span data-stu-id="b5658-124">Whether compliance policy is managed by Intune</span></span>|
|<span data-ttu-id="b5658-125">windowsUpdateForBusiness</span><span class="sxs-lookup"><span data-stu-id="b5658-125">windowsUpdateForBusiness</span></span>|<span data-ttu-id="b5658-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5658-126">Boolean</span></span>|<span data-ttu-id="b5658-127">Windows Update for Business が Intune によって管理されているかどうか</span><span class="sxs-lookup"><span data-stu-id="b5658-127">Whether Windows Update for Business is managed by Intune</span></span>|

## <a name="relationships"></a><span data-ttu-id="b5658-128">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="b5658-128">Relationships</span></span>
<span data-ttu-id="b5658-129">なし</span><span class="sxs-lookup"><span data-stu-id="b5658-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b5658-130">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b5658-130">JSON Representation</span></span>
<span data-ttu-id="b5658-131">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="b5658-131">Here is a JSON representation of the resource.</span></span>
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



