---
title: vppTokenRevokeLicensesActionResult リソースの種類
description: Apple ボリューム購入プログラムのトークンに対して実行された取り消しライセンス操作の状態。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 432419f337750362256140b8d13a1841b49907d4
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32566466"
---
# <a name="vpptokenrevokelicensesactionresult-resource-type"></a><span data-ttu-id="e9827-103">vppTokenRevokeLicensesActionResult リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e9827-103">vppTokenRevokeLicensesActionResult resource type</span></span>

> <span data-ttu-id="e9827-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e9827-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e9827-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="e9827-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e9827-106">Apple ボリューム購入プログラムのトークンに対して実行された取り消しライセンス操作の状態。</span><span class="sxs-lookup"><span data-stu-id="e9827-106">The status of the revoke licenses action performed on the Apple Volume Purchase Program token.</span></span>


<span data-ttu-id="e9827-107">[vpptokenactionresult](../resources/intune-onboarding-vpptokenactionresult.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="e9827-107">Inherits from [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="e9827-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e9827-108">Properties</span></span>
|<span data-ttu-id="e9827-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e9827-109">Property</span></span>|<span data-ttu-id="e9827-110">型</span><span class="sxs-lookup"><span data-stu-id="e9827-110">Type</span></span>|<span data-ttu-id="e9827-111">説明</span><span class="sxs-lookup"><span data-stu-id="e9827-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e9827-112">actionName</span><span class="sxs-lookup"><span data-stu-id="e9827-112">actionName</span></span>|<span data-ttu-id="e9827-113">String</span><span class="sxs-lookup"><span data-stu-id="e9827-113">String</span></span>|<span data-ttu-id="e9827-114">[vpptokenactionresult](../resources/intune-onboarding-vpptokenactionresult.md)から継承されるアクション名</span><span class="sxs-lookup"><span data-stu-id="e9827-114">Action name Inherited from [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)</span></span>|
|<span data-ttu-id="e9827-115">actionState</span><span class="sxs-lookup"><span data-stu-id="e9827-115">actionState</span></span>|[<span data-ttu-id="e9827-116">actionState</span><span class="sxs-lookup"><span data-stu-id="e9827-116">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="e9827-117">[vpptokenactionresult](../resources/intune-onboarding-vpptokenactionresult.md)から継承されたアクションの状態。</span><span class="sxs-lookup"><span data-stu-id="e9827-117">State of the action Inherited from [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md).</span></span> <span data-ttu-id="e9827-118">可能な値は、`none`、`pending`、`canceled`、`active`、`done`、`failed`、`notSupported` です。</span><span class="sxs-lookup"><span data-stu-id="e9827-118">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="e9827-119">startDateTime</span><span class="sxs-lookup"><span data-stu-id="e9827-119">startDateTime</span></span>|<span data-ttu-id="e9827-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e9827-120">DateTimeOffset</span></span>|<span data-ttu-id="e9827-121">アクションが[vpptokenactionresult](../resources/intune-onboarding-vpptokenactionresult.md)から継承された時刻</span><span class="sxs-lookup"><span data-stu-id="e9827-121">Time the action was initiated Inherited from [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)</span></span>|
|<span data-ttu-id="e9827-122">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="e9827-122">lastUpdatedDateTime</span></span>|<span data-ttu-id="e9827-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e9827-123">DateTimeOffset</span></span>|<span data-ttu-id="e9827-124">アクション状態が最後に更新された時刻。 [vpptokenactionresult](../resources/intune-onboarding-vpptokenactionresult.md)から継承</span><span class="sxs-lookup"><span data-stu-id="e9827-124">Time the action state was last updated Inherited from [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)</span></span>|
|<span data-ttu-id="e9827-125">合計の合計数</span><span class="sxs-lookup"><span data-stu-id="e9827-125">totalLicensesCount</span></span>|<span data-ttu-id="e9827-126">Int32</span><span class="sxs-lookup"><span data-stu-id="e9827-126">Int32</span></span>|<span data-ttu-id="e9827-127">失効しようとしたライセンスの数。</span><span class="sxs-lookup"><span data-stu-id="e9827-127">A count of the number of licenses that were attempted to revoke.</span></span>|
|<span data-ttu-id="e9827-128">failedLicensesCount</span><span class="sxs-lookup"><span data-stu-id="e9827-128">failedLicensesCount</span></span>|<span data-ttu-id="e9827-129">Int32</span><span class="sxs-lookup"><span data-stu-id="e9827-129">Int32</span></span>|<span data-ttu-id="e9827-130">失効に失敗したライセンスの数。</span><span class="sxs-lookup"><span data-stu-id="e9827-130">A count of the number of licenses that failed to revoke.</span></span>|
|<span data-ttu-id="e9827-131">actionFailureReason</span><span class="sxs-lookup"><span data-stu-id="e9827-131">actionFailureReason</span></span>|[<span data-ttu-id="e9827-132">vppTokenActionFailureReason</span><span class="sxs-lookup"><span data-stu-id="e9827-132">vppTokenActionFailureReason</span></span>](../resources/intune-shared-vpptokenactionfailurereason.md)|<span data-ttu-id="e9827-133">失効ライセンスの処理の失敗の理由。</span><span class="sxs-lookup"><span data-stu-id="e9827-133">The reason for the revoke licenses action failure.</span></span> <span data-ttu-id="e9827-134">可能な値は、`none`、`appleFailure`、`internalError`、`expiredVppToken`、`expiredApplePushNotificationCertificate` です。</span><span class="sxs-lookup"><span data-stu-id="e9827-134">Possible values are: `none`, `appleFailure`, `internalError`, `expiredVppToken`, `expiredApplePushNotificationCertificate`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e9827-135">関係</span><span class="sxs-lookup"><span data-stu-id="e9827-135">Relationships</span></span>
<span data-ttu-id="e9827-136">なし</span><span class="sxs-lookup"><span data-stu-id="e9827-136">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e9827-137">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e9827-137">JSON Representation</span></span>
<span data-ttu-id="e9827-138">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="e9827-138">Here is a JSON representation of the resource.</span></span>
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





