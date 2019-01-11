---
title: mobileAppTroubleshootingDeviceCheckinHistory リソースの種類
description: 履歴項目は、モバイル アプリケーションのトラブルシューティング イベントに含まれています。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 6b9d900e712e3c3b126dd36671049e8935f09a83
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27844948"
---
# <a name="mobileapptroubleshootingdevicecheckinhistory-resource-type"></a><span data-ttu-id="06852-103">mobileAppTroubleshootingDeviceCheckinHistory リソースの種類</span><span class="sxs-lookup"><span data-stu-id="06852-103">mobileAppTroubleshootingDeviceCheckinHistory resource type</span></span>

> <span data-ttu-id="06852-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="06852-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="06852-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="06852-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="06852-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="06852-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="06852-107">履歴項目は、モバイル アプリケーションのトラブルシューティング イベントに含まれています。</span><span class="sxs-lookup"><span data-stu-id="06852-107">History Item contained in the Mobile App Troubleshooting Event.</span></span>

<span data-ttu-id="06852-108">[MobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="06852-108">Inherits from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="06852-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="06852-109">Properties</span></span>
|<span data-ttu-id="06852-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="06852-110">Property</span></span>|<span data-ttu-id="06852-111">種類</span><span class="sxs-lookup"><span data-stu-id="06852-111">Type</span></span>|<span data-ttu-id="06852-112">説明</span><span class="sxs-lookup"><span data-stu-id="06852-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="06852-113">occurrenceDateTime</span><span class="sxs-lookup"><span data-stu-id="06852-113">occurrenceDateTime</span></span>|<span data-ttu-id="06852-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="06852-114">DateTimeOffset</span></span>|<span data-ttu-id="06852-115">履歴項目が発生した時刻です。</span><span class="sxs-lookup"><span data-stu-id="06852-115">Time when the history item occurred.</span></span> <span data-ttu-id="06852-116">[MobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="06852-116">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="06852-117">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="06852-117">Relationships</span></span>
<span data-ttu-id="06852-118">なし</span><span class="sxs-lookup"><span data-stu-id="06852-118">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="06852-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="06852-119">JSON Representation</span></span>
<span data-ttu-id="06852-120">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="06852-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mobileAppTroubleshootingDeviceCheckinHistory"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppTroubleshootingDeviceCheckinHistory",
  "occurrenceDateTime": "String (timestamp)"
}
```





