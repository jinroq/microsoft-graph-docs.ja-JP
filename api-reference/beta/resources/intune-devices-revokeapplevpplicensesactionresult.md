---
title: revokeAppleVppLicensesActionResult リソースの種類
description: アップル Vpp ライセンスのアクションの結果を取り消す
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: b7e578ee695e171a1a91167b61e47af717dd82c0
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27879101"
---
# <a name="revokeapplevpplicensesactionresult-resource-type"></a><span data-ttu-id="1285a-103">revokeAppleVppLicensesActionResult リソースの種類</span><span class="sxs-lookup"><span data-stu-id="1285a-103">revokeAppleVppLicensesActionResult resource type</span></span>

> <span data-ttu-id="1285a-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="1285a-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1285a-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1285a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1285a-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="1285a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1285a-107">アップル Vpp ライセンスのアクションの結果を取り消す</span><span class="sxs-lookup"><span data-stu-id="1285a-107">Revoke Apple Vpp licenses action result</span></span>

<span data-ttu-id="1285a-108">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1285a-108">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="1285a-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1285a-109">Properties</span></span>
|<span data-ttu-id="1285a-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1285a-110">Property</span></span>|<span data-ttu-id="1285a-111">種類</span><span class="sxs-lookup"><span data-stu-id="1285a-111">Type</span></span>|<span data-ttu-id="1285a-112">説明</span><span class="sxs-lookup"><span data-stu-id="1285a-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1285a-113">actionName</span><span class="sxs-lookup"><span data-stu-id="1285a-113">actionName</span></span>|<span data-ttu-id="1285a-114">String</span><span class="sxs-lookup"><span data-stu-id="1285a-114">String</span></span>|<span data-ttu-id="1285a-115">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) から継承されるアクション名</span><span class="sxs-lookup"><span data-stu-id="1285a-115">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="1285a-116">actionState</span><span class="sxs-lookup"><span data-stu-id="1285a-116">actionState</span></span>|[<span data-ttu-id="1285a-117">actionState</span><span class="sxs-lookup"><span data-stu-id="1285a-117">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="1285a-118">[DeviceActionResult](../resources/intune-devices-deviceactionresult.md)から継承される、アクションの状態です。</span><span class="sxs-lookup"><span data-stu-id="1285a-118">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="1285a-119">可能な値は、`none`、`pending`、`canceled`、`active`、`done`、`failed`、`notSupported` です。</span><span class="sxs-lookup"><span data-stu-id="1285a-119">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="1285a-120">startDateTime</span><span class="sxs-lookup"><span data-stu-id="1285a-120">startDateTime</span></span>|<span data-ttu-id="1285a-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1285a-121">DateTimeOffset</span></span>|<span data-ttu-id="1285a-122">アクションが開始された時刻 ([deviceActionResult](../resources/intune-devices-deviceactionresult.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="1285a-122">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="1285a-123">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="1285a-123">lastUpdatedDateTime</span></span>|<span data-ttu-id="1285a-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1285a-124">DateTimeOffset</span></span>|<span data-ttu-id="1285a-125">アクション状態の最終更新時刻 ([deviceActionResult](../resources/intune-devices-deviceactionresult.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="1285a-125">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="1285a-126">totalLicensesCount</span><span class="sxs-lookup"><span data-stu-id="1285a-126">totalLicensesCount</span></span>|<span data-ttu-id="1285a-127">Int32</span><span class="sxs-lookup"><span data-stu-id="1285a-127">Int32</span></span>|<span data-ttu-id="1285a-128">関連付けられている Apple Vpp ライセンスの合計数</span><span class="sxs-lookup"><span data-stu-id="1285a-128">Total number of Apple Vpp licenses associated</span></span>|
|<span data-ttu-id="1285a-129">failedLicensesCount</span><span class="sxs-lookup"><span data-stu-id="1285a-129">failedLicensesCount</span></span>|<span data-ttu-id="1285a-130">Int32</span><span class="sxs-lookup"><span data-stu-id="1285a-130">Int32</span></span>|<span data-ttu-id="1285a-131">アップル Vpp ライセンスを失効に失敗した数の合計</span><span class="sxs-lookup"><span data-stu-id="1285a-131">Total number of Apple Vpp licenses that failed to revoke</span></span>|

## <a name="relationships"></a><span data-ttu-id="1285a-132">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="1285a-132">Relationships</span></span>
<span data-ttu-id="1285a-133">なし</span><span class="sxs-lookup"><span data-stu-id="1285a-133">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="1285a-134">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="1285a-134">JSON Representation</span></span>
<span data-ttu-id="1285a-135">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="1285a-135">Here is a JSON representation of the resource.</span></span>
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





