---
title: mobileAppTroubleshootingAppStateHistory リソースの種類
description: モバイルアプリのトラブルシューティングイベントに含まれる履歴アイテム。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 2d145212645283738d1248bd05c50b1f6658460f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35967218"
---
# <a name="mobileapptroubleshootingappstatehistory-resource-type"></a><span data-ttu-id="9e2c6-103">mobileAppTroubleshootingAppStateHistory リソースの種類</span><span class="sxs-lookup"><span data-stu-id="9e2c6-103">mobileAppTroubleshootingAppStateHistory resource type</span></span>

> <span data-ttu-id="9e2c6-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9e2c6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9e2c6-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="9e2c6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9e2c6-106">モバイルアプリのトラブルシューティングイベントに含まれる履歴アイテム。</span><span class="sxs-lookup"><span data-stu-id="9e2c6-106">History Item contained in the Mobile App Troubleshooting Event.</span></span>


<span data-ttu-id="9e2c6-107">[MobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="9e2c6-107">Inherits from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="9e2c6-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9e2c6-108">Properties</span></span>
|<span data-ttu-id="9e2c6-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9e2c6-109">Property</span></span>|<span data-ttu-id="9e2c6-110">型</span><span class="sxs-lookup"><span data-stu-id="9e2c6-110">Type</span></span>|<span data-ttu-id="9e2c6-111">説明</span><span class="sxs-lookup"><span data-stu-id="9e2c6-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9e2c6-112">occurrenceDateTime</span><span class="sxs-lookup"><span data-stu-id="9e2c6-112">occurrenceDateTime</span></span>|<span data-ttu-id="9e2c6-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9e2c6-113">DateTimeOffset</span></span>|<span data-ttu-id="9e2c6-114">履歴アイテムが発生した時刻。</span><span class="sxs-lookup"><span data-stu-id="9e2c6-114">Time when the history item occurred.</span></span> <span data-ttu-id="9e2c6-115">[MobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="9e2c6-115">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|
|<span data-ttu-id="9e2c6-116">actionType</span><span class="sxs-lookup"><span data-stu-id="9e2c6-116">actionType</span></span>|[<span data-ttu-id="9e2c6-117">mobileAppActionType</span><span class="sxs-lookup"><span data-stu-id="9e2c6-117">mobileAppActionType</span></span>](../resources/intune-troubleshooting-mobileappactiontype.md)|<span data-ttu-id="9e2c6-118">Intune アプリケーションのアクションの種類。</span><span class="sxs-lookup"><span data-stu-id="9e2c6-118">Action type for Intune Application.</span></span> <span data-ttu-id="9e2c6-119">可能な値は、`unknown`、`installCommandSent`、`installed`、`uninstalled`、`userRequestedInstall` です。</span><span class="sxs-lookup"><span data-stu-id="9e2c6-119">Possible values are: `unknown`, `installCommandSent`, `installed`, `uninstalled`, `userRequestedInstall`.</span></span>|
|<span data-ttu-id="9e2c6-120">runState</span><span class="sxs-lookup"><span data-stu-id="9e2c6-120">runState</span></span>|[<span data-ttu-id="9e2c6-121">runState</span><span class="sxs-lookup"><span data-stu-id="9e2c6-121">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="9e2c6-122">アイテムの状態。</span><span class="sxs-lookup"><span data-stu-id="9e2c6-122">Status of the item.</span></span> <span data-ttu-id="9e2c6-123">可能な値は、`unknown`、`success`、`fail` です。</span><span class="sxs-lookup"><span data-stu-id="9e2c6-123">Possible values are: `unknown`, `success`, `fail`.</span></span>|
|<span data-ttu-id="9e2c6-124">errorCode</span><span class="sxs-lookup"><span data-stu-id="9e2c6-124">errorCode</span></span>|<span data-ttu-id="9e2c6-125">String</span><span class="sxs-lookup"><span data-stu-id="9e2c6-125">String</span></span>|<span data-ttu-id="9e2c6-126">失敗のエラーコード。エラーがない場合は空です。</span><span class="sxs-lookup"><span data-stu-id="9e2c6-126">Error code for the failure, empty if no failure.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9e2c6-127">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="9e2c6-127">Relationships</span></span>
<span data-ttu-id="9e2c6-128">なし</span><span class="sxs-lookup"><span data-stu-id="9e2c6-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9e2c6-129">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="9e2c6-129">JSON Representation</span></span>
<span data-ttu-id="9e2c6-130">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="9e2c6-130">Here is a JSON representation of the resource.</span></span>
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





