---
title: windowsDefenderScanActionResult リソースの種類
description: Windows Defender の最後のスキャン結果
ms.openlocfilehash: 9adfa41f21bb23f5073f0d62c1c49bc1cfea3912
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27072686"
---
# <a name="windowsdefenderscanactionresult-resource-type"></a><span data-ttu-id="754f2-103">windowsDefenderScanActionResult リソースの種類</span><span class="sxs-lookup"><span data-stu-id="754f2-103">windowsDefenderScanActionResult resource type</span></span>

> <span data-ttu-id="754f2-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="754f2-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="754f2-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="754f2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="754f2-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="754f2-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="754f2-107">Windows Defender の最後のスキャン結果</span><span class="sxs-lookup"><span data-stu-id="754f2-107">Windows Defender last scan result</span></span>

<span data-ttu-id="754f2-108">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="754f2-108">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="754f2-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="754f2-109">Properties</span></span>
|<span data-ttu-id="754f2-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="754f2-110">Property</span></span>|<span data-ttu-id="754f2-111">型</span><span class="sxs-lookup"><span data-stu-id="754f2-111">Type</span></span>|<span data-ttu-id="754f2-112">説明</span><span class="sxs-lookup"><span data-stu-id="754f2-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="754f2-113">actionName</span><span class="sxs-lookup"><span data-stu-id="754f2-113">actionName</span></span>|<span data-ttu-id="754f2-114">String</span><span class="sxs-lookup"><span data-stu-id="754f2-114">String</span></span>|<span data-ttu-id="754f2-115">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) から継承されるアクション名</span><span class="sxs-lookup"><span data-stu-id="754f2-115">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="754f2-116">actionState</span><span class="sxs-lookup"><span data-stu-id="754f2-116">actionState</span></span>|[<span data-ttu-id="754f2-117">actionState</span><span class="sxs-lookup"><span data-stu-id="754f2-117">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="754f2-118">[DeviceActionResult](../resources/intune-devices-deviceactionresult.md)から継承される、アクションの状態です。</span><span class="sxs-lookup"><span data-stu-id="754f2-118">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="754f2-119">可能な値は、`none`、`pending`、`canceled`、`active`、`done`、`failed`、`notSupported` です。</span><span class="sxs-lookup"><span data-stu-id="754f2-119">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="754f2-120">startDateTime</span><span class="sxs-lookup"><span data-stu-id="754f2-120">startDateTime</span></span>|<span data-ttu-id="754f2-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="754f2-121">DateTimeOffset</span></span>|<span data-ttu-id="754f2-122">アクションが開始された時刻 ([deviceActionResult](../resources/intune-devices-deviceactionresult.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="754f2-122">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="754f2-123">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="754f2-123">lastUpdatedDateTime</span></span>|<span data-ttu-id="754f2-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="754f2-124">DateTimeOffset</span></span>|<span data-ttu-id="754f2-125">アクション状態の最終更新時刻。[deviceActionResult](../resources/intune-devices-deviceactionresult.md) から継承</span><span class="sxs-lookup"><span data-stu-id="754f2-125">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="754f2-126">scanType</span><span class="sxs-lookup"><span data-stu-id="754f2-126">scanType</span></span>|<span data-ttu-id="754f2-127">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="754f2-127">String</span></span>|<span data-ttu-id="754f2-128">スキャンの種類。フル スキャンまたはクイック スキャン</span><span class="sxs-lookup"><span data-stu-id="754f2-128">Scan type either full scan or quick scan</span></span>|

## <a name="relationships"></a><span data-ttu-id="754f2-129">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="754f2-129">Relationships</span></span>
<span data-ttu-id="754f2-130">なし</span><span class="sxs-lookup"><span data-stu-id="754f2-130">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="754f2-131">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="754f2-131">JSON Representation</span></span>
<span data-ttu-id="754f2-132">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="754f2-132">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsDefenderScanActionResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsDefenderScanActionResult",
  "actionName": "String",
  "actionState": "String",
  "startDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)",
  "scanType": "String"
}
```





