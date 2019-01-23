---
title: vppTokenRevokeLicensesActionResult リソースの種類
description: 取り消しライセンスのステータスは、Apple ボリューム購入プログラムのトークンで実行されます。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 75c75c6b8bcdc06ede0f71b19956155becc4d478
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29418226"
---
# <a name="vpptokenrevokelicensesactionresult-resource-type"></a><span data-ttu-id="14015-103">vppTokenRevokeLicensesActionResult リソースの種類</span><span class="sxs-lookup"><span data-stu-id="14015-103">vppTokenRevokeLicensesActionResult resource type</span></span>

> <span data-ttu-id="14015-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="14015-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="14015-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="14015-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="14015-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="14015-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="14015-107">取り消しライセンスのステータスは、Apple ボリューム購入プログラムのトークンで実行されます。</span><span class="sxs-lookup"><span data-stu-id="14015-107">The status of the revoke licenses action performed on the Apple Volume Purchase Program token.</span></span>


<span data-ttu-id="14015-108">[VppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="14015-108">Inherits from [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="14015-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="14015-109">Properties</span></span>
|<span data-ttu-id="14015-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="14015-110">Property</span></span>|<span data-ttu-id="14015-111">型</span><span class="sxs-lookup"><span data-stu-id="14015-111">Type</span></span>|<span data-ttu-id="14015-112">説明</span><span class="sxs-lookup"><span data-stu-id="14015-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="14015-113">actionName</span><span class="sxs-lookup"><span data-stu-id="14015-113">actionName</span></span>|<span data-ttu-id="14015-114">String</span><span class="sxs-lookup"><span data-stu-id="14015-114">String</span></span>|<span data-ttu-id="14015-115">[VppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)からアクション名継承</span><span class="sxs-lookup"><span data-stu-id="14015-115">Action name Inherited from [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)</span></span>|
|<span data-ttu-id="14015-116">actionState</span><span class="sxs-lookup"><span data-stu-id="14015-116">actionState</span></span>|[<span data-ttu-id="14015-117">actionState</span><span class="sxs-lookup"><span data-stu-id="14015-117">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="14015-118">[VppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)から継承される、アクションの状態です。</span><span class="sxs-lookup"><span data-stu-id="14015-118">State of the action Inherited from [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md).</span></span> <span data-ttu-id="14015-119">可能な値は、`none`、`pending`、`canceled`、`active`、`done`、`failed`、`notSupported` です。</span><span class="sxs-lookup"><span data-stu-id="14015-119">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="14015-120">startDateTime</span><span class="sxs-lookup"><span data-stu-id="14015-120">startDateTime</span></span>|<span data-ttu-id="14015-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="14015-121">DateTimeOffset</span></span>|<span data-ttu-id="14015-122">アクションが開始された時刻[vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="14015-122">Time the action was initiated Inherited from [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)</span></span>|
|<span data-ttu-id="14015-123">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="14015-123">lastUpdatedDateTime</span></span>|<span data-ttu-id="14015-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="14015-124">DateTimeOffset</span></span>|<span data-ttu-id="14015-125">動作状態が最後に[vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)からの継承の更新</span><span class="sxs-lookup"><span data-stu-id="14015-125">Time the action state was last updated Inherited from [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)</span></span>|
|<span data-ttu-id="14015-126">totalLicensesCount</span><span class="sxs-lookup"><span data-stu-id="14015-126">totalLicensesCount</span></span>|<span data-ttu-id="14015-127">Int32</span><span class="sxs-lookup"><span data-stu-id="14015-127">Int32</span></span>|<span data-ttu-id="14015-128">無効にしようとしていたライセンスの数のカウントです。</span><span class="sxs-lookup"><span data-stu-id="14015-128">A count of the number of licenses that were attempted to revoke.</span></span>|
|<span data-ttu-id="14015-129">failedLicensesCount</span><span class="sxs-lookup"><span data-stu-id="14015-129">failedLicensesCount</span></span>|<span data-ttu-id="14015-130">Int32</span><span class="sxs-lookup"><span data-stu-id="14015-130">Int32</span></span>|<span data-ttu-id="14015-131">取り消しに失敗したライセンスの数のカウントです。</span><span class="sxs-lookup"><span data-stu-id="14015-131">A count of the number of licenses that failed to revoke.</span></span>|
|<span data-ttu-id="14015-132">actionFailureReason</span><span class="sxs-lookup"><span data-stu-id="14015-132">actionFailureReason</span></span>|[<span data-ttu-id="14015-133">vppTokenActionFailureReason</span><span class="sxs-lookup"><span data-stu-id="14015-133">vppTokenActionFailureReason</span></span>](../resources/intune-shared-vpptokenactionfailurereason.md)|<span data-ttu-id="14015-134">取り消しライセンス操作が失敗した理由です。</span><span class="sxs-lookup"><span data-stu-id="14015-134">The reason for the revoke licenses action failure.</span></span> <span data-ttu-id="14015-135">可能な値は、`none`、`appleFailure`、`internalError`、`expiredVppToken`、`expiredApplePushNotificationCertificate` です。</span><span class="sxs-lookup"><span data-stu-id="14015-135">Possible values are: `none`, `appleFailure`, `internalError`, `expiredVppToken`, `expiredApplePushNotificationCertificate`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="14015-136">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="14015-136">Relationships</span></span>
<span data-ttu-id="14015-137">なし</span><span class="sxs-lookup"><span data-stu-id="14015-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="14015-138">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="14015-138">JSON Representation</span></span>
<span data-ttu-id="14015-139">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="14015-139">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.vppTokenRevokeLicensesActionResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.vppTokenRevokeLicensesActionResult",
  "actionName": "String",
  "actionState": "String",
  "startDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)",
  "totalLicensesCount": 1024,
  "failedLicensesCount": 1024,
  "actionFailureReason": "String"
}
```




