---
title: resetPasscodeActionResult リソースの種類
description: パスコードのリセット アクションの結果
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 5c022d2531bd1576ab7e336193d2f488f5f89f98
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29407047"
---
# <a name="resetpasscodeactionresult-resource-type"></a><span data-ttu-id="c8966-103">resetPasscodeActionResult リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c8966-103">resetPasscodeActionResult resource type</span></span>

> <span data-ttu-id="c8966-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="c8966-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="c8966-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c8966-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c8966-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="c8966-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c8966-107">パスコードのリセット アクションの結果</span><span class="sxs-lookup"><span data-stu-id="c8966-107">Reset passcode action result</span></span>


<span data-ttu-id="c8966-108">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="c8966-108">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c8966-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c8966-109">Properties</span></span>
|<span data-ttu-id="c8966-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c8966-110">Property</span></span>|<span data-ttu-id="c8966-111">型</span><span class="sxs-lookup"><span data-stu-id="c8966-111">Type</span></span>|<span data-ttu-id="c8966-112">説明</span><span class="sxs-lookup"><span data-stu-id="c8966-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c8966-113">actionName</span><span class="sxs-lookup"><span data-stu-id="c8966-113">actionName</span></span>|<span data-ttu-id="c8966-114">String</span><span class="sxs-lookup"><span data-stu-id="c8966-114">String</span></span>|<span data-ttu-id="c8966-115">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) から継承されるアクション名</span><span class="sxs-lookup"><span data-stu-id="c8966-115">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="c8966-116">actionState</span><span class="sxs-lookup"><span data-stu-id="c8966-116">actionState</span></span>|[<span data-ttu-id="c8966-117">actionState</span><span class="sxs-lookup"><span data-stu-id="c8966-117">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="c8966-118">[DeviceActionResult](../resources/intune-devices-deviceactionresult.md)から継承される、アクションの状態です。</span><span class="sxs-lookup"><span data-stu-id="c8966-118">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="c8966-119">可能な値は、`none`、`pending`、`canceled`、`active`、`done`、`failed`、`notSupported` です。</span><span class="sxs-lookup"><span data-stu-id="c8966-119">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="c8966-120">startDateTime</span><span class="sxs-lookup"><span data-stu-id="c8966-120">startDateTime</span></span>|<span data-ttu-id="c8966-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c8966-121">DateTimeOffset</span></span>|<span data-ttu-id="c8966-122">アクションが開始された時刻 ([deviceActionResult](../resources/intune-devices-deviceactionresult.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="c8966-122">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="c8966-123">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="c8966-123">lastUpdatedDateTime</span></span>|<span data-ttu-id="c8966-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c8966-124">DateTimeOffset</span></span>|<span data-ttu-id="c8966-125">アクション状態の最終更新時刻。[deviceActionResult](../resources/intune-devices-deviceactionresult.md) から継承</span><span class="sxs-lookup"><span data-stu-id="c8966-125">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="c8966-126">passcode</span><span class="sxs-lookup"><span data-stu-id="c8966-126">passcode</span></span>|<span data-ttu-id="c8966-127">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="c8966-127">String</span></span>|<span data-ttu-id="c8966-128">デバイス用に新たに生成されたパスコード</span><span class="sxs-lookup"><span data-stu-id="c8966-128">Newly generated passcode for the device</span></span> |

## <a name="relationships"></a><span data-ttu-id="c8966-129">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="c8966-129">Relationships</span></span>
<span data-ttu-id="c8966-130">なし</span><span class="sxs-lookup"><span data-stu-id="c8966-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c8966-131">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c8966-131">JSON Representation</span></span>
<span data-ttu-id="c8966-132">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="c8966-132">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.resetPasscodeActionResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.resetPasscodeActionResult",
  "actionName": "String",
  "actionState": "String",
  "startDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)",
  "passcode": "String"
}
```




