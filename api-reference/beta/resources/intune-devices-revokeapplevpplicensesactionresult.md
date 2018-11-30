---
title: revokeAppleVppLicensesActionResult リソースの種類
description: アップル Vpp ライセンスのアクションの結果を取り消す
ms.openlocfilehash: f751f90b90bbf282fa05a59a4a1c59d04ccfbb99
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27069754"
---
# <a name="revokeapplevpplicensesactionresult-resource-type"></a><span data-ttu-id="02039-103">revokeAppleVppLicensesActionResult リソースの種類</span><span class="sxs-lookup"><span data-stu-id="02039-103">revokeAppleVppLicensesActionResult resource type</span></span>

> <span data-ttu-id="02039-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="02039-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="02039-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="02039-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="02039-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="02039-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="02039-107">アップル Vpp ライセンスのアクションの結果を取り消す</span><span class="sxs-lookup"><span data-stu-id="02039-107">Revoke Apple Vpp licenses action result</span></span>

<span data-ttu-id="02039-108">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="02039-108">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="02039-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="02039-109">Properties</span></span>
|<span data-ttu-id="02039-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="02039-110">Property</span></span>|<span data-ttu-id="02039-111">型</span><span class="sxs-lookup"><span data-stu-id="02039-111">Type</span></span>|<span data-ttu-id="02039-112">説明</span><span class="sxs-lookup"><span data-stu-id="02039-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="02039-113">actionName</span><span class="sxs-lookup"><span data-stu-id="02039-113">actionName</span></span>|<span data-ttu-id="02039-114">String</span><span class="sxs-lookup"><span data-stu-id="02039-114">String</span></span>|<span data-ttu-id="02039-115">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) から継承されるアクション名</span><span class="sxs-lookup"><span data-stu-id="02039-115">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="02039-116">actionState</span><span class="sxs-lookup"><span data-stu-id="02039-116">actionState</span></span>|[<span data-ttu-id="02039-117">actionState</span><span class="sxs-lookup"><span data-stu-id="02039-117">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="02039-118">[DeviceActionResult](../resources/intune-devices-deviceactionresult.md)から継承される、アクションの状態です。</span><span class="sxs-lookup"><span data-stu-id="02039-118">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="02039-119">可能な値は、`none`、`pending`、`canceled`、`active`、`done`、`failed`、`notSupported` です。</span><span class="sxs-lookup"><span data-stu-id="02039-119">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="02039-120">startDateTime</span><span class="sxs-lookup"><span data-stu-id="02039-120">startDateTime</span></span>|<span data-ttu-id="02039-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="02039-121">DateTimeOffset</span></span>|<span data-ttu-id="02039-122">アクションが開始された時刻 ([deviceActionResult](../resources/intune-devices-deviceactionresult.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="02039-122">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="02039-123">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="02039-123">lastUpdatedDateTime</span></span>|<span data-ttu-id="02039-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="02039-124">DateTimeOffset</span></span>|<span data-ttu-id="02039-125">アクション状態の最終更新時刻 ([deviceActionResult](../resources/intune-devices-deviceactionresult.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="02039-125">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="02039-126">totalLicensesCount</span><span class="sxs-lookup"><span data-stu-id="02039-126">totalLicensesCount</span></span>|<span data-ttu-id="02039-127">Int32</span><span class="sxs-lookup"><span data-stu-id="02039-127">Int32</span></span>|<span data-ttu-id="02039-128">関連付けられている Apple Vpp ライセンスの合計数</span><span class="sxs-lookup"><span data-stu-id="02039-128">Total number of Apple Vpp licenses associated</span></span>|
|<span data-ttu-id="02039-129">failedLicensesCount</span><span class="sxs-lookup"><span data-stu-id="02039-129">failedLicensesCount</span></span>|<span data-ttu-id="02039-130">Int32</span><span class="sxs-lookup"><span data-stu-id="02039-130">Int32</span></span>|<span data-ttu-id="02039-131">アップル Vpp ライセンスを失効に失敗した数の合計</span><span class="sxs-lookup"><span data-stu-id="02039-131">Total number of Apple Vpp licenses that failed to revoke</span></span>|

## <a name="relationships"></a><span data-ttu-id="02039-132">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="02039-132">Relationships</span></span>
<span data-ttu-id="02039-133">なし</span><span class="sxs-lookup"><span data-stu-id="02039-133">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="02039-134">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="02039-134">JSON Representation</span></span>
<span data-ttu-id="02039-135">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="02039-135">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.revokeAppleVppLicensesActionResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.revokeAppleVppLicensesActionResult",
  "actionName": "String",
  "actionState": "String",
  "startDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)",
  "totalLicensesCount": 1024,
  "failedLicensesCount": 1024
}
```





