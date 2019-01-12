---
title: resetPasscodeActionResult リソースの種類
description: パスコードのリセット アクションの結果
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: e526370ca86792ed30a5f5e24a4be244d73441b6
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27920843"
---
# <a name="resetpasscodeactionresult-resource-type"></a><span data-ttu-id="526be-103">resetPasscodeActionResult リソースの種類</span><span class="sxs-lookup"><span data-stu-id="526be-103">resetPasscodeActionResult resource type</span></span>

> <span data-ttu-id="526be-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="526be-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="526be-105">パスコードのリセット アクションの結果</span><span class="sxs-lookup"><span data-stu-id="526be-105">Reset passcode action result</span></span>

<span data-ttu-id="526be-106">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="526be-106">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="526be-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="526be-107">Properties</span></span>
|<span data-ttu-id="526be-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="526be-108">Property</span></span>|<span data-ttu-id="526be-109">種類</span><span class="sxs-lookup"><span data-stu-id="526be-109">Type</span></span>|<span data-ttu-id="526be-110">説明</span><span class="sxs-lookup"><span data-stu-id="526be-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="526be-111">actionName</span><span class="sxs-lookup"><span data-stu-id="526be-111">actionName</span></span>|<span data-ttu-id="526be-112">String</span><span class="sxs-lookup"><span data-stu-id="526be-112">String</span></span>|<span data-ttu-id="526be-113">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) から継承されるアクション名</span><span class="sxs-lookup"><span data-stu-id="526be-113">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="526be-114">actionState</span><span class="sxs-lookup"><span data-stu-id="526be-114">actionState</span></span>|[<span data-ttu-id="526be-115">actionState</span><span class="sxs-lookup"><span data-stu-id="526be-115">actionState</span></span>](../resources/intune-devices-actionstate.md)|<span data-ttu-id="526be-116">[DeviceActionResult](../resources/intune-devices-deviceactionresult.md)から継承される、アクションの状態です。</span><span class="sxs-lookup"><span data-stu-id="526be-116">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="526be-117">可能な値は、`none`、`pending`、`canceled`、`active`、`done`、`failed`、`notSupported` です。</span><span class="sxs-lookup"><span data-stu-id="526be-117">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="526be-118">startDateTime</span><span class="sxs-lookup"><span data-stu-id="526be-118">startDateTime</span></span>|<span data-ttu-id="526be-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="526be-119">DateTimeOffset</span></span>|<span data-ttu-id="526be-120">アクションが開始された時刻 ([deviceActionResult](../resources/intune-devices-deviceactionresult.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="526be-120">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="526be-121">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="526be-121">lastUpdatedDateTime</span></span>|<span data-ttu-id="526be-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="526be-122">DateTimeOffset</span></span>|<span data-ttu-id="526be-123">アクション状態の最終更新時刻。[deviceActionResult](../resources/intune-devices-deviceactionresult.md) から継承</span><span class="sxs-lookup"><span data-stu-id="526be-123">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="526be-124">passcode</span><span class="sxs-lookup"><span data-stu-id="526be-124">passcode</span></span>|<span data-ttu-id="526be-125">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="526be-125">String</span></span>|<span data-ttu-id="526be-126">デバイス用に新たに生成されたパスコード</span><span class="sxs-lookup"><span data-stu-id="526be-126">Newly generated passcode for the device</span></span> |

## <a name="relationships"></a><span data-ttu-id="526be-127">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="526be-127">Relationships</span></span>
<span data-ttu-id="526be-128">なし</span><span class="sxs-lookup"><span data-stu-id="526be-128">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="526be-129">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="526be-129">JSON Representation</span></span>
<span data-ttu-id="526be-130">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="526be-130">Here is a JSON representation of the resource.</span></span>
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



