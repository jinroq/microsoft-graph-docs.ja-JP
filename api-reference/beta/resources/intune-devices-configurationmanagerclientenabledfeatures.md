---
title: configurationManagerClientEnabledFeatures リソースの種類
description: 構成マネージャーのクライアントに対応した機能
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7a90b7f0009b4d9bd617b781338ceee3de2f432c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32549133"
---
# <a name="configurationmanagerclientenabledfeatures-resource-type"></a><span data-ttu-id="a4643-103">configurationManagerClientEnabledFeatures リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a4643-103">configurationManagerClientEnabledFeatures resource type</span></span>

> <span data-ttu-id="a4643-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a4643-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a4643-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="a4643-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a4643-106">構成マネージャーのクライアントに対応した機能</span><span class="sxs-lookup"><span data-stu-id="a4643-106">configuration Manager client enabled features</span></span>

## <a name="properties"></a><span data-ttu-id="a4643-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a4643-107">Properties</span></span>
|<span data-ttu-id="a4643-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a4643-108">Property</span></span>|<span data-ttu-id="a4643-109">型</span><span class="sxs-lookup"><span data-stu-id="a4643-109">Type</span></span>|<span data-ttu-id="a4643-110">説明</span><span class="sxs-lookup"><span data-stu-id="a4643-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a4643-111">inventory</span><span class="sxs-lookup"><span data-stu-id="a4643-111">inventory</span></span>|<span data-ttu-id="a4643-112">ブール値</span><span class="sxs-lookup"><span data-stu-id="a4643-112">Boolean</span></span>|<span data-ttu-id="a4643-113">在庫が Intune によって管理されているかどうか</span><span class="sxs-lookup"><span data-stu-id="a4643-113">Whether inventory is managed by Intune</span></span>|
|<span data-ttu-id="a4643-114">modernApps</span><span class="sxs-lookup"><span data-stu-id="a4643-114">modernApps</span></span>|<span data-ttu-id="a4643-115">ブール値</span><span class="sxs-lookup"><span data-stu-id="a4643-115">Boolean</span></span>|<span data-ttu-id="a4643-116">モダン アプリケーションが Intune によって管理されているかどうか</span><span class="sxs-lookup"><span data-stu-id="a4643-116">Whether modern application is managed by Intune</span></span>|
|<span data-ttu-id="a4643-117">resourceAccess</span><span class="sxs-lookup"><span data-stu-id="a4643-117">resourceAccess</span></span>|<span data-ttu-id="a4643-118">ブール値</span><span class="sxs-lookup"><span data-stu-id="a4643-118">Boolean</span></span>|<span data-ttu-id="a4643-119">リソース アクセスが Intune によって管理されているかどうか</span><span class="sxs-lookup"><span data-stu-id="a4643-119">Whether resource access is managed by Intune</span></span>|
|<span data-ttu-id="a4643-120">deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="a4643-120">deviceConfiguration</span></span>|<span data-ttu-id="a4643-121">ブール値</span><span class="sxs-lookup"><span data-stu-id="a4643-121">Boolean</span></span>|<span data-ttu-id="a4643-122">デバイス構成が Intune によって管理されているかどうか</span><span class="sxs-lookup"><span data-stu-id="a4643-122">Whether device configuration is managed by Intune</span></span>|
|<span data-ttu-id="a4643-123">compliancePolicy</span><span class="sxs-lookup"><span data-stu-id="a4643-123">compliancePolicy</span></span>|<span data-ttu-id="a4643-124">ブール値</span><span class="sxs-lookup"><span data-stu-id="a4643-124">Boolean</span></span>|<span data-ttu-id="a4643-125">コンプライアンス ポリシーが Intune によって管理されているかどうか</span><span class="sxs-lookup"><span data-stu-id="a4643-125">Whether compliance policy is managed by Intune</span></span>|
|<span data-ttu-id="a4643-126">windowsUpdateForBusiness</span><span class="sxs-lookup"><span data-stu-id="a4643-126">windowsUpdateForBusiness</span></span>|<span data-ttu-id="a4643-127">Boolean</span><span class="sxs-lookup"><span data-stu-id="a4643-127">Boolean</span></span>|<span data-ttu-id="a4643-128">Windows Update for Business が Intune によって管理されているかどうか</span><span class="sxs-lookup"><span data-stu-id="a4643-128">Whether Windows Update for Business is managed by Intune</span></span>|
|<span data-ttu-id="a4643-129">endpointprotection</span><span class="sxs-lookup"><span data-stu-id="a4643-129">endpointProtection</span></span>|<span data-ttu-id="a4643-130">ブール値</span><span class="sxs-lookup"><span data-stu-id="a4643-130">Boolean</span></span>|<span data-ttu-id="a4643-131">エンドポイント保護が Intune によって管理されているかどうか</span><span class="sxs-lookup"><span data-stu-id="a4643-131">Whether Endpoint Protection is managed by Intune</span></span>|
|<span data-ttu-id="a4643-132">officeoffice</span><span class="sxs-lookup"><span data-stu-id="a4643-132">officeApps</span></span>|<span data-ttu-id="a4643-133">ブール値</span><span class="sxs-lookup"><span data-stu-id="a4643-133">Boolean</span></span>|<span data-ttu-id="a4643-134">Office アプリケーションが Intune によって管理されているかどうか</span><span class="sxs-lookup"><span data-stu-id="a4643-134">Whether Office application is managed by Intune</span></span>|

## <a name="relationships"></a><span data-ttu-id="a4643-135">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="a4643-135">Relationships</span></span>
<span data-ttu-id="a4643-136">なし</span><span class="sxs-lookup"><span data-stu-id="a4643-136">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a4643-137">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a4643-137">JSON Representation</span></span>
<span data-ttu-id="a4643-138">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="a4643-138">Here is a JSON representation of the resource.</span></span>
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





