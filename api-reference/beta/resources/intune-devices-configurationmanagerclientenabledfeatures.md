---
title: configurationManagerClientEnabledFeatures リソースの種類
description: 構成マネージャーのクライアントに対応した機能
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 7975130bb047e097ea0d52a4ce770fb35e4efa32
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425905"
---
# <a name="configurationmanagerclientenabledfeatures-resource-type"></a><span data-ttu-id="ea263-103">configurationManagerClientEnabledFeatures リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ea263-103">configurationManagerClientEnabledFeatures resource type</span></span>

> <span data-ttu-id="ea263-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="ea263-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="ea263-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ea263-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ea263-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="ea263-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ea263-107">構成マネージャーのクライアントに対応した機能</span><span class="sxs-lookup"><span data-stu-id="ea263-107">configuration Manager client enabled features</span></span>

## <a name="properties"></a><span data-ttu-id="ea263-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ea263-108">Properties</span></span>
|<span data-ttu-id="ea263-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ea263-109">Property</span></span>|<span data-ttu-id="ea263-110">型</span><span class="sxs-lookup"><span data-stu-id="ea263-110">Type</span></span>|<span data-ttu-id="ea263-111">説明</span><span class="sxs-lookup"><span data-stu-id="ea263-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ea263-112">inventory</span><span class="sxs-lookup"><span data-stu-id="ea263-112">inventory</span></span>|<span data-ttu-id="ea263-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="ea263-113">Boolean</span></span>|<span data-ttu-id="ea263-114">在庫が Intune によって管理されているかどうか</span><span class="sxs-lookup"><span data-stu-id="ea263-114">Whether inventory is managed by Intune</span></span>|
|<span data-ttu-id="ea263-115">modernApps</span><span class="sxs-lookup"><span data-stu-id="ea263-115">modernApps</span></span>|<span data-ttu-id="ea263-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="ea263-116">Boolean</span></span>|<span data-ttu-id="ea263-117">モダン アプリケーションが Intune によって管理されているかどうか</span><span class="sxs-lookup"><span data-stu-id="ea263-117">Whether modern application is managed by Intune</span></span>|
|<span data-ttu-id="ea263-118">resourceAccess</span><span class="sxs-lookup"><span data-stu-id="ea263-118">resourceAccess</span></span>|<span data-ttu-id="ea263-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="ea263-119">Boolean</span></span>|<span data-ttu-id="ea263-120">リソース アクセスが Intune によって管理されているかどうか</span><span class="sxs-lookup"><span data-stu-id="ea263-120">Whether resource access is managed by Intune</span></span>|
|<span data-ttu-id="ea263-121">deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="ea263-121">deviceConfiguration</span></span>|<span data-ttu-id="ea263-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="ea263-122">Boolean</span></span>|<span data-ttu-id="ea263-123">デバイス構成が Intune によって管理されているかどうか</span><span class="sxs-lookup"><span data-stu-id="ea263-123">Whether device configuration is managed by Intune</span></span>|
|<span data-ttu-id="ea263-124">compliancePolicy</span><span class="sxs-lookup"><span data-stu-id="ea263-124">compliancePolicy</span></span>|<span data-ttu-id="ea263-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="ea263-125">Boolean</span></span>|<span data-ttu-id="ea263-126">コンプライアンス ポリシーが Intune によって管理されているかどうか</span><span class="sxs-lookup"><span data-stu-id="ea263-126">Whether compliance policy is managed by Intune</span></span>|
|<span data-ttu-id="ea263-127">windowsUpdateForBusiness</span><span class="sxs-lookup"><span data-stu-id="ea263-127">windowsUpdateForBusiness</span></span>|<span data-ttu-id="ea263-128">Boolean</span><span class="sxs-lookup"><span data-stu-id="ea263-128">Boolean</span></span>|<span data-ttu-id="ea263-129">Windows Update for Business が Intune によって管理されているかどうか</span><span class="sxs-lookup"><span data-stu-id="ea263-129">Whether Windows Update for Business is managed by Intune</span></span>|

## <a name="relationships"></a><span data-ttu-id="ea263-130">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="ea263-130">Relationships</span></span>
<span data-ttu-id="ea263-131">なし</span><span class="sxs-lookup"><span data-stu-id="ea263-131">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ea263-132">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ea263-132">JSON Representation</span></span>
<span data-ttu-id="ea263-133">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="ea263-133">Here is a JSON representation of the resource.</span></span>
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




