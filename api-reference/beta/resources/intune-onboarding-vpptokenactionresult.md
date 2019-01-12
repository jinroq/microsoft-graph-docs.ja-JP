---
title: vppTokenActionResult リソースの種類
description: アクションのステータスは、Apple ボリューム購入プログラム トークンで実行されます。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: f3aa2467d8f30c023a7564817a2da9e1c970125f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27961919"
---
# <a name="vpptokenactionresult-resource-type"></a><span data-ttu-id="9b75b-103">vppTokenActionResult リソースの種類</span><span class="sxs-lookup"><span data-stu-id="9b75b-103">vppTokenActionResult resource type</span></span>

> <span data-ttu-id="9b75b-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="9b75b-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9b75b-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9b75b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9b75b-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="9b75b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9b75b-107">アクションのステータスは、Apple ボリューム購入プログラム トークンで実行されます。</span><span class="sxs-lookup"><span data-stu-id="9b75b-107">The status of the action performed with an Apple Volume Purchase Program token.</span></span>
## <a name="properties"></a><span data-ttu-id="9b75b-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9b75b-108">Properties</span></span>
|<span data-ttu-id="9b75b-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9b75b-109">Property</span></span>|<span data-ttu-id="9b75b-110">型</span><span class="sxs-lookup"><span data-stu-id="9b75b-110">Type</span></span>|<span data-ttu-id="9b75b-111">説明</span><span class="sxs-lookup"><span data-stu-id="9b75b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9b75b-112">actionName</span><span class="sxs-lookup"><span data-stu-id="9b75b-112">actionName</span></span>|<span data-ttu-id="9b75b-113">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="9b75b-113">String</span></span>|<span data-ttu-id="9b75b-114">アクション名</span><span class="sxs-lookup"><span data-stu-id="9b75b-114">Action name</span></span>|
|<span data-ttu-id="9b75b-115">actionState</span><span class="sxs-lookup"><span data-stu-id="9b75b-115">actionState</span></span>|[<span data-ttu-id="9b75b-116">actionState</span><span class="sxs-lookup"><span data-stu-id="9b75b-116">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="9b75b-117">アクションの状態です。</span><span class="sxs-lookup"><span data-stu-id="9b75b-117">State of the action.</span></span> <span data-ttu-id="9b75b-118">可能な値は、`none`、`pending`、`canceled`、`active`、`done`、`failed`、`notSupported` です。</span><span class="sxs-lookup"><span data-stu-id="9b75b-118">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="9b75b-119">startDateTime</span><span class="sxs-lookup"><span data-stu-id="9b75b-119">startDateTime</span></span>|<span data-ttu-id="9b75b-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9b75b-120">DateTimeOffset</span></span>|<span data-ttu-id="9b75b-121">アクションが開始された時刻</span><span class="sxs-lookup"><span data-stu-id="9b75b-121">Time the action was initiated</span></span>|
|<span data-ttu-id="9b75b-122">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="9b75b-122">lastUpdatedDateTime</span></span>|<span data-ttu-id="9b75b-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9b75b-123">DateTimeOffset</span></span>|<span data-ttu-id="9b75b-124">アクション状態の最終更新時刻</span><span class="sxs-lookup"><span data-stu-id="9b75b-124">Time the action state was last updated</span></span>|

## <a name="relationships"></a><span data-ttu-id="9b75b-125">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="9b75b-125">Relationships</span></span>
<span data-ttu-id="9b75b-126">なし</span><span class="sxs-lookup"><span data-stu-id="9b75b-126">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="9b75b-127">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="9b75b-127">JSON Representation</span></span>
<span data-ttu-id="9b75b-128">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="9b75b-128">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.vppTokenActionResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.vppTokenActionResult",
  "actionName": "String",
  "actionState": "String",
  "startDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)"
}
```





