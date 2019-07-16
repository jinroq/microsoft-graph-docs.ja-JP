---
title: mobileAppTroubleshootingAppStateHistory リソースの種類
description: モバイルアプリのトラブルシューティングイベントに含まれる履歴アイテム。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: efef2bb43c34c004df48453ca6a2713d445ec970
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35737364"
---
# <a name="mobileapptroubleshootingappstatehistory-resource-type"></a><span data-ttu-id="e8753-103">mobileAppTroubleshootingAppStateHistory リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e8753-103">mobileAppTroubleshootingAppStateHistory resource type</span></span>

> <span data-ttu-id="e8753-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e8753-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e8753-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="e8753-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e8753-106">モバイルアプリのトラブルシューティングイベントに含まれる履歴アイテム。</span><span class="sxs-lookup"><span data-stu-id="e8753-106">History Item contained in the Mobile App Troubleshooting Event.</span></span>


<span data-ttu-id="e8753-107">[MobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="e8753-107">Inherits from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="e8753-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e8753-108">Properties</span></span>
|<span data-ttu-id="e8753-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e8753-109">Property</span></span>|<span data-ttu-id="e8753-110">型</span><span class="sxs-lookup"><span data-stu-id="e8753-110">Type</span></span>|<span data-ttu-id="e8753-111">説明</span><span class="sxs-lookup"><span data-stu-id="e8753-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e8753-112">occurrenceDateTime</span><span class="sxs-lookup"><span data-stu-id="e8753-112">occurrenceDateTime</span></span>|<span data-ttu-id="e8753-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e8753-113">DateTimeOffset</span></span>|<span data-ttu-id="e8753-114">履歴アイテムが発生した時刻。</span><span class="sxs-lookup"><span data-stu-id="e8753-114">Time when the history item occurred.</span></span> <span data-ttu-id="e8753-115">[MobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="e8753-115">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|
|<span data-ttu-id="e8753-116">actionType</span><span class="sxs-lookup"><span data-stu-id="e8753-116">actionType</span></span>|[<span data-ttu-id="e8753-117">mobileAppActionType</span><span class="sxs-lookup"><span data-stu-id="e8753-117">mobileAppActionType</span></span>](../resources/intune-troubleshooting-mobileappactiontype.md)|<span data-ttu-id="e8753-118">Intune アプリケーションのアクションの種類。</span><span class="sxs-lookup"><span data-stu-id="e8753-118">Action type for Intune Application.</span></span> <span data-ttu-id="e8753-119">可能な値は、`unknown`、`installCommandSent`、`installed`、`uninstalled`、`userRequestedInstall` です。</span><span class="sxs-lookup"><span data-stu-id="e8753-119">Possible values are: `unknown`, `installCommandSent`, `installed`, `uninstalled`, `userRequestedInstall`.</span></span>|
|<span data-ttu-id="e8753-120">runState</span><span class="sxs-lookup"><span data-stu-id="e8753-120">runState</span></span>|[<span data-ttu-id="e8753-121">runState</span><span class="sxs-lookup"><span data-stu-id="e8753-121">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="e8753-122">アイテムの状態。</span><span class="sxs-lookup"><span data-stu-id="e8753-122">Status of the item.</span></span> <span data-ttu-id="e8753-123">可能な値は、`unknown`、`success`、`fail` です。</span><span class="sxs-lookup"><span data-stu-id="e8753-123">Possible values are: `unknown`, `success`, `fail`.</span></span>|
|<span data-ttu-id="e8753-124">errorCode</span><span class="sxs-lookup"><span data-stu-id="e8753-124">errorCode</span></span>|<span data-ttu-id="e8753-125">String</span><span class="sxs-lookup"><span data-stu-id="e8753-125">String</span></span>|<span data-ttu-id="e8753-126">失敗のエラーコード。エラーがない場合は空です。</span><span class="sxs-lookup"><span data-stu-id="e8753-126">Error code for the failure, empty if no failure.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e8753-127">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="e8753-127">Relationships</span></span>
<span data-ttu-id="e8753-128">なし</span><span class="sxs-lookup"><span data-stu-id="e8753-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e8753-129">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e8753-129">JSON Representation</span></span>
<span data-ttu-id="e8753-130">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="e8753-130">Here is a JSON representation of the resource.</span></span>
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





