---
title: resetPasscodeActionResult リソースの種類
description: パスコードのリセット アクションの結果
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 883818d7061f070f01f3e3c9fdfee9e15f322829
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35968261"
---
# <a name="resetpasscodeactionresult-resource-type"></a><span data-ttu-id="1dcdb-103">resetPasscodeActionResult リソースの種類</span><span class="sxs-lookup"><span data-stu-id="1dcdb-103">resetPasscodeActionResult resource type</span></span>

> <span data-ttu-id="1dcdb-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1dcdb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1dcdb-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="1dcdb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1dcdb-106">パスコードのリセット アクションの結果</span><span class="sxs-lookup"><span data-stu-id="1dcdb-106">Reset passcode action result</span></span>


<span data-ttu-id="1dcdb-107">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="1dcdb-107">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="1dcdb-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1dcdb-108">Properties</span></span>
|<span data-ttu-id="1dcdb-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1dcdb-109">Property</span></span>|<span data-ttu-id="1dcdb-110">型</span><span class="sxs-lookup"><span data-stu-id="1dcdb-110">Type</span></span>|<span data-ttu-id="1dcdb-111">説明</span><span class="sxs-lookup"><span data-stu-id="1dcdb-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1dcdb-112">actionName</span><span class="sxs-lookup"><span data-stu-id="1dcdb-112">actionName</span></span>|<span data-ttu-id="1dcdb-113">String</span><span class="sxs-lookup"><span data-stu-id="1dcdb-113">String</span></span>|<span data-ttu-id="1dcdb-114">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) から継承されるアクション名</span><span class="sxs-lookup"><span data-stu-id="1dcdb-114">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="1dcdb-115">actionState</span><span class="sxs-lookup"><span data-stu-id="1dcdb-115">actionState</span></span>|[<span data-ttu-id="1dcdb-116">actionState</span><span class="sxs-lookup"><span data-stu-id="1dcdb-116">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="1dcdb-117">[Deviceactionresult](../resources/intune-devices-deviceactionresult.md)から継承されるアクションの状態。</span><span class="sxs-lookup"><span data-stu-id="1dcdb-117">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="1dcdb-118">可能な値は、`none`、`pending`、`canceled`、`active`、`done`、`failed`、`notSupported` です。</span><span class="sxs-lookup"><span data-stu-id="1dcdb-118">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="1dcdb-119">startDateTime</span><span class="sxs-lookup"><span data-stu-id="1dcdb-119">startDateTime</span></span>|<span data-ttu-id="1dcdb-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1dcdb-120">DateTimeOffset</span></span>|<span data-ttu-id="1dcdb-121">アクションが開始された時刻。[deviceActionResult](../resources/intune-devices-deviceactionresult.md) から継承。</span><span class="sxs-lookup"><span data-stu-id="1dcdb-121">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="1dcdb-122">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="1dcdb-122">lastUpdatedDateTime</span></span>|<span data-ttu-id="1dcdb-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1dcdb-123">DateTimeOffset</span></span>|<span data-ttu-id="1dcdb-124">アクション状態の最終更新時刻。[deviceActionResult](../resources/intune-devices-deviceactionresult.md) から継承</span><span class="sxs-lookup"><span data-stu-id="1dcdb-124">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="1dcdb-125">passcode</span><span class="sxs-lookup"><span data-stu-id="1dcdb-125">passcode</span></span>|<span data-ttu-id="1dcdb-126">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="1dcdb-126">String</span></span>|<span data-ttu-id="1dcdb-127">デバイス用に新たに生成されたパスコード</span><span class="sxs-lookup"><span data-stu-id="1dcdb-127">Newly generated passcode for the device</span></span> |

## <a name="relationships"></a><span data-ttu-id="1dcdb-128">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="1dcdb-128">Relationships</span></span>
<span data-ttu-id="1dcdb-129">なし</span><span class="sxs-lookup"><span data-stu-id="1dcdb-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1dcdb-130">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="1dcdb-130">JSON Representation</span></span>
<span data-ttu-id="1dcdb-131">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="1dcdb-131">Here is a JSON representation of the resource.</span></span>
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





