---
title: macOsVppAppRevokeLicensesActionResult リソースの種類
description: MacOS Vpp アプリでのアクションの結果を定義します。 ActionResult の継承されたプロパティが含まれています。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: cd659ab07b5db81de4e8004461bc149c236ec576
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34989155"
---
# <a name="macosvppapprevokelicensesactionresult-resource-type"></a><span data-ttu-id="2e075-103">macOsVppAppRevokeLicensesActionResult リソースの種類</span><span class="sxs-lookup"><span data-stu-id="2e075-103">macOsVppAppRevokeLicensesActionResult resource type</span></span>

> <span data-ttu-id="2e075-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2e075-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2e075-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="2e075-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2e075-106">MacOS Vpp アプリでのアクションの結果を定義します。 ActionResult の継承されたプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="2e075-106">Defines results for actions on MacOS Vpp Apps, contains inherited properties for ActionResult.</span></span>

## <a name="properties"></a><span data-ttu-id="2e075-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2e075-107">Properties</span></span>
|<span data-ttu-id="2e075-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2e075-108">Property</span></span>|<span data-ttu-id="2e075-109">型</span><span class="sxs-lookup"><span data-stu-id="2e075-109">Type</span></span>|<span data-ttu-id="2e075-110">説明</span><span class="sxs-lookup"><span data-stu-id="2e075-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2e075-111">userId</span><span class="sxs-lookup"><span data-stu-id="2e075-111">userId</span></span>|<span data-ttu-id="2e075-112">String</span><span class="sxs-lookup"><span data-stu-id="2e075-112">String</span></span>|<span data-ttu-id="2e075-113">アクションに関連付けられている UserId。</span><span class="sxs-lookup"><span data-stu-id="2e075-113">UserId associated with the action.</span></span>|
|<span data-ttu-id="2e075-114">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="2e075-114">managedDeviceId</span></span>|<span data-ttu-id="2e075-115">String</span><span class="sxs-lookup"><span data-stu-id="2e075-115">String</span></span>|<span data-ttu-id="2e075-116">アクションに関連付けられている DeviceId。</span><span class="sxs-lookup"><span data-stu-id="2e075-116">DeviceId associated with the action.</span></span>|
|<span data-ttu-id="2e075-117">合計の合計数</span><span class="sxs-lookup"><span data-stu-id="2e075-117">totalLicensesCount</span></span>|<span data-ttu-id="2e075-118">Int32</span><span class="sxs-lookup"><span data-stu-id="2e075-118">Int32</span></span>|<span data-ttu-id="2e075-119">取り消しが試行されたライセンスの数。</span><span class="sxs-lookup"><span data-stu-id="2e075-119">A count of the number of licenses for which revoke was attempted.</span></span>|
|<span data-ttu-id="2e075-120">failedLicensesCount</span><span class="sxs-lookup"><span data-stu-id="2e075-120">failedLicensesCount</span></span>|<span data-ttu-id="2e075-121">Int32</span><span class="sxs-lookup"><span data-stu-id="2e075-121">Int32</span></span>|<span data-ttu-id="2e075-122">失効に失敗したライセンスの数。</span><span class="sxs-lookup"><span data-stu-id="2e075-122">A count of the number of licenses for which revoke failed.</span></span>|
|<span data-ttu-id="2e075-123">actionFailureReason</span><span class="sxs-lookup"><span data-stu-id="2e075-123">actionFailureReason</span></span>|[<span data-ttu-id="2e075-124">vppTokenActionFailureReason</span><span class="sxs-lookup"><span data-stu-id="2e075-124">vppTokenActionFailureReason</span></span>](../resources/intune-shared-vpptokenactionfailurereason.md)|<span data-ttu-id="2e075-125">失効ライセンスの処理の失敗の理由。</span><span class="sxs-lookup"><span data-stu-id="2e075-125">The reason for the revoke licenses action failure.</span></span> <span data-ttu-id="2e075-126">可能な値は、`none`、`appleFailure`、`internalError`、`expiredVppToken`、`expiredApplePushNotificationCertificate` です。</span><span class="sxs-lookup"><span data-stu-id="2e075-126">Possible values are: `none`, `appleFailure`, `internalError`, `expiredVppToken`, `expiredApplePushNotificationCertificate`.</span></span>|
|<span data-ttu-id="2e075-127">actionName</span><span class="sxs-lookup"><span data-stu-id="2e075-127">actionName</span></span>|<span data-ttu-id="2e075-128">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="2e075-128">String</span></span>|<span data-ttu-id="2e075-129">アクション名</span><span class="sxs-lookup"><span data-stu-id="2e075-129">Action name</span></span>|
|<span data-ttu-id="2e075-130">actionState</span><span class="sxs-lookup"><span data-stu-id="2e075-130">actionState</span></span>|[<span data-ttu-id="2e075-131">actionState</span><span class="sxs-lookup"><span data-stu-id="2e075-131">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="2e075-132">アクションの状態。</span><span class="sxs-lookup"><span data-stu-id="2e075-132">State of the action.</span></span> <span data-ttu-id="2e075-133">可能な値は、`none`、`pending`、`canceled`、`active`、`done`、`failed`、`notSupported` です。</span><span class="sxs-lookup"><span data-stu-id="2e075-133">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="2e075-134">startDateTime</span><span class="sxs-lookup"><span data-stu-id="2e075-134">startDateTime</span></span>|<span data-ttu-id="2e075-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2e075-135">DateTimeOffset</span></span>|<span data-ttu-id="2e075-136">アクションが開始された時刻</span><span class="sxs-lookup"><span data-stu-id="2e075-136">Time the action was initiated</span></span>|
|<span data-ttu-id="2e075-137">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="2e075-137">lastUpdatedDateTime</span></span>|<span data-ttu-id="2e075-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2e075-138">DateTimeOffset</span></span>|<span data-ttu-id="2e075-139">アクション状態の最終更新時刻</span><span class="sxs-lookup"><span data-stu-id="2e075-139">Time the action state was last updated</span></span>|

## <a name="relationships"></a><span data-ttu-id="2e075-140">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="2e075-140">Relationships</span></span>
<span data-ttu-id="2e075-141">なし</span><span class="sxs-lookup"><span data-stu-id="2e075-141">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2e075-142">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="2e075-142">JSON Representation</span></span>
<span data-ttu-id="2e075-143">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="2e075-143">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.macOsVppAppRevokeLicensesActionResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOsVppAppRevokeLicensesActionResult",
  "userId": "String",
  "managedDeviceId": "String",
  "totalLicensesCount": 1024,
  "failedLicensesCount": 1024,
  "actionFailureReason": "String",
  "actionName": "String",
  "actionState": "String",
  "startDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)"
}
```





