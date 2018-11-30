---
title: deviceActionResult リソースの種類
description: デバイス アクションの結果
ms.openlocfilehash: 9d7804b994474778f0f06c52079e09ed5887a09f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27023008"
---
# <a name="deviceactionresult-resource-type"></a><span data-ttu-id="c5276-103">deviceActionResult リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c5276-103">deviceActionResult resource type</span></span>

> <span data-ttu-id="c5276-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="c5276-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c5276-105">デバイス アクションの結果</span><span class="sxs-lookup"><span data-stu-id="c5276-105">Device action result</span></span>
## <a name="properties"></a><span data-ttu-id="c5276-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c5276-106">Properties</span></span>
|<span data-ttu-id="c5276-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c5276-107">Property</span></span>|<span data-ttu-id="c5276-108">型</span><span class="sxs-lookup"><span data-stu-id="c5276-108">Type</span></span>|<span data-ttu-id="c5276-109">説明</span><span class="sxs-lookup"><span data-stu-id="c5276-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c5276-110">actionName</span><span class="sxs-lookup"><span data-stu-id="c5276-110">actionName</span></span>|<span data-ttu-id="c5276-111">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="c5276-111">String</span></span>|<span data-ttu-id="c5276-112">アクション名</span><span class="sxs-lookup"><span data-stu-id="c5276-112">Action name</span></span>|
|<span data-ttu-id="c5276-113">actionState</span><span class="sxs-lookup"><span data-stu-id="c5276-113">actionState</span></span>|[<span data-ttu-id="c5276-114">actionState</span><span class="sxs-lookup"><span data-stu-id="c5276-114">actionState</span></span>](../resources/intune-devices-actionstate.md)|<span data-ttu-id="c5276-115">アクションの状態です。</span><span class="sxs-lookup"><span data-stu-id="c5276-115">State of the action.</span></span> <span data-ttu-id="c5276-116">可能な値は、`none`、`pending`、`canceled`、`active`、`done`、`failed`、`notSupported` です。</span><span class="sxs-lookup"><span data-stu-id="c5276-116">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="c5276-117">startDateTime</span><span class="sxs-lookup"><span data-stu-id="c5276-117">startDateTime</span></span>|<span data-ttu-id="c5276-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c5276-118">DateTimeOffset</span></span>|<span data-ttu-id="c5276-119">アクションが開始された時刻</span><span class="sxs-lookup"><span data-stu-id="c5276-119">Time the action was initiated</span></span>|
|<span data-ttu-id="c5276-120">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="c5276-120">lastUpdatedDateTime</span></span>|<span data-ttu-id="c5276-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c5276-121">DateTimeOffset</span></span>|<span data-ttu-id="c5276-122">アクション状態の最終更新時刻</span><span class="sxs-lookup"><span data-stu-id="c5276-122">Time the action state was last updated</span></span>|

## <a name="relationships"></a><span data-ttu-id="c5276-123">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="c5276-123">Relationships</span></span>
<span data-ttu-id="c5276-124">なし</span><span class="sxs-lookup"><span data-stu-id="c5276-124">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="c5276-125">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c5276-125">JSON Representation</span></span>
<span data-ttu-id="c5276-126">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="c5276-126">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceActionResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceActionResult",
  "actionName": "String",
  "actionState": "String",
  "startDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)"
}
```


