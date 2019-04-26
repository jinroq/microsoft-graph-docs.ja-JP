---
title: mobileAppRelationshipState リソースの種類
description: UPN とデバイス id のコンテキストでの子アプリのインストール状態の詳細について説明します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e7f3dcbbc2544a4231cd5da102985d7142feb03a
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32551800"
---
# <a name="mobileapprelationshipstate-resource-type"></a><span data-ttu-id="09fbe-103">mobileAppRelationshipState リソースの種類</span><span class="sxs-lookup"><span data-stu-id="09fbe-103">mobileAppRelationshipState resource type</span></span>

> <span data-ttu-id="09fbe-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="09fbe-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="09fbe-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="09fbe-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="09fbe-106">UPN とデバイス id のコンテキストでの子アプリのインストール状態の詳細について説明します。</span><span class="sxs-lookup"><span data-stu-id="09fbe-106">Describes the installation status details of the child app in the context of UPN and device id.</span></span>

## <a name="properties"></a><span data-ttu-id="09fbe-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="09fbe-107">Properties</span></span>
|<span data-ttu-id="09fbe-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="09fbe-108">Property</span></span>|<span data-ttu-id="09fbe-109">型</span><span class="sxs-lookup"><span data-stu-id="09fbe-109">Type</span></span>|<span data-ttu-id="09fbe-110">説明</span><span class="sxs-lookup"><span data-stu-id="09fbe-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="09fbe-111">sourceIds</span><span class="sxs-lookup"><span data-stu-id="09fbe-111">sourceIds</span></span>|<span data-ttu-id="09fbe-112">String collection</span><span class="sxs-lookup"><span data-stu-id="09fbe-112">String collection</span></span>|<span data-ttu-id="09fbe-113">送信元モバイルアプリの id のコレクション。</span><span class="sxs-lookup"><span data-stu-id="09fbe-113">The collection of source mobile app's ids.</span></span>|
|<span data-ttu-id="09fbe-114">targetId</span><span class="sxs-lookup"><span data-stu-id="09fbe-114">targetId</span></span>|<span data-ttu-id="09fbe-115">String</span><span class="sxs-lookup"><span data-stu-id="09fbe-115">String</span></span>|<span data-ttu-id="09fbe-116">関連するターゲットアプリの id。</span><span class="sxs-lookup"><span data-stu-id="09fbe-116">The related target app's id.</span></span>|
|<span data-ttu-id="09fbe-117">targetdisplayname</span><span class="sxs-lookup"><span data-stu-id="09fbe-117">targetDisplayName</span></span>|<span data-ttu-id="09fbe-118">String</span><span class="sxs-lookup"><span data-stu-id="09fbe-118">String</span></span>|<span data-ttu-id="09fbe-119">関連するターゲットアプリの表示名。</span><span class="sxs-lookup"><span data-stu-id="09fbe-119">The related target app's display name.</span></span>|
|<span data-ttu-id="09fbe-120">deviceId</span><span class="sxs-lookup"><span data-stu-id="09fbe-120">deviceId</span></span>|<span data-ttu-id="09fbe-121">String</span><span class="sxs-lookup"><span data-stu-id="09fbe-121">String</span></span>|<span data-ttu-id="09fbe-122">対応するデバイス id。</span><span class="sxs-lookup"><span data-stu-id="09fbe-122">The corresponding device id.</span></span>|
|<span data-ttu-id="09fbe-123">installState</span><span class="sxs-lookup"><span data-stu-id="09fbe-123">installState</span></span>|[<span data-ttu-id="09fbe-124">resultappstate</span><span class="sxs-lookup"><span data-stu-id="09fbe-124">resultantAppState</span></span>](../resources/intune-shared-resultantappstate.md)|<span data-ttu-id="09fbe-125">ターゲットアプリのアプリのインストール状態。</span><span class="sxs-lookup"><span data-stu-id="09fbe-125">The install state of the app of target app.</span></span> <span data-ttu-id="09fbe-126">可能な値は、`installed`、`failed`、`notInstalled`、`uninstallFailed`、`pendingInstall`、`unknown`、`notApplicable` です。</span><span class="sxs-lookup"><span data-stu-id="09fbe-126">Possible values are: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span></span>|
|<span data-ttu-id="09fbe-127">installstatedetail</span><span class="sxs-lookup"><span data-stu-id="09fbe-127">installStateDetail</span></span>|[<span data-ttu-id="09fbe-128">resultantAppStateDetail</span><span class="sxs-lookup"><span data-stu-id="09fbe-128">resultantAppStateDetail</span></span>](../resources/intune-apps-resultantappstatedetail.md)|<span data-ttu-id="09fbe-129">アプリのインストール状態の詳細。</span><span class="sxs-lookup"><span data-stu-id="09fbe-129">The install state detail of the app.</span></span> <span data-ttu-id="09fbe-130">可能な値: `noAdditionalDetails`、 `dependencyFailedToInstall` `dependencyWithRequirementsNotMet` `dependencyPendingReboot` `dependencyWithAutoInstallDisabled` `seeInstallErrorCode` `autoInstallDisabled` `seeUninstallErrorCode` `pendingReboot` `installingDependencies` `powerShellScriptRequirementNotMet` `registryRequirementNotMet`、、、、、、、、、、、、 `fileSystemRequirementNotMet` `platformNotApplicable` `minimumCpuSpeedNotMet` `minimumLogicalProcessorCountNotMet` `minimumPhysicalMemoryNotMet` `minimumOsVersionNotMet` `minimumDiskSpaceNotMet`, `processorArchitectureNotApplicable`.</span><span class="sxs-lookup"><span data-stu-id="09fbe-130">Possible values are: `noAdditionalDetails`, `dependencyFailedToInstall`, `dependencyWithRequirementsNotMet`, `dependencyPendingReboot`, `dependencyWithAutoInstallDisabled`, `seeInstallErrorCode`, `autoInstallDisabled`, `seeUninstallErrorCode`, `pendingReboot`, `installingDependencies`, `powerShellScriptRequirementNotMet`, `registryRequirementNotMet`, `fileSystemRequirementNotMet`, `platformNotApplicable`, `minimumCpuSpeedNotMet`, `minimumLogicalProcessorCountNotMet`, `minimumPhysicalMemoryNotMet`, `minimumOsVersionNotMet`, `minimumDiskSpaceNotMet`, `processorArchitectureNotApplicable`.</span></span>|
|<span data-ttu-id="09fbe-131">errorCode</span><span class="sxs-lookup"><span data-stu-id="09fbe-131">errorCode</span></span>|<span data-ttu-id="09fbe-132">Int32</span><span class="sxs-lookup"><span data-stu-id="09fbe-132">Int32</span></span>|<span data-ttu-id="09fbe-133">ターゲットアプリのインストールまたはアンインストールに失敗した場合のエラーコード。</span><span class="sxs-lookup"><span data-stu-id="09fbe-133">The error code for install or uninstall failures of target app.</span></span>|
|<span data-ttu-id="09fbe-134">targetlastsyncdatetime</span><span class="sxs-lookup"><span data-stu-id="09fbe-134">targetLastSyncDateTime</span></span>|<span data-ttu-id="09fbe-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="09fbe-135">DateTimeOffset</span></span>|<span data-ttu-id="09fbe-136">ターゲットアプリの最終同期時刻。</span><span class="sxs-lookup"><span data-stu-id="09fbe-136">The last sync time of the target app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="09fbe-137">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="09fbe-137">Relationships</span></span>
<span data-ttu-id="09fbe-138">なし</span><span class="sxs-lookup"><span data-stu-id="09fbe-138">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="09fbe-139">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="09fbe-139">JSON Representation</span></span>
<span data-ttu-id="09fbe-140">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="09fbe-140">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mobileAppRelationshipState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppRelationshipState",
  "sourceIds": [
    "String"
  ],
  "targetId": "String",
  "targetDisplayName": "String",
  "deviceId": "String",
  "installState": "String",
  "installStateDetail": "String",
  "errorCode": 1024,
  "targetLastSyncDateTime": "String (timestamp)"
}
```





