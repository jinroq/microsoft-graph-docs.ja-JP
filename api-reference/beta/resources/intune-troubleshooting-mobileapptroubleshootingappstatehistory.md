---
title: mobileAppTroubleshootingAppStateHistory リソースの種類
description: 履歴項目は、モバイル アプリケーションのトラブルシューティング イベントに含まれています。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 65ee72ed0c265f2e989e82dfdcc28d27605d4753
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27885569"
---
# <a name="mobileapptroubleshootingappstatehistory-resource-type"></a><span data-ttu-id="cd529-103">mobileAppTroubleshootingAppStateHistory リソースの種類</span><span class="sxs-lookup"><span data-stu-id="cd529-103">mobileAppTroubleshootingAppStateHistory resource type</span></span>

> <span data-ttu-id="cd529-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="cd529-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cd529-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cd529-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="cd529-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="cd529-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cd529-107">履歴項目は、モバイル アプリケーションのトラブルシューティング イベントに含まれています。</span><span class="sxs-lookup"><span data-stu-id="cd529-107">History Item contained in the Mobile App Troubleshooting Event.</span></span>

<span data-ttu-id="cd529-108">[MobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="cd529-108">Inherits from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="cd529-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cd529-109">Properties</span></span>
|<span data-ttu-id="cd529-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cd529-110">Property</span></span>|<span data-ttu-id="cd529-111">種類</span><span class="sxs-lookup"><span data-stu-id="cd529-111">Type</span></span>|<span data-ttu-id="cd529-112">説明</span><span class="sxs-lookup"><span data-stu-id="cd529-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cd529-113">occurrenceDateTime</span><span class="sxs-lookup"><span data-stu-id="cd529-113">occurrenceDateTime</span></span>|<span data-ttu-id="cd529-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cd529-114">DateTimeOffset</span></span>|<span data-ttu-id="cd529-115">履歴項目が発生した時刻です。</span><span class="sxs-lookup"><span data-stu-id="cd529-115">Time when the history item occurred.</span></span> <span data-ttu-id="cd529-116">[MobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="cd529-116">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|
|<span data-ttu-id="cd529-117">actionType</span><span class="sxs-lookup"><span data-stu-id="cd529-117">actionType</span></span>|[<span data-ttu-id="cd529-118">mobileAppActionType</span><span class="sxs-lookup"><span data-stu-id="cd529-118">mobileAppActionType</span></span>](../resources/intune-troubleshooting-mobileappactiontype.md)|<span data-ttu-id="cd529-119">AAD セキュリティ グループの id が対象となります。</span><span class="sxs-lookup"><span data-stu-id="cd529-119">AAD security group id to which it was targeted.</span></span> <span data-ttu-id="cd529-120">可能な値は、`unknown`、`installCommandSent`、`installed`、`uninstalled`、`userRequestedInstall` です。</span><span class="sxs-lookup"><span data-stu-id="cd529-120">Possible values are: `unknown`, `installCommandSent`, `installed`, `uninstalled`, `userRequestedInstall`.</span></span>|
|<span data-ttu-id="cd529-121">runState</span><span class="sxs-lookup"><span data-stu-id="cd529-121">runState</span></span>|[<span data-ttu-id="cd529-122">runState</span><span class="sxs-lookup"><span data-stu-id="cd529-122">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="cd529-123">項目の状態です。</span><span class="sxs-lookup"><span data-stu-id="cd529-123">Status of the item.</span></span> <span data-ttu-id="cd529-124">可能な値は、`unknown`、`success`、`fail` です。</span><span class="sxs-lookup"><span data-stu-id="cd529-124">Possible values are: `unknown`, `success`, `fail`.</span></span>|
|<span data-ttu-id="cd529-125">errorCode</span><span class="sxs-lookup"><span data-stu-id="cd529-125">errorCode</span></span>|<span data-ttu-id="cd529-126">String</span><span class="sxs-lookup"><span data-stu-id="cd529-126">String</span></span>|<span data-ttu-id="cd529-127">障害なしの場合は、空のエラーのエラー コードです。</span><span class="sxs-lookup"><span data-stu-id="cd529-127">Error code for the failure, empty if no failure.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cd529-128">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="cd529-128">Relationships</span></span>
<span data-ttu-id="cd529-129">なし</span><span class="sxs-lookup"><span data-stu-id="cd529-129">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="cd529-130">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="cd529-130">JSON Representation</span></span>
<span data-ttu-id="cd529-131">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="cd529-131">Here is a JSON representation of the resource.</span></span>
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





