---
title: vppTokenActionResult リソースの種類
description: Apple Volume Purchase Program トークンを使用して実行されたアクションの状態。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0faeee14db33366f8d48645e7419a97e6909398c
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33940107"
---
# <a name="vpptokenactionresult-resource-type"></a><span data-ttu-id="aa4a5-103">vppTokenActionResult リソースの種類</span><span class="sxs-lookup"><span data-stu-id="aa4a5-103">vppTokenActionResult resource type</span></span>

> <span data-ttu-id="aa4a5-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="aa4a5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="aa4a5-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="aa4a5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="aa4a5-106">Apple Volume Purchase Program トークンを使用して実行されたアクションの状態。</span><span class="sxs-lookup"><span data-stu-id="aa4a5-106">The status of the action performed with an Apple Volume Purchase Program token.</span></span>

## <a name="properties"></a><span data-ttu-id="aa4a5-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="aa4a5-107">Properties</span></span>
|<span data-ttu-id="aa4a5-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="aa4a5-108">Property</span></span>|<span data-ttu-id="aa4a5-109">型</span><span class="sxs-lookup"><span data-stu-id="aa4a5-109">Type</span></span>|<span data-ttu-id="aa4a5-110">説明</span><span class="sxs-lookup"><span data-stu-id="aa4a5-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aa4a5-111">actionName</span><span class="sxs-lookup"><span data-stu-id="aa4a5-111">actionName</span></span>|<span data-ttu-id="aa4a5-112">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="aa4a5-112">String</span></span>|<span data-ttu-id="aa4a5-113">アクション名</span><span class="sxs-lookup"><span data-stu-id="aa4a5-113">Action name</span></span>|
|<span data-ttu-id="aa4a5-114">actionState</span><span class="sxs-lookup"><span data-stu-id="aa4a5-114">actionState</span></span>|[<span data-ttu-id="aa4a5-115">actionState</span><span class="sxs-lookup"><span data-stu-id="aa4a5-115">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="aa4a5-116">アクションの状態。</span><span class="sxs-lookup"><span data-stu-id="aa4a5-116">State of the action.</span></span> <span data-ttu-id="aa4a5-117">可能な値は、`none`、`pending`、`canceled`、`active`、`done`、`failed`、`notSupported` です。</span><span class="sxs-lookup"><span data-stu-id="aa4a5-117">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="aa4a5-118">startDateTime</span><span class="sxs-lookup"><span data-stu-id="aa4a5-118">startDateTime</span></span>|<span data-ttu-id="aa4a5-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aa4a5-119">DateTimeOffset</span></span>|<span data-ttu-id="aa4a5-120">アクションが開始された時刻</span><span class="sxs-lookup"><span data-stu-id="aa4a5-120">Time the action was initiated</span></span>|
|<span data-ttu-id="aa4a5-121">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="aa4a5-121">lastUpdatedDateTime</span></span>|<span data-ttu-id="aa4a5-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aa4a5-122">DateTimeOffset</span></span>|<span data-ttu-id="aa4a5-123">アクション状態の最終更新時刻</span><span class="sxs-lookup"><span data-stu-id="aa4a5-123">Time the action state was last updated</span></span>|

## <a name="relationships"></a><span data-ttu-id="aa4a5-124">関係</span><span class="sxs-lookup"><span data-stu-id="aa4a5-124">Relationships</span></span>
<span data-ttu-id="aa4a5-125">なし</span><span class="sxs-lookup"><span data-stu-id="aa4a5-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="aa4a5-126">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="aa4a5-126">JSON Representation</span></span>
<span data-ttu-id="aa4a5-127">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="aa4a5-127">Here is a JSON representation of the resource.</span></span>
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




