---
title: deviceActionResult リソースの種類
description: デバイス アクションの結果
author: tfitzmac
ms.openlocfilehash: fd2160c501820ec04a94b618b3456a3f8fafa6cd
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27324949"
---
# <a name="deviceactionresult-resource-type"></a><span data-ttu-id="b2708-103">deviceActionResult リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b2708-103">deviceActionResult resource type</span></span>

> <span data-ttu-id="b2708-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="b2708-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b2708-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b2708-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b2708-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="b2708-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b2708-107">デバイス アクションの結果</span><span class="sxs-lookup"><span data-stu-id="b2708-107">Device action result</span></span>
## <a name="properties"></a><span data-ttu-id="b2708-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b2708-108">Properties</span></span>
|<span data-ttu-id="b2708-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b2708-109">Property</span></span>|<span data-ttu-id="b2708-110">種類</span><span class="sxs-lookup"><span data-stu-id="b2708-110">Type</span></span>|<span data-ttu-id="b2708-111">説明</span><span class="sxs-lookup"><span data-stu-id="b2708-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b2708-112">actionName</span><span class="sxs-lookup"><span data-stu-id="b2708-112">actionName</span></span>|<span data-ttu-id="b2708-113">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="b2708-113">String</span></span>|<span data-ttu-id="b2708-114">アクション名</span><span class="sxs-lookup"><span data-stu-id="b2708-114">Action name</span></span>|
|<span data-ttu-id="b2708-115">actionState</span><span class="sxs-lookup"><span data-stu-id="b2708-115">actionState</span></span>|[<span data-ttu-id="b2708-116">actionState</span><span class="sxs-lookup"><span data-stu-id="b2708-116">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="b2708-117">アクションの状態です。</span><span class="sxs-lookup"><span data-stu-id="b2708-117">State of the action.</span></span> <span data-ttu-id="b2708-118">可能な値は、`none`、`pending`、`canceled`、`active`、`done`、`failed`、`notSupported` です。</span><span class="sxs-lookup"><span data-stu-id="b2708-118">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="b2708-119">startDateTime</span><span class="sxs-lookup"><span data-stu-id="b2708-119">startDateTime</span></span>|<span data-ttu-id="b2708-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b2708-120">DateTimeOffset</span></span>|<span data-ttu-id="b2708-121">アクションが開始された時刻</span><span class="sxs-lookup"><span data-stu-id="b2708-121">Time the action was initiated</span></span>|
|<span data-ttu-id="b2708-122">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="b2708-122">lastUpdatedDateTime</span></span>|<span data-ttu-id="b2708-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b2708-123">DateTimeOffset</span></span>|<span data-ttu-id="b2708-124">アクション状態の最終更新時刻</span><span class="sxs-lookup"><span data-stu-id="b2708-124">Time the action state was last updated</span></span>|

## <a name="relationships"></a><span data-ttu-id="b2708-125">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="b2708-125">Relationships</span></span>
<span data-ttu-id="b2708-126">なし</span><span class="sxs-lookup"><span data-stu-id="b2708-126">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="b2708-127">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b2708-127">JSON Representation</span></span>
<span data-ttu-id="b2708-128">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="b2708-128">Here is a JSON representation of the resource.</span></span>
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





