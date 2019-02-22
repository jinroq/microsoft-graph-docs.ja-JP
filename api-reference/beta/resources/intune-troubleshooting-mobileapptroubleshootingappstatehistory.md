---
title: mobileAppTroubleshootingAppStateHistory リソースの種類
description: モバイルアプリのトラブルシューティングイベントに含まれる履歴アイテム。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: bd39115de207532b42d1554da54e154a5066eb76
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30150961"
---
# <a name="mobileapptroubleshootingappstatehistory-resource-type"></a><span data-ttu-id="e471a-103">mobileAppTroubleshootingAppStateHistory リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e471a-103">mobileAppTroubleshootingAppStateHistory resource type</span></span>

> <span data-ttu-id="e471a-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e471a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e471a-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="e471a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e471a-106">モバイルアプリのトラブルシューティングイベントに含まれる履歴アイテム。</span><span class="sxs-lookup"><span data-stu-id="e471a-106">History Item contained in the Mobile App Troubleshooting Event.</span></span>


<span data-ttu-id="e471a-107">[mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="e471a-107">Inherits from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="e471a-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e471a-108">Properties</span></span>
|<span data-ttu-id="e471a-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e471a-109">Property</span></span>|<span data-ttu-id="e471a-110">型</span><span class="sxs-lookup"><span data-stu-id="e471a-110">Type</span></span>|<span data-ttu-id="e471a-111">説明</span><span class="sxs-lookup"><span data-stu-id="e471a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e471a-112">occurrenceDateTime</span><span class="sxs-lookup"><span data-stu-id="e471a-112">occurrenceDateTime</span></span>|<span data-ttu-id="e471a-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e471a-113">DateTimeOffset</span></span>|<span data-ttu-id="e471a-114">履歴アイテムが発生した時刻。</span><span class="sxs-lookup"><span data-stu-id="e471a-114">Time when the history item occurred.</span></span> <span data-ttu-id="e471a-115">[mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="e471a-115">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|
|<span data-ttu-id="e471a-116">actionType</span><span class="sxs-lookup"><span data-stu-id="e471a-116">actionType</span></span>|[<span data-ttu-id="e471a-117">mobileAppActionType</span><span class="sxs-lookup"><span data-stu-id="e471a-117">mobileAppActionType</span></span>](../resources/intune-troubleshooting-mobileappactiontype.md)|<span data-ttu-id="e471a-118">対象となった AAD セキュリティグループ id。</span><span class="sxs-lookup"><span data-stu-id="e471a-118">AAD security group id to which it was targeted.</span></span> <span data-ttu-id="e471a-119">可能な値は、`unknown`、`installCommandSent`、`installed`、`uninstalled`、`userRequestedInstall` です。</span><span class="sxs-lookup"><span data-stu-id="e471a-119">Possible values are: `unknown`, `installCommandSent`, `installed`, `uninstalled`, `userRequestedInstall`.</span></span>|
|<span data-ttu-id="e471a-120">runstate</span><span class="sxs-lookup"><span data-stu-id="e471a-120">runState</span></span>|[<span data-ttu-id="e471a-121">runstate</span><span class="sxs-lookup"><span data-stu-id="e471a-121">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="e471a-122">アイテムの状態。</span><span class="sxs-lookup"><span data-stu-id="e471a-122">Status of the item.</span></span> <span data-ttu-id="e471a-123">可能な値は `unknown`、`success`、`fail` です。</span><span class="sxs-lookup"><span data-stu-id="e471a-123">Possible values are: `unknown`, `success`, `fail`.</span></span>|
|<span data-ttu-id="e471a-124">errorCode</span><span class="sxs-lookup"><span data-stu-id="e471a-124">errorCode</span></span>|<span data-ttu-id="e471a-125">String</span><span class="sxs-lookup"><span data-stu-id="e471a-125">String</span></span>|<span data-ttu-id="e471a-126">失敗のエラーコード。エラーがない場合は空です。</span><span class="sxs-lookup"><span data-stu-id="e471a-126">Error code for the failure, empty if no failure.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e471a-127">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="e471a-127">Relationships</span></span>
<span data-ttu-id="e471a-128">なし</span><span class="sxs-lookup"><span data-stu-id="e471a-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e471a-129">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e471a-129">JSON Representation</span></span>
<span data-ttu-id="e471a-130">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="e471a-130">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mobileAppTroubleshootingAppStateHistory"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppTroubleshootingAppStateHistory",
  "occurrenceDateTime": "String (timestamp)",
  "actionType": "String",
  "runState": "String",
  "errorCode": "String"
}
```




