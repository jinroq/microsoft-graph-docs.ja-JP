---
title: iosVppAppRevokeLicensesActionResult リソースの種類
description: ActionResult の継承されたプロパティが含まれています、iOS Vpp のアプリケーションでの操作の結果を定義します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 1f64f2df709d5332be46dd76216b1a1457d27a61
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29418905"
---
# <a name="iosvppapprevokelicensesactionresult-resource-type"></a><span data-ttu-id="4db85-103">iosVppAppRevokeLicensesActionResult リソースの種類</span><span class="sxs-lookup"><span data-stu-id="4db85-103">iosVppAppRevokeLicensesActionResult resource type</span></span>

> <span data-ttu-id="4db85-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="4db85-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="4db85-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4db85-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4db85-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="4db85-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4db85-107">ActionResult の継承されたプロパティが含まれています、iOS Vpp のアプリケーションでの操作の結果を定義します。</span><span class="sxs-lookup"><span data-stu-id="4db85-107">Defines results for actions on iOS Vpp Apps, contains inherited properties for ActionResult.</span></span>

## <a name="properties"></a><span data-ttu-id="4db85-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4db85-108">Properties</span></span>
|<span data-ttu-id="4db85-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4db85-109">Property</span></span>|<span data-ttu-id="4db85-110">型</span><span class="sxs-lookup"><span data-stu-id="4db85-110">Type</span></span>|<span data-ttu-id="4db85-111">説明</span><span class="sxs-lookup"><span data-stu-id="4db85-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4db85-112">userId</span><span class="sxs-lookup"><span data-stu-id="4db85-112">userId</span></span>|<span data-ttu-id="4db85-113">String</span><span class="sxs-lookup"><span data-stu-id="4db85-113">String</span></span>|<span data-ttu-id="4db85-114">アクションに関連付けられているユーザーの Id。</span><span class="sxs-lookup"><span data-stu-id="4db85-114">UserId associated with the action.</span></span>|
|<span data-ttu-id="4db85-115">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="4db85-115">managedDeviceId</span></span>|<span data-ttu-id="4db85-116">String</span><span class="sxs-lookup"><span data-stu-id="4db85-116">String</span></span>|<span data-ttu-id="4db85-117">DeviceId はアクションに関連付けられています。</span><span class="sxs-lookup"><span data-stu-id="4db85-117">DeviceId associated with the action.</span></span>|
|<span data-ttu-id="4db85-118">totalLicensesCount</span><span class="sxs-lookup"><span data-stu-id="4db85-118">totalLicensesCount</span></span>|<span data-ttu-id="4db85-119">Int32</span><span class="sxs-lookup"><span data-stu-id="4db85-119">Int32</span></span>|<span data-ttu-id="4db85-120">取り消しが実行しようとするライセンス数のカウントです。</span><span class="sxs-lookup"><span data-stu-id="4db85-120">A count of the number of licenses for which revoke was attempted.</span></span>|
|<span data-ttu-id="4db85-121">failedLicensesCount</span><span class="sxs-lookup"><span data-stu-id="4db85-121">failedLicensesCount</span></span>|<span data-ttu-id="4db85-122">Int32</span><span class="sxs-lookup"><span data-stu-id="4db85-122">Int32</span></span>|<span data-ttu-id="4db85-123">失敗する revoke のライセンス数のカウントです。</span><span class="sxs-lookup"><span data-stu-id="4db85-123">A count of the number of licenses for which revoke failed.</span></span>|
|<span data-ttu-id="4db85-124">actionFailureReason</span><span class="sxs-lookup"><span data-stu-id="4db85-124">actionFailureReason</span></span>|[<span data-ttu-id="4db85-125">vppTokenActionFailureReason</span><span class="sxs-lookup"><span data-stu-id="4db85-125">vppTokenActionFailureReason</span></span>](../resources/intune-shared-vpptokenactionfailurereason.md)|<span data-ttu-id="4db85-126">取り消しライセンス操作が失敗した理由です。</span><span class="sxs-lookup"><span data-stu-id="4db85-126">The reason for the revoke licenses action failure.</span></span> <span data-ttu-id="4db85-127">可能な値は、`none`、`appleFailure`、`internalError`、`expiredVppToken`、`expiredApplePushNotificationCertificate` です。</span><span class="sxs-lookup"><span data-stu-id="4db85-127">Possible values are: `none`, `appleFailure`, `internalError`, `expiredVppToken`, `expiredApplePushNotificationCertificate`.</span></span>|
|<span data-ttu-id="4db85-128">actionName</span><span class="sxs-lookup"><span data-stu-id="4db85-128">actionName</span></span>|<span data-ttu-id="4db85-129">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="4db85-129">String</span></span>|<span data-ttu-id="4db85-130">アクション名</span><span class="sxs-lookup"><span data-stu-id="4db85-130">Action name</span></span>|
|<span data-ttu-id="4db85-131">actionState</span><span class="sxs-lookup"><span data-stu-id="4db85-131">actionState</span></span>|[<span data-ttu-id="4db85-132">actionState</span><span class="sxs-lookup"><span data-stu-id="4db85-132">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="4db85-133">アクションの状態です。</span><span class="sxs-lookup"><span data-stu-id="4db85-133">State of the action.</span></span> <span data-ttu-id="4db85-134">可能な値は、`none`、`pending`、`canceled`、`active`、`done`、`failed`、`notSupported` です。</span><span class="sxs-lookup"><span data-stu-id="4db85-134">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="4db85-135">startDateTime</span><span class="sxs-lookup"><span data-stu-id="4db85-135">startDateTime</span></span>|<span data-ttu-id="4db85-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4db85-136">DateTimeOffset</span></span>|<span data-ttu-id="4db85-137">アクションが開始された時刻</span><span class="sxs-lookup"><span data-stu-id="4db85-137">Time the action was initiated</span></span>|
|<span data-ttu-id="4db85-138">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="4db85-138">lastUpdatedDateTime</span></span>|<span data-ttu-id="4db85-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4db85-139">DateTimeOffset</span></span>|<span data-ttu-id="4db85-140">アクション状態の最終更新時刻</span><span class="sxs-lookup"><span data-stu-id="4db85-140">Time the action state was last updated</span></span>|

## <a name="relationships"></a><span data-ttu-id="4db85-141">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="4db85-141">Relationships</span></span>
<span data-ttu-id="4db85-142">なし</span><span class="sxs-lookup"><span data-stu-id="4db85-142">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4db85-143">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="4db85-143">JSON Representation</span></span>
<span data-ttu-id="4db85-144">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="4db85-144">Here is a JSON representation of the resource.</span></span>
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




