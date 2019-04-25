---
title: resetPasscodeActionResult リソースの種類
description: パスコードのリセット アクションの結果
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2e23c3e7d39566df98ab57258a54ab6f637439d1
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32523687"
---
# <a name="resetpasscodeactionresult-resource-type"></a><span data-ttu-id="b5048-103">resetPasscodeActionResult リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b5048-103">resetPasscodeActionResult resource type</span></span>

> <span data-ttu-id="b5048-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="b5048-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b5048-105">パスコードのリセット アクションの結果</span><span class="sxs-lookup"><span data-stu-id="b5048-105">Reset passcode action result</span></span>


<span data-ttu-id="b5048-106">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="b5048-106">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="b5048-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b5048-107">Properties</span></span>
|<span data-ttu-id="b5048-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b5048-108">Property</span></span>|<span data-ttu-id="b5048-109">型</span><span class="sxs-lookup"><span data-stu-id="b5048-109">Type</span></span>|<span data-ttu-id="b5048-110">説明</span><span class="sxs-lookup"><span data-stu-id="b5048-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b5048-111">actionName</span><span class="sxs-lookup"><span data-stu-id="b5048-111">actionName</span></span>|<span data-ttu-id="b5048-112">String</span><span class="sxs-lookup"><span data-stu-id="b5048-112">String</span></span>|<span data-ttu-id="b5048-113">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) から継承されるアクション名</span><span class="sxs-lookup"><span data-stu-id="b5048-113">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="b5048-114">actionState</span><span class="sxs-lookup"><span data-stu-id="b5048-114">actionState</span></span>|[<span data-ttu-id="b5048-115">actionState</span><span class="sxs-lookup"><span data-stu-id="b5048-115">actionState</span></span>](../resources/intune-devices-actionstate.md)|<span data-ttu-id="b5048-116">[deviceactionresult](../resources/intune-devices-deviceactionresult.md)から継承されるアクションの状態。</span><span class="sxs-lookup"><span data-stu-id="b5048-116">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="b5048-117">可能な値は、`none`、`pending`、`canceled`、`active`、`done`、`failed`、`notSupported` です。</span><span class="sxs-lookup"><span data-stu-id="b5048-117">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="b5048-118">startDateTime</span><span class="sxs-lookup"><span data-stu-id="b5048-118">startDateTime</span></span>|<span data-ttu-id="b5048-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b5048-119">DateTimeOffset</span></span>|<span data-ttu-id="b5048-120">アクションが開始された時刻。[deviceActionResult](../resources/intune-devices-deviceactionresult.md) から継承。</span><span class="sxs-lookup"><span data-stu-id="b5048-120">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="b5048-121">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="b5048-121">lastUpdatedDateTime</span></span>|<span data-ttu-id="b5048-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b5048-122">DateTimeOffset</span></span>|<span data-ttu-id="b5048-123">アクション状態の最終更新時刻。[deviceActionResult](../resources/intune-devices-deviceactionresult.md) から継承</span><span class="sxs-lookup"><span data-stu-id="b5048-123">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="b5048-124">passcode</span><span class="sxs-lookup"><span data-stu-id="b5048-124">passcode</span></span>|<span data-ttu-id="b5048-125">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="b5048-125">String</span></span>|<span data-ttu-id="b5048-126">デバイス用に新たに生成されたパスコード</span><span class="sxs-lookup"><span data-stu-id="b5048-126">Newly generated passcode for the device</span></span> |

## <a name="relationships"></a><span data-ttu-id="b5048-127">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="b5048-127">Relationships</span></span>
<span data-ttu-id="b5048-128">なし</span><span class="sxs-lookup"><span data-stu-id="b5048-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b5048-129">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b5048-129">JSON Representation</span></span>
<span data-ttu-id="b5048-130">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="b5048-130">Here is a JSON representation of the resource.</span></span>
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



