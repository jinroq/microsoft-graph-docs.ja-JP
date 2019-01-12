---
title: mobileAppTroubleshootingAppStateHistory リソースの種類
description: 履歴項目は、モバイル アプリケーションのトラブルシューティング イベントに含まれています。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 03a7cd7a67790dca8824b7e446b5add5304c6f0a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27917742"
---
# <a name="mobileapptroubleshootingappstatehistory-resource-type"></a><span data-ttu-id="c805a-103">mobileAppTroubleshootingAppStateHistory リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c805a-103">mobileAppTroubleshootingAppStateHistory resource type</span></span>

> <span data-ttu-id="c805a-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="c805a-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c805a-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c805a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c805a-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="c805a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c805a-107">履歴項目は、モバイル アプリケーションのトラブルシューティング イベントに含まれています。</span><span class="sxs-lookup"><span data-stu-id="c805a-107">History Item contained in the Mobile App Troubleshooting Event.</span></span>

<span data-ttu-id="c805a-108">[MobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="c805a-108">Inherits from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c805a-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c805a-109">Properties</span></span>
|<span data-ttu-id="c805a-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c805a-110">Property</span></span>|<span data-ttu-id="c805a-111">種類</span><span class="sxs-lookup"><span data-stu-id="c805a-111">Type</span></span>|<span data-ttu-id="c805a-112">説明</span><span class="sxs-lookup"><span data-stu-id="c805a-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c805a-113">occurrenceDateTime</span><span class="sxs-lookup"><span data-stu-id="c805a-113">occurrenceDateTime</span></span>|<span data-ttu-id="c805a-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c805a-114">DateTimeOffset</span></span>|<span data-ttu-id="c805a-115">履歴項目が発生した時刻です。</span><span class="sxs-lookup"><span data-stu-id="c805a-115">Time when the history item occurred.</span></span> <span data-ttu-id="c805a-116">[MobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="c805a-116">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|
|<span data-ttu-id="c805a-117">actionType</span><span class="sxs-lookup"><span data-stu-id="c805a-117">actionType</span></span>|[<span data-ttu-id="c805a-118">mobileAppActionType</span><span class="sxs-lookup"><span data-stu-id="c805a-118">mobileAppActionType</span></span>](../resources/intune-troubleshooting-mobileappactiontype.md)|<span data-ttu-id="c805a-119">AAD セキュリティ グループの id が対象となります。</span><span class="sxs-lookup"><span data-stu-id="c805a-119">AAD security group id to which it was targeted.</span></span> <span data-ttu-id="c805a-120">可能な値は、`unknown`、`installCommandSent`、`installed`、`uninstalled`、`userRequestedInstall` です。</span><span class="sxs-lookup"><span data-stu-id="c805a-120">Possible values are: `unknown`, `installCommandSent`, `installed`, `uninstalled`, `userRequestedInstall`.</span></span>|
|<span data-ttu-id="c805a-121">runState</span><span class="sxs-lookup"><span data-stu-id="c805a-121">runState</span></span>|[<span data-ttu-id="c805a-122">runState</span><span class="sxs-lookup"><span data-stu-id="c805a-122">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="c805a-123">項目の状態です。</span><span class="sxs-lookup"><span data-stu-id="c805a-123">Status of the item.</span></span> <span data-ttu-id="c805a-124">可能な値は、`unknown`、`success`、`fail` です。</span><span class="sxs-lookup"><span data-stu-id="c805a-124">Possible values are: `unknown`, `success`, `fail`.</span></span>|
|<span data-ttu-id="c805a-125">errorCode</span><span class="sxs-lookup"><span data-stu-id="c805a-125">errorCode</span></span>|<span data-ttu-id="c805a-126">String</span><span class="sxs-lookup"><span data-stu-id="c805a-126">String</span></span>|<span data-ttu-id="c805a-127">障害なしの場合は、空のエラーのエラー コードです。</span><span class="sxs-lookup"><span data-stu-id="c805a-127">Error code for the failure, empty if no failure.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c805a-128">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="c805a-128">Relationships</span></span>
<span data-ttu-id="c805a-129">なし</span><span class="sxs-lookup"><span data-stu-id="c805a-129">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="c805a-130">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c805a-130">JSON Representation</span></span>
<span data-ttu-id="c805a-131">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="c805a-131">Here is a JSON representation of the resource.</span></span>
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





