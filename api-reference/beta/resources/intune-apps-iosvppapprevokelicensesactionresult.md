---
title: iosVppAppRevokeLicensesActionResult リソースの種類
description: ActionResult の継承されたプロパティが含まれています、iOS Vpp のアプリケーションでの操作の結果を定義します。
ms.openlocfilehash: 1c6c1486d63ba5ce7c866dc2697d1a3eb2ee8e38
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27073227"
---
# <a name="iosvppapprevokelicensesactionresult-resource-type"></a><span data-ttu-id="ac6d7-103">iosVppAppRevokeLicensesActionResult リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ac6d7-103">iosVppAppRevokeLicensesActionResult resource type</span></span>

> <span data-ttu-id="ac6d7-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="ac6d7-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ac6d7-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ac6d7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ac6d7-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="ac6d7-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ac6d7-107">ActionResult の継承されたプロパティが含まれています、iOS Vpp のアプリケーションでの操作の結果を定義します。</span><span class="sxs-lookup"><span data-stu-id="ac6d7-107">Defines results for actions on iOS Vpp Apps, contains inherited properties for ActionResult.</span></span>
## <a name="properties"></a><span data-ttu-id="ac6d7-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ac6d7-108">Properties</span></span>
|<span data-ttu-id="ac6d7-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ac6d7-109">Property</span></span>|<span data-ttu-id="ac6d7-110">型</span><span class="sxs-lookup"><span data-stu-id="ac6d7-110">Type</span></span>|<span data-ttu-id="ac6d7-111">説明</span><span class="sxs-lookup"><span data-stu-id="ac6d7-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ac6d7-112">userId</span><span class="sxs-lookup"><span data-stu-id="ac6d7-112">userId</span></span>|<span data-ttu-id="ac6d7-113">String</span><span class="sxs-lookup"><span data-stu-id="ac6d7-113">String</span></span>|<span data-ttu-id="ac6d7-114">アクションに関連付けられているユーザーの Id。</span><span class="sxs-lookup"><span data-stu-id="ac6d7-114">UserId associated with the action.</span></span>|
|<span data-ttu-id="ac6d7-115">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="ac6d7-115">managedDeviceId</span></span>|<span data-ttu-id="ac6d7-116">String</span><span class="sxs-lookup"><span data-stu-id="ac6d7-116">String</span></span>|<span data-ttu-id="ac6d7-117">DeviceId はアクションに関連付けられています。</span><span class="sxs-lookup"><span data-stu-id="ac6d7-117">DeviceId associated with the action.</span></span>|
|<span data-ttu-id="ac6d7-118">totalLicensesCount</span><span class="sxs-lookup"><span data-stu-id="ac6d7-118">totalLicensesCount</span></span>|<span data-ttu-id="ac6d7-119">Int32</span><span class="sxs-lookup"><span data-stu-id="ac6d7-119">Int32</span></span>|<span data-ttu-id="ac6d7-120">取り消しが実行しようとするライセンス数のカウントです。</span><span class="sxs-lookup"><span data-stu-id="ac6d7-120">A count of the number of licenses for which revoke was attempted.</span></span>|
|<span data-ttu-id="ac6d7-121">failedLicensesCount</span><span class="sxs-lookup"><span data-stu-id="ac6d7-121">failedLicensesCount</span></span>|<span data-ttu-id="ac6d7-122">Int32</span><span class="sxs-lookup"><span data-stu-id="ac6d7-122">Int32</span></span>|<span data-ttu-id="ac6d7-123">失敗する revoke のライセンス数のカウントです。</span><span class="sxs-lookup"><span data-stu-id="ac6d7-123">A count of the number of licenses for which revoke failed.</span></span>|
|<span data-ttu-id="ac6d7-124">actionFailureReason</span><span class="sxs-lookup"><span data-stu-id="ac6d7-124">actionFailureReason</span></span>|[<span data-ttu-id="ac6d7-125">vppTokenActionFailureReason</span><span class="sxs-lookup"><span data-stu-id="ac6d7-125">vppTokenActionFailureReason</span></span>](../resources/intune-shared-vpptokenactionfailurereason.md)|<span data-ttu-id="ac6d7-126">取り消しライセンス操作が失敗した理由です。</span><span class="sxs-lookup"><span data-stu-id="ac6d7-126">The reason for the revoke licenses action failure.</span></span> <span data-ttu-id="ac6d7-127">可能な値は、`none`、`appleFailure`、`internalError`、`expiredVppToken`、`expiredApplePushNotificationCertificate` です。</span><span class="sxs-lookup"><span data-stu-id="ac6d7-127">Possible values are: `none`, `appleFailure`, `internalError`, `expiredVppToken`, `expiredApplePushNotificationCertificate`.</span></span>|
|<span data-ttu-id="ac6d7-128">actionName</span><span class="sxs-lookup"><span data-stu-id="ac6d7-128">actionName</span></span>|<span data-ttu-id="ac6d7-129">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="ac6d7-129">String</span></span>|<span data-ttu-id="ac6d7-130">アクション名</span><span class="sxs-lookup"><span data-stu-id="ac6d7-130">Action name</span></span>|
|<span data-ttu-id="ac6d7-131">actionState</span><span class="sxs-lookup"><span data-stu-id="ac6d7-131">actionState</span></span>|[<span data-ttu-id="ac6d7-132">actionState</span><span class="sxs-lookup"><span data-stu-id="ac6d7-132">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="ac6d7-133">アクションの状態です。</span><span class="sxs-lookup"><span data-stu-id="ac6d7-133">State of the action.</span></span> <span data-ttu-id="ac6d7-134">可能な値は、`none`、`pending`、`canceled`、`active`、`done`、`failed`、`notSupported` です。</span><span class="sxs-lookup"><span data-stu-id="ac6d7-134">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="ac6d7-135">startDateTime</span><span class="sxs-lookup"><span data-stu-id="ac6d7-135">startDateTime</span></span>|<span data-ttu-id="ac6d7-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ac6d7-136">DateTimeOffset</span></span>|<span data-ttu-id="ac6d7-137">アクションが開始された時刻</span><span class="sxs-lookup"><span data-stu-id="ac6d7-137">Time the action was initiated</span></span>|
|<span data-ttu-id="ac6d7-138">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="ac6d7-138">lastUpdatedDateTime</span></span>|<span data-ttu-id="ac6d7-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ac6d7-139">DateTimeOffset</span></span>|<span data-ttu-id="ac6d7-140">アクション状態の最終更新時刻</span><span class="sxs-lookup"><span data-stu-id="ac6d7-140">Time the action state was last updated</span></span>|

## <a name="relationships"></a><span data-ttu-id="ac6d7-141">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="ac6d7-141">Relationships</span></span>
<span data-ttu-id="ac6d7-142">なし</span><span class="sxs-lookup"><span data-stu-id="ac6d7-142">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="ac6d7-143">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ac6d7-143">JSON Representation</span></span>
<span data-ttu-id="ac6d7-144">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="ac6d7-144">Here is a JSON representation of the resource.</span></span>
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





