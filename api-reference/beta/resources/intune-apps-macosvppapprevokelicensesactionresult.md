---
title: macOsVppAppRevokeLicensesActionResult リソースの種類
description: MacOS Vpp アプリでのアクションの結果を定義します。 actionresult の継承されたプロパティが含まれています。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7cf8390dc2c1541525e288b81defd073144f4132
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30166508"
---
# <a name="macosvppapprevokelicensesactionresult-resource-type"></a><span data-ttu-id="06d38-103">macOsVppAppRevokeLicensesActionResult リソースの種類</span><span class="sxs-lookup"><span data-stu-id="06d38-103">macOsVppAppRevokeLicensesActionResult resource type</span></span>

> <span data-ttu-id="06d38-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="06d38-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="06d38-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="06d38-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="06d38-106">MacOS Vpp アプリでのアクションの結果を定義します。 actionresult の継承されたプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="06d38-106">Defines results for actions on MacOS Vpp Apps, contains inherited properties for ActionResult.</span></span>

## <a name="properties"></a><span data-ttu-id="06d38-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="06d38-107">Properties</span></span>
|<span data-ttu-id="06d38-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="06d38-108">Property</span></span>|<span data-ttu-id="06d38-109">型</span><span class="sxs-lookup"><span data-stu-id="06d38-109">Type</span></span>|<span data-ttu-id="06d38-110">説明</span><span class="sxs-lookup"><span data-stu-id="06d38-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="06d38-111">userId</span><span class="sxs-lookup"><span data-stu-id="06d38-111">userId</span></span>|<span data-ttu-id="06d38-112">String</span><span class="sxs-lookup"><span data-stu-id="06d38-112">String</span></span>|<span data-ttu-id="06d38-113">アクションに関連付けられている UserId。</span><span class="sxs-lookup"><span data-stu-id="06d38-113">UserId associated with the action.</span></span>|
|<span data-ttu-id="06d38-114">manageddeviceid</span><span class="sxs-lookup"><span data-stu-id="06d38-114">managedDeviceId</span></span>|<span data-ttu-id="06d38-115">String</span><span class="sxs-lookup"><span data-stu-id="06d38-115">String</span></span>|<span data-ttu-id="06d38-116">アクションに関連付けられている DeviceId。</span><span class="sxs-lookup"><span data-stu-id="06d38-116">DeviceId associated with the action.</span></span>|
|<span data-ttu-id="06d38-117">合計の合計数</span><span class="sxs-lookup"><span data-stu-id="06d38-117">totalLicensesCount</span></span>|<span data-ttu-id="06d38-118">Int32</span><span class="sxs-lookup"><span data-stu-id="06d38-118">Int32</span></span>|<span data-ttu-id="06d38-119">取り消しが試行されたライセンスの数。</span><span class="sxs-lookup"><span data-stu-id="06d38-119">A count of the number of licenses for which revoke was attempted.</span></span>|
|<span data-ttu-id="06d38-120">failedLicensesCount</span><span class="sxs-lookup"><span data-stu-id="06d38-120">failedLicensesCount</span></span>|<span data-ttu-id="06d38-121">Int32</span><span class="sxs-lookup"><span data-stu-id="06d38-121">Int32</span></span>|<span data-ttu-id="06d38-122">失効に失敗したライセンスの数。</span><span class="sxs-lookup"><span data-stu-id="06d38-122">A count of the number of licenses for which revoke failed.</span></span>|
|<span data-ttu-id="06d38-123">actionFailureReason</span><span class="sxs-lookup"><span data-stu-id="06d38-123">actionFailureReason</span></span>|[<span data-ttu-id="06d38-124">vppTokenActionFailureReason</span><span class="sxs-lookup"><span data-stu-id="06d38-124">vppTokenActionFailureReason</span></span>](../resources/intune-shared-vpptokenactionfailurereason.md)|<span data-ttu-id="06d38-125">失効ライセンスの処理の失敗の理由。</span><span class="sxs-lookup"><span data-stu-id="06d38-125">The reason for the revoke licenses action failure.</span></span> <span data-ttu-id="06d38-126">可能な値は、`none`、`appleFailure`、`internalError`、`expiredVppToken`、`expiredApplePushNotificationCertificate` です。</span><span class="sxs-lookup"><span data-stu-id="06d38-126">Possible values are: `none`, `appleFailure`, `internalError`, `expiredVppToken`, `expiredApplePushNotificationCertificate`.</span></span>|
|<span data-ttu-id="06d38-127">actionName</span><span class="sxs-lookup"><span data-stu-id="06d38-127">actionName</span></span>|<span data-ttu-id="06d38-128">String</span><span class="sxs-lookup"><span data-stu-id="06d38-128">String</span></span>|<span data-ttu-id="06d38-129">アクション名</span><span class="sxs-lookup"><span data-stu-id="06d38-129">Action name</span></span>|
|<span data-ttu-id="06d38-130">actionState</span><span class="sxs-lookup"><span data-stu-id="06d38-130">actionState</span></span>|[<span data-ttu-id="06d38-131">actionState</span><span class="sxs-lookup"><span data-stu-id="06d38-131">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="06d38-132">アクションの状態。</span><span class="sxs-lookup"><span data-stu-id="06d38-132">State of the action.</span></span> <span data-ttu-id="06d38-133">可能な値は、`none`、`pending`、`canceled`、`active`、`done`、`failed`、`notSupported` です。</span><span class="sxs-lookup"><span data-stu-id="06d38-133">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="06d38-134">startDateTime</span><span class="sxs-lookup"><span data-stu-id="06d38-134">startDateTime</span></span>|<span data-ttu-id="06d38-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="06d38-135">DateTimeOffset</span></span>|<span data-ttu-id="06d38-136">アクションが開始された時刻</span><span class="sxs-lookup"><span data-stu-id="06d38-136">Time the action was initiated</span></span>|
|<span data-ttu-id="06d38-137">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="06d38-137">lastUpdatedDateTime</span></span>|<span data-ttu-id="06d38-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="06d38-138">DateTimeOffset</span></span>|<span data-ttu-id="06d38-139">アクション状態の最終更新時刻</span><span class="sxs-lookup"><span data-stu-id="06d38-139">Time the action state was last updated</span></span>|

## <a name="relationships"></a><span data-ttu-id="06d38-140">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="06d38-140">Relationships</span></span>
<span data-ttu-id="06d38-141">なし</span><span class="sxs-lookup"><span data-stu-id="06d38-141">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="06d38-142">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="06d38-142">JSON Representation</span></span>
<span data-ttu-id="06d38-143">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="06d38-143">Here is a JSON representation of the resource.</span></span>
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




