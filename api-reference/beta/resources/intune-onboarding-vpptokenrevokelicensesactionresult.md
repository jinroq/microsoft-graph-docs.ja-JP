---
title: vppTokenRevokeLicensesActionResult リソースの種類
description: 取り消しライセンスのステータスは、Apple ボリューム購入プログラムのトークンで実行されます。
author: tfitzmac
ms.openlocfilehash: a4188a269f9273b955fd29b32348dec82023b181
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27351458"
---
# <a name="vpptokenrevokelicensesactionresult-resource-type"></a><span data-ttu-id="e28b6-103">vppTokenRevokeLicensesActionResult リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e28b6-103">vppTokenRevokeLicensesActionResult resource type</span></span>

> <span data-ttu-id="e28b6-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="e28b6-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e28b6-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e28b6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e28b6-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="e28b6-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e28b6-107">取り消しライセンスのステータスは、Apple ボリューム購入プログラムのトークンで実行されます。</span><span class="sxs-lookup"><span data-stu-id="e28b6-107">The status of the revoke licenses action performed on the Apple Volume Purchase Program token.</span></span>

<span data-ttu-id="e28b6-108">[VppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="e28b6-108">Inherits from [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="e28b6-109">Properties</span><span class="sxs-lookup"><span data-stu-id="e28b6-109">Properties</span></span>
|<span data-ttu-id="e28b6-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e28b6-110">Property</span></span>|<span data-ttu-id="e28b6-111">種類</span><span class="sxs-lookup"><span data-stu-id="e28b6-111">Type</span></span>|<span data-ttu-id="e28b6-112">説明</span><span class="sxs-lookup"><span data-stu-id="e28b6-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e28b6-113">actionName</span><span class="sxs-lookup"><span data-stu-id="e28b6-113">actionName</span></span>|<span data-ttu-id="e28b6-114">String</span><span class="sxs-lookup"><span data-stu-id="e28b6-114">String</span></span>|<span data-ttu-id="e28b6-115">[VppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)からアクション名継承</span><span class="sxs-lookup"><span data-stu-id="e28b6-115">Action name Inherited from [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)</span></span>|
|<span data-ttu-id="e28b6-116">actionState</span><span class="sxs-lookup"><span data-stu-id="e28b6-116">actionState</span></span>|[<span data-ttu-id="e28b6-117">actionState</span><span class="sxs-lookup"><span data-stu-id="e28b6-117">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="e28b6-118">[VppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)から継承される、アクションの状態です。</span><span class="sxs-lookup"><span data-stu-id="e28b6-118">State of the action Inherited from [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md).</span></span> <span data-ttu-id="e28b6-119">可能な値は、`none`、`pending`、`canceled`、`active`、`done`、`failed`、`notSupported` です。</span><span class="sxs-lookup"><span data-stu-id="e28b6-119">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="e28b6-120">startDateTime</span><span class="sxs-lookup"><span data-stu-id="e28b6-120">startDateTime</span></span>|<span data-ttu-id="e28b6-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e28b6-121">DateTimeOffset</span></span>|<span data-ttu-id="e28b6-122">アクションが開始された時刻[vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="e28b6-122">Time the action was initiated Inherited from [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)</span></span>|
|<span data-ttu-id="e28b6-123">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="e28b6-123">lastUpdatedDateTime</span></span>|<span data-ttu-id="e28b6-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e28b6-124">DateTimeOffset</span></span>|<span data-ttu-id="e28b6-125">動作状態が最後に[vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)からの継承の更新</span><span class="sxs-lookup"><span data-stu-id="e28b6-125">Time the action state was last updated Inherited from [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)</span></span>|
|<span data-ttu-id="e28b6-126">totalLicensesCount</span><span class="sxs-lookup"><span data-stu-id="e28b6-126">totalLicensesCount</span></span>|<span data-ttu-id="e28b6-127">Int32</span><span class="sxs-lookup"><span data-stu-id="e28b6-127">Int32</span></span>|<span data-ttu-id="e28b6-128">無効にしようとしていたライセンスの数のカウントです。</span><span class="sxs-lookup"><span data-stu-id="e28b6-128">A count of the number of licenses that were attempted to revoke.</span></span>|
|<span data-ttu-id="e28b6-129">failedLicensesCount</span><span class="sxs-lookup"><span data-stu-id="e28b6-129">failedLicensesCount</span></span>|<span data-ttu-id="e28b6-130">Int32</span><span class="sxs-lookup"><span data-stu-id="e28b6-130">Int32</span></span>|<span data-ttu-id="e28b6-131">取り消しに失敗したライセンスの数のカウントです。</span><span class="sxs-lookup"><span data-stu-id="e28b6-131">A count of the number of licenses that failed to revoke.</span></span>|
|<span data-ttu-id="e28b6-132">actionFailureReason</span><span class="sxs-lookup"><span data-stu-id="e28b6-132">actionFailureReason</span></span>|[<span data-ttu-id="e28b6-133">vppTokenActionFailureReason</span><span class="sxs-lookup"><span data-stu-id="e28b6-133">vppTokenActionFailureReason</span></span>](../resources/intune-shared-vpptokenactionfailurereason.md)|<span data-ttu-id="e28b6-134">取り消しライセンス操作が失敗した理由です。</span><span class="sxs-lookup"><span data-stu-id="e28b6-134">The reason for the revoke licenses action failure.</span></span> <span data-ttu-id="e28b6-135">可能な値は、`none`、`appleFailure`、`internalError`、`expiredVppToken`、`expiredApplePushNotificationCertificate` です。</span><span class="sxs-lookup"><span data-stu-id="e28b6-135">Possible values are: `none`, `appleFailure`, `internalError`, `expiredVppToken`, `expiredApplePushNotificationCertificate`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e28b6-136">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="e28b6-136">Relationships</span></span>
<span data-ttu-id="e28b6-137">なし</span><span class="sxs-lookup"><span data-stu-id="e28b6-137">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="e28b6-138">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e28b6-138">JSON Representation</span></span>
<span data-ttu-id="e28b6-139">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="e28b6-139">Here is a JSON representation of the resource.</span></span>
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





