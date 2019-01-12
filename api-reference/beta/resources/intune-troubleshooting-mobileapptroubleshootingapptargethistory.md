---
title: mobileAppTroubleshootingAppTargetHistory リソースの種類
description: 履歴項目は、モバイル アプリケーションのトラブルシューティング イベントに含まれています。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 9da17e4a03d1a28c32215b8616dad2ea3700ef4f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27969423"
---
# <a name="mobileapptroubleshootingapptargethistory-resource-type"></a><span data-ttu-id="8fb03-103">mobileAppTroubleshootingAppTargetHistory リソースの種類</span><span class="sxs-lookup"><span data-stu-id="8fb03-103">mobileAppTroubleshootingAppTargetHistory resource type</span></span>

> <span data-ttu-id="8fb03-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="8fb03-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8fb03-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8fb03-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8fb03-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="8fb03-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8fb03-107">履歴項目は、モバイル アプリケーションのトラブルシューティング イベントに含まれています。</span><span class="sxs-lookup"><span data-stu-id="8fb03-107">History Item contained in the Mobile App Troubleshooting Event.</span></span>

<span data-ttu-id="8fb03-108">[MobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="8fb03-108">Inherits from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="8fb03-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8fb03-109">Properties</span></span>
|<span data-ttu-id="8fb03-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8fb03-110">Property</span></span>|<span data-ttu-id="8fb03-111">種類</span><span class="sxs-lookup"><span data-stu-id="8fb03-111">Type</span></span>|<span data-ttu-id="8fb03-112">説明</span><span class="sxs-lookup"><span data-stu-id="8fb03-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8fb03-113">occurrenceDateTime</span><span class="sxs-lookup"><span data-stu-id="8fb03-113">occurrenceDateTime</span></span>|<span data-ttu-id="8fb03-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8fb03-114">DateTimeOffset</span></span>|<span data-ttu-id="8fb03-115">履歴項目が発生した時刻です。</span><span class="sxs-lookup"><span data-stu-id="8fb03-115">Time when the history item occurred.</span></span> <span data-ttu-id="8fb03-116">[MobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="8fb03-116">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|
|<span data-ttu-id="8fb03-117">securityGroupId</span><span class="sxs-lookup"><span data-stu-id="8fb03-117">securityGroupId</span></span>|<span data-ttu-id="8fb03-118">String</span><span class="sxs-lookup"><span data-stu-id="8fb03-118">String</span></span>|<span data-ttu-id="8fb03-119">AAD セキュリティ グループの id が対象となります。</span><span class="sxs-lookup"><span data-stu-id="8fb03-119">AAD security group id to which it was targeted.</span></span>|
|<span data-ttu-id="8fb03-120">runState</span><span class="sxs-lookup"><span data-stu-id="8fb03-120">runState</span></span>|[<span data-ttu-id="8fb03-121">runState</span><span class="sxs-lookup"><span data-stu-id="8fb03-121">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="8fb03-122">項目の状態です。</span><span class="sxs-lookup"><span data-stu-id="8fb03-122">Status of the item.</span></span> <span data-ttu-id="8fb03-123">可能な値は、`unknown`、`success`、`fail` です。</span><span class="sxs-lookup"><span data-stu-id="8fb03-123">Possible values are: `unknown`, `success`, `fail`.</span></span>|
|<span data-ttu-id="8fb03-124">errorCode</span><span class="sxs-lookup"><span data-stu-id="8fb03-124">errorCode</span></span>|<span data-ttu-id="8fb03-125">String</span><span class="sxs-lookup"><span data-stu-id="8fb03-125">String</span></span>|<span data-ttu-id="8fb03-126">障害なしの場合は、空のエラーのエラー コードです。</span><span class="sxs-lookup"><span data-stu-id="8fb03-126">Error code for the failure, empty if no failure.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8fb03-127">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="8fb03-127">Relationships</span></span>
<span data-ttu-id="8fb03-128">なし</span><span class="sxs-lookup"><span data-stu-id="8fb03-128">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="8fb03-129">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="8fb03-129">JSON Representation</span></span>
<span data-ttu-id="8fb03-130">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="8fb03-130">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mobileAppTroubleshootingAppTargetHistory"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppTroubleshootingAppTargetHistory",
  "occurrenceDateTime": "String (timestamp)",
  "securityGroupId": "String",
  "runState": "String",
  "errorCode": "String"
}
```





