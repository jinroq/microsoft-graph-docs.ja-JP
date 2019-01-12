---
title: remoteLockActionResult リソースの種類
description: ロック解除するためのピンが含まれるアクション結果のロック。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 341d1425de71c7175346e1ba6b30fe2a81b696a4
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27922719"
---
# <a name="remotelockactionresult-resource-type"></a><span data-ttu-id="a8e2b-103">remoteLockActionResult リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a8e2b-103">remoteLockActionResult resource type</span></span>

> <span data-ttu-id="a8e2b-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="a8e2b-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a8e2b-105">ロック解除するためのピンが含まれるアクション結果のロック。</span><span class="sxs-lookup"><span data-stu-id="a8e2b-105">Lock action result with a pin to unlock</span></span>

<span data-ttu-id="a8e2b-106">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="a8e2b-106">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="a8e2b-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a8e2b-107">Properties</span></span>
|<span data-ttu-id="a8e2b-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a8e2b-108">Property</span></span>|<span data-ttu-id="a8e2b-109">種類</span><span class="sxs-lookup"><span data-stu-id="a8e2b-109">Type</span></span>|<span data-ttu-id="a8e2b-110">説明</span><span class="sxs-lookup"><span data-stu-id="a8e2b-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a8e2b-111">actionName</span><span class="sxs-lookup"><span data-stu-id="a8e2b-111">actionName</span></span>|<span data-ttu-id="a8e2b-112">String</span><span class="sxs-lookup"><span data-stu-id="a8e2b-112">String</span></span>|<span data-ttu-id="a8e2b-113">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) から継承されるアクション名</span><span class="sxs-lookup"><span data-stu-id="a8e2b-113">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="a8e2b-114">actionState</span><span class="sxs-lookup"><span data-stu-id="a8e2b-114">actionState</span></span>|[<span data-ttu-id="a8e2b-115">actionState</span><span class="sxs-lookup"><span data-stu-id="a8e2b-115">actionState</span></span>](../resources/intune-devices-actionstate.md)|<span data-ttu-id="a8e2b-116">[DeviceActionResult](../resources/intune-devices-deviceactionresult.md)から継承される、アクションの状態です。</span><span class="sxs-lookup"><span data-stu-id="a8e2b-116">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="a8e2b-117">可能な値は、`none`、`pending`、`canceled`、`active`、`done`、`failed`、`notSupported` です。</span><span class="sxs-lookup"><span data-stu-id="a8e2b-117">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="a8e2b-118">startDateTime</span><span class="sxs-lookup"><span data-stu-id="a8e2b-118">startDateTime</span></span>|<span data-ttu-id="a8e2b-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a8e2b-119">DateTimeOffset</span></span>|<span data-ttu-id="a8e2b-120">アクションが開始された時刻 ([deviceActionResult](../resources/intune-devices-deviceactionresult.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="a8e2b-120">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="a8e2b-121">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="a8e2b-121">lastUpdatedDateTime</span></span>|<span data-ttu-id="a8e2b-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a8e2b-122">DateTimeOffset</span></span>|<span data-ttu-id="a8e2b-123">アクション状態の最終更新時刻。[deviceActionResult](../resources/intune-devices-deviceactionresult.md) から継承</span><span class="sxs-lookup"><span data-stu-id="a8e2b-123">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="a8e2b-124">unlockPin</span><span class="sxs-lookup"><span data-stu-id="a8e2b-124">unlockPin</span></span>|<span data-ttu-id="a8e2b-125">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="a8e2b-125">String</span></span>|<span data-ttu-id="a8e2b-126">クライアントをロック解除するためのピン</span><span class="sxs-lookup"><span data-stu-id="a8e2b-126">Pin to unlock the client</span></span>|

## <a name="relationships"></a><span data-ttu-id="a8e2b-127">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="a8e2b-127">Relationships</span></span>
<span data-ttu-id="a8e2b-128">なし</span><span class="sxs-lookup"><span data-stu-id="a8e2b-128">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="a8e2b-129">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a8e2b-129">JSON Representation</span></span>
<span data-ttu-id="a8e2b-130">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="a8e2b-130">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.remoteLockActionResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.remoteLockActionResult",
  "actionName": "String",
  "actionState": "String",
  "startDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)",
  "unlockPin": "String"
}
```



