---
title: iosVppAppRevokeLicensesActionResult リソースの種類
description: IOS Vpp アプリでのアクションの結果を定義します。 ActionResult の継承されたプロパティが含まれています。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6e28e21baa4dc0461d9b54f206810a969a153c15
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33950243"
---
# <a name="iosvppapprevokelicensesactionresult-resource-type"></a><span data-ttu-id="5d0a1-103">iosVppAppRevokeLicensesActionResult リソースの種類</span><span class="sxs-lookup"><span data-stu-id="5d0a1-103">iosVppAppRevokeLicensesActionResult resource type</span></span>

> <span data-ttu-id="5d0a1-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5d0a1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5d0a1-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="5d0a1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5d0a1-106">IOS Vpp アプリでのアクションの結果を定義します。 ActionResult の継承されたプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="5d0a1-106">Defines results for actions on iOS Vpp Apps, contains inherited properties for ActionResult.</span></span>

## <a name="properties"></a><span data-ttu-id="5d0a1-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5d0a1-107">Properties</span></span>
|<span data-ttu-id="5d0a1-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5d0a1-108">Property</span></span>|<span data-ttu-id="5d0a1-109">型</span><span class="sxs-lookup"><span data-stu-id="5d0a1-109">Type</span></span>|<span data-ttu-id="5d0a1-110">説明</span><span class="sxs-lookup"><span data-stu-id="5d0a1-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5d0a1-111">userId</span><span class="sxs-lookup"><span data-stu-id="5d0a1-111">userId</span></span>|<span data-ttu-id="5d0a1-112">String</span><span class="sxs-lookup"><span data-stu-id="5d0a1-112">String</span></span>|<span data-ttu-id="5d0a1-113">アクションに関連付けられている UserId。</span><span class="sxs-lookup"><span data-stu-id="5d0a1-113">UserId associated with the action.</span></span>|
|<span data-ttu-id="5d0a1-114">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="5d0a1-114">managedDeviceId</span></span>|<span data-ttu-id="5d0a1-115">String</span><span class="sxs-lookup"><span data-stu-id="5d0a1-115">String</span></span>|<span data-ttu-id="5d0a1-116">アクションに関連付けられている DeviceId。</span><span class="sxs-lookup"><span data-stu-id="5d0a1-116">DeviceId associated with the action.</span></span>|
|<span data-ttu-id="5d0a1-117">合計の合計数</span><span class="sxs-lookup"><span data-stu-id="5d0a1-117">totalLicensesCount</span></span>|<span data-ttu-id="5d0a1-118">Int32</span><span class="sxs-lookup"><span data-stu-id="5d0a1-118">Int32</span></span>|<span data-ttu-id="5d0a1-119">取り消しが試行されたライセンスの数。</span><span class="sxs-lookup"><span data-stu-id="5d0a1-119">A count of the number of licenses for which revoke was attempted.</span></span>|
|<span data-ttu-id="5d0a1-120">failedLicensesCount</span><span class="sxs-lookup"><span data-stu-id="5d0a1-120">failedLicensesCount</span></span>|<span data-ttu-id="5d0a1-121">Int32</span><span class="sxs-lookup"><span data-stu-id="5d0a1-121">Int32</span></span>|<span data-ttu-id="5d0a1-122">失効に失敗したライセンスの数。</span><span class="sxs-lookup"><span data-stu-id="5d0a1-122">A count of the number of licenses for which revoke failed.</span></span>|
|<span data-ttu-id="5d0a1-123">actionFailureReason</span><span class="sxs-lookup"><span data-stu-id="5d0a1-123">actionFailureReason</span></span>|[<span data-ttu-id="5d0a1-124">vppTokenActionFailureReason</span><span class="sxs-lookup"><span data-stu-id="5d0a1-124">vppTokenActionFailureReason</span></span>](../resources/intune-shared-vpptokenactionfailurereason.md)|<span data-ttu-id="5d0a1-125">失効ライセンスの処理の失敗の理由。</span><span class="sxs-lookup"><span data-stu-id="5d0a1-125">The reason for the revoke licenses action failure.</span></span> <span data-ttu-id="5d0a1-126">可能な値は、`none`、`appleFailure`、`internalError`、`expiredVppToken`、`expiredApplePushNotificationCertificate` です。</span><span class="sxs-lookup"><span data-stu-id="5d0a1-126">Possible values are: `none`, `appleFailure`, `internalError`, `expiredVppToken`, `expiredApplePushNotificationCertificate`.</span></span>|
|<span data-ttu-id="5d0a1-127">actionName</span><span class="sxs-lookup"><span data-stu-id="5d0a1-127">actionName</span></span>|<span data-ttu-id="5d0a1-128">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="5d0a1-128">String</span></span>|<span data-ttu-id="5d0a1-129">アクション名</span><span class="sxs-lookup"><span data-stu-id="5d0a1-129">Action name</span></span>|
|<span data-ttu-id="5d0a1-130">actionState</span><span class="sxs-lookup"><span data-stu-id="5d0a1-130">actionState</span></span>|[<span data-ttu-id="5d0a1-131">actionState</span><span class="sxs-lookup"><span data-stu-id="5d0a1-131">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="5d0a1-132">アクションの状態。</span><span class="sxs-lookup"><span data-stu-id="5d0a1-132">State of the action.</span></span> <span data-ttu-id="5d0a1-133">可能な値は、`none`、`pending`、`canceled`、`active`、`done`、`failed`、`notSupported` です。</span><span class="sxs-lookup"><span data-stu-id="5d0a1-133">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="5d0a1-134">startDateTime</span><span class="sxs-lookup"><span data-stu-id="5d0a1-134">startDateTime</span></span>|<span data-ttu-id="5d0a1-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5d0a1-135">DateTimeOffset</span></span>|<span data-ttu-id="5d0a1-136">アクションが開始された時刻</span><span class="sxs-lookup"><span data-stu-id="5d0a1-136">Time the action was initiated</span></span>|
|<span data-ttu-id="5d0a1-137">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="5d0a1-137">lastUpdatedDateTime</span></span>|<span data-ttu-id="5d0a1-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5d0a1-138">DateTimeOffset</span></span>|<span data-ttu-id="5d0a1-139">アクション状態の最終更新時刻</span><span class="sxs-lookup"><span data-stu-id="5d0a1-139">Time the action state was last updated</span></span>|

## <a name="relationships"></a><span data-ttu-id="5d0a1-140">関係</span><span class="sxs-lookup"><span data-stu-id="5d0a1-140">Relationships</span></span>
<span data-ttu-id="5d0a1-141">なし</span><span class="sxs-lookup"><span data-stu-id="5d0a1-141">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5d0a1-142">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="5d0a1-142">JSON Representation</span></span>
<span data-ttu-id="5d0a1-143">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="5d0a1-143">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosVppAppRevokeLicensesActionResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosVppAppRevokeLicensesActionResult",
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




