---
title: resetPasscodeActionResult リソースの種類
description: パスコードのリセット アクションの結果
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 61f70e9de99b831e650fa08d3d59e5359a9d93ec
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33941780"
---
# <a name="resetpasscodeactionresult-resource-type"></a><span data-ttu-id="bca39-103">resetPasscodeActionResult リソースの種類</span><span class="sxs-lookup"><span data-stu-id="bca39-103">resetPasscodeActionResult resource type</span></span>

> <span data-ttu-id="bca39-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bca39-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bca39-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="bca39-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bca39-106">パスコードのリセット アクションの結果</span><span class="sxs-lookup"><span data-stu-id="bca39-106">Reset passcode action result</span></span>


<span data-ttu-id="bca39-107">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="bca39-107">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="bca39-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bca39-108">Properties</span></span>
|<span data-ttu-id="bca39-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bca39-109">Property</span></span>|<span data-ttu-id="bca39-110">型</span><span class="sxs-lookup"><span data-stu-id="bca39-110">Type</span></span>|<span data-ttu-id="bca39-111">説明</span><span class="sxs-lookup"><span data-stu-id="bca39-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bca39-112">actionName</span><span class="sxs-lookup"><span data-stu-id="bca39-112">actionName</span></span>|<span data-ttu-id="bca39-113">String</span><span class="sxs-lookup"><span data-stu-id="bca39-113">String</span></span>|<span data-ttu-id="bca39-114">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) から継承されるアクション名</span><span class="sxs-lookup"><span data-stu-id="bca39-114">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="bca39-115">actionState</span><span class="sxs-lookup"><span data-stu-id="bca39-115">actionState</span></span>|[<span data-ttu-id="bca39-116">actionState</span><span class="sxs-lookup"><span data-stu-id="bca39-116">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="bca39-117">[Deviceactionresult](../resources/intune-devices-deviceactionresult.md)から継承されるアクションの状態。</span><span class="sxs-lookup"><span data-stu-id="bca39-117">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="bca39-118">可能な値は、`none`、`pending`、`canceled`、`active`、`done`、`failed`、`notSupported` です。</span><span class="sxs-lookup"><span data-stu-id="bca39-118">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="bca39-119">startDateTime</span><span class="sxs-lookup"><span data-stu-id="bca39-119">startDateTime</span></span>|<span data-ttu-id="bca39-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bca39-120">DateTimeOffset</span></span>|<span data-ttu-id="bca39-121">アクションが開始された時刻。[deviceActionResult](../resources/intune-devices-deviceactionresult.md) から継承。</span><span class="sxs-lookup"><span data-stu-id="bca39-121">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="bca39-122">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="bca39-122">lastUpdatedDateTime</span></span>|<span data-ttu-id="bca39-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bca39-123">DateTimeOffset</span></span>|<span data-ttu-id="bca39-124">アクション状態の最終更新時刻。[deviceActionResult](../resources/intune-devices-deviceactionresult.md) から継承</span><span class="sxs-lookup"><span data-stu-id="bca39-124">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="bca39-125">passcode</span><span class="sxs-lookup"><span data-stu-id="bca39-125">passcode</span></span>|<span data-ttu-id="bca39-126">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="bca39-126">String</span></span>|<span data-ttu-id="bca39-127">デバイス用に新たに生成されたパスコード</span><span class="sxs-lookup"><span data-stu-id="bca39-127">Newly generated passcode for the device</span></span> |

## <a name="relationships"></a><span data-ttu-id="bca39-128">関係</span><span class="sxs-lookup"><span data-stu-id="bca39-128">Relationships</span></span>
<span data-ttu-id="bca39-129">なし</span><span class="sxs-lookup"><span data-stu-id="bca39-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bca39-130">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="bca39-130">JSON Representation</span></span>
<span data-ttu-id="bca39-131">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="bca39-131">Here is a JSON representation of the resource.</span></span>
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




