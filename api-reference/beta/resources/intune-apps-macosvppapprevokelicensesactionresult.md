---
title: macOsVppAppRevokeLicensesActionResult リソースの種類
description: MacOS Vpp アプリでのアクションの結果を定義します。 ActionResult の継承されたプロパティが含まれています。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: bb8a69ab5852aa3fee9ab8ffab757a87ef0235ba
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36365896"
---
# <a name="macosvppapprevokelicensesactionresult-resource-type"></a><span data-ttu-id="4ceef-103">macOsVppAppRevokeLicensesActionResult リソースの種類</span><span class="sxs-lookup"><span data-stu-id="4ceef-103">macOsVppAppRevokeLicensesActionResult resource type</span></span>

> <span data-ttu-id="4ceef-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4ceef-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4ceef-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="4ceef-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4ceef-106">MacOS Vpp アプリでのアクションの結果を定義します。 ActionResult の継承されたプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="4ceef-106">Defines results for actions on MacOS Vpp Apps, contains inherited properties for ActionResult.</span></span>

## <a name="properties"></a><span data-ttu-id="4ceef-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4ceef-107">Properties</span></span>
|<span data-ttu-id="4ceef-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4ceef-108">Property</span></span>|<span data-ttu-id="4ceef-109">型</span><span class="sxs-lookup"><span data-stu-id="4ceef-109">Type</span></span>|<span data-ttu-id="4ceef-110">説明</span><span class="sxs-lookup"><span data-stu-id="4ceef-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4ceef-111">userId</span><span class="sxs-lookup"><span data-stu-id="4ceef-111">userId</span></span>|<span data-ttu-id="4ceef-112">String</span><span class="sxs-lookup"><span data-stu-id="4ceef-112">String</span></span>|<span data-ttu-id="4ceef-113">アクションに関連付けられている UserId。</span><span class="sxs-lookup"><span data-stu-id="4ceef-113">UserId associated with the action.</span></span>|
|<span data-ttu-id="4ceef-114">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="4ceef-114">managedDeviceId</span></span>|<span data-ttu-id="4ceef-115">String</span><span class="sxs-lookup"><span data-stu-id="4ceef-115">String</span></span>|<span data-ttu-id="4ceef-116">アクションに関連付けられている DeviceId。</span><span class="sxs-lookup"><span data-stu-id="4ceef-116">DeviceId associated with the action.</span></span>|
|<span data-ttu-id="4ceef-117">合計の合計数</span><span class="sxs-lookup"><span data-stu-id="4ceef-117">totalLicensesCount</span></span>|<span data-ttu-id="4ceef-118">Int32</span><span class="sxs-lookup"><span data-stu-id="4ceef-118">Int32</span></span>|<span data-ttu-id="4ceef-119">取り消しが試行されたライセンスの数。</span><span class="sxs-lookup"><span data-stu-id="4ceef-119">A count of the number of licenses for which revoke was attempted.</span></span>|
|<span data-ttu-id="4ceef-120">failedLicensesCount</span><span class="sxs-lookup"><span data-stu-id="4ceef-120">failedLicensesCount</span></span>|<span data-ttu-id="4ceef-121">Int32</span><span class="sxs-lookup"><span data-stu-id="4ceef-121">Int32</span></span>|<span data-ttu-id="4ceef-122">失効に失敗したライセンスの数。</span><span class="sxs-lookup"><span data-stu-id="4ceef-122">A count of the number of licenses for which revoke failed.</span></span>|
|<span data-ttu-id="4ceef-123">actionFailureReason</span><span class="sxs-lookup"><span data-stu-id="4ceef-123">actionFailureReason</span></span>|[<span data-ttu-id="4ceef-124">vppTokenActionFailureReason</span><span class="sxs-lookup"><span data-stu-id="4ceef-124">vppTokenActionFailureReason</span></span>](../resources/intune-shared-vpptokenactionfailurereason.md)|<span data-ttu-id="4ceef-125">失効ライセンスの処理の失敗の理由。</span><span class="sxs-lookup"><span data-stu-id="4ceef-125">The reason for the revoke licenses action failure.</span></span> <span data-ttu-id="4ceef-126">可能な値は、`none`、`appleFailure`、`internalError`、`expiredVppToken`、`expiredApplePushNotificationCertificate` です。</span><span class="sxs-lookup"><span data-stu-id="4ceef-126">Possible values are: `none`, `appleFailure`, `internalError`, `expiredVppToken`, `expiredApplePushNotificationCertificate`.</span></span>|
|<span data-ttu-id="4ceef-127">actionName</span><span class="sxs-lookup"><span data-stu-id="4ceef-127">actionName</span></span>|<span data-ttu-id="4ceef-128">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="4ceef-128">String</span></span>|<span data-ttu-id="4ceef-129">アクション名</span><span class="sxs-lookup"><span data-stu-id="4ceef-129">Action name</span></span>|
|<span data-ttu-id="4ceef-130">actionState</span><span class="sxs-lookup"><span data-stu-id="4ceef-130">actionState</span></span>|[<span data-ttu-id="4ceef-131">actionState</span><span class="sxs-lookup"><span data-stu-id="4ceef-131">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="4ceef-132">アクションの状態。</span><span class="sxs-lookup"><span data-stu-id="4ceef-132">State of the action.</span></span> <span data-ttu-id="4ceef-133">可能な値は、`none`、`pending`、`canceled`、`active`、`done`、`failed`、`notSupported` です。</span><span class="sxs-lookup"><span data-stu-id="4ceef-133">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="4ceef-134">startDateTime</span><span class="sxs-lookup"><span data-stu-id="4ceef-134">startDateTime</span></span>|<span data-ttu-id="4ceef-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4ceef-135">DateTimeOffset</span></span>|<span data-ttu-id="4ceef-136">アクションが開始された時刻</span><span class="sxs-lookup"><span data-stu-id="4ceef-136">Time the action was initiated</span></span>|
|<span data-ttu-id="4ceef-137">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="4ceef-137">lastUpdatedDateTime</span></span>|<span data-ttu-id="4ceef-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4ceef-138">DateTimeOffset</span></span>|<span data-ttu-id="4ceef-139">アクション状態の最終更新時刻</span><span class="sxs-lookup"><span data-stu-id="4ceef-139">Time the action state was last updated</span></span>|

## <a name="relationships"></a><span data-ttu-id="4ceef-140">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="4ceef-140">Relationships</span></span>
<span data-ttu-id="4ceef-141">なし</span><span class="sxs-lookup"><span data-stu-id="4ceef-141">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4ceef-142">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="4ceef-142">JSON Representation</span></span>
<span data-ttu-id="4ceef-143">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="4ceef-143">Here is a JSON representation of the resource.</span></span>
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



