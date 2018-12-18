---
title: mobileAppTroubleshootingAppTargetHistory リソースの種類
description: 履歴項目は、モバイル アプリケーションのトラブルシューティング イベントに含まれています。
author: tfitzmac
ms.openlocfilehash: cdb901d4c532b57025837a2fb0cc0975ceba3f8c
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27312734"
---
# <a name="mobileapptroubleshootingapptargethistory-resource-type"></a><span data-ttu-id="ff147-103">mobileAppTroubleshootingAppTargetHistory リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ff147-103">mobileAppTroubleshootingAppTargetHistory resource type</span></span>

> <span data-ttu-id="ff147-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="ff147-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ff147-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ff147-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ff147-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="ff147-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ff147-107">履歴項目は、モバイル アプリケーションのトラブルシューティング イベントに含まれています。</span><span class="sxs-lookup"><span data-stu-id="ff147-107">History Item contained in the Mobile App Troubleshooting Event.</span></span>

<span data-ttu-id="ff147-108">[MobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="ff147-108">Inherits from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="ff147-109">Properties</span><span class="sxs-lookup"><span data-stu-id="ff147-109">Properties</span></span>
|<span data-ttu-id="ff147-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ff147-110">Property</span></span>|<span data-ttu-id="ff147-111">種類</span><span class="sxs-lookup"><span data-stu-id="ff147-111">Type</span></span>|<span data-ttu-id="ff147-112">説明</span><span class="sxs-lookup"><span data-stu-id="ff147-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ff147-113">occurrenceDateTime</span><span class="sxs-lookup"><span data-stu-id="ff147-113">occurrenceDateTime</span></span>|<span data-ttu-id="ff147-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ff147-114">DateTimeOffset</span></span>|<span data-ttu-id="ff147-115">履歴項目が発生した時刻です。</span><span class="sxs-lookup"><span data-stu-id="ff147-115">Time when the history item occurred.</span></span> <span data-ttu-id="ff147-116">[MobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="ff147-116">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|
|<span data-ttu-id="ff147-117">securityGroupId</span><span class="sxs-lookup"><span data-stu-id="ff147-117">securityGroupId</span></span>|<span data-ttu-id="ff147-118">String</span><span class="sxs-lookup"><span data-stu-id="ff147-118">String</span></span>|<span data-ttu-id="ff147-119">AAD セキュリティ グループの id が対象となります。</span><span class="sxs-lookup"><span data-stu-id="ff147-119">AAD security group id to which it was targeted.</span></span>|
|<span data-ttu-id="ff147-120">runState</span><span class="sxs-lookup"><span data-stu-id="ff147-120">runState</span></span>|[<span data-ttu-id="ff147-121">runState</span><span class="sxs-lookup"><span data-stu-id="ff147-121">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="ff147-122">項目の状態です。</span><span class="sxs-lookup"><span data-stu-id="ff147-122">Status of the item.</span></span> <span data-ttu-id="ff147-123">可能な値は、`unknown`、`success`、`fail` です。</span><span class="sxs-lookup"><span data-stu-id="ff147-123">Possible values are: `unknown`, `success`, `fail`.</span></span>|
|<span data-ttu-id="ff147-124">errorCode</span><span class="sxs-lookup"><span data-stu-id="ff147-124">errorCode</span></span>|<span data-ttu-id="ff147-125">String</span><span class="sxs-lookup"><span data-stu-id="ff147-125">String</span></span>|<span data-ttu-id="ff147-126">障害なしの場合は、空のエラーのエラー コードです。</span><span class="sxs-lookup"><span data-stu-id="ff147-126">Error code for the failure, empty if no failure.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ff147-127">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="ff147-127">Relationships</span></span>
<span data-ttu-id="ff147-128">なし</span><span class="sxs-lookup"><span data-stu-id="ff147-128">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="ff147-129">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ff147-129">JSON Representation</span></span>
<span data-ttu-id="ff147-130">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="ff147-130">Here is a JSON representation of the resource.</span></span>
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





