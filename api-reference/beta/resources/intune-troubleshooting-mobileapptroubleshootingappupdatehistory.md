---
title: mobileAppTroubleshootingAppUpdateHistory リソースの種類
description: 履歴項目は、モバイル アプリケーションのトラブルシューティング イベントに含まれています。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 26ca343f761853bba05fa9905737b7fddf6ab3ec
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27870680"
---
# <a name="mobileapptroubleshootingappupdatehistory-resource-type"></a><span data-ttu-id="70895-103">mobileAppTroubleshootingAppUpdateHistory リソースの種類</span><span class="sxs-lookup"><span data-stu-id="70895-103">mobileAppTroubleshootingAppUpdateHistory resource type</span></span>

> <span data-ttu-id="70895-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="70895-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="70895-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="70895-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="70895-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="70895-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="70895-107">履歴項目は、モバイル アプリケーションのトラブルシューティング イベントに含まれています。</span><span class="sxs-lookup"><span data-stu-id="70895-107">History Item contained in the Mobile App Troubleshooting Event.</span></span>

<span data-ttu-id="70895-108">[MobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="70895-108">Inherits from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="70895-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="70895-109">Properties</span></span>
|<span data-ttu-id="70895-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="70895-110">Property</span></span>|<span data-ttu-id="70895-111">種類</span><span class="sxs-lookup"><span data-stu-id="70895-111">Type</span></span>|<span data-ttu-id="70895-112">説明</span><span class="sxs-lookup"><span data-stu-id="70895-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="70895-113">occurrenceDateTime</span><span class="sxs-lookup"><span data-stu-id="70895-113">occurrenceDateTime</span></span>|<span data-ttu-id="70895-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="70895-114">DateTimeOffset</span></span>|<span data-ttu-id="70895-115">履歴項目が発生した時刻です。</span><span class="sxs-lookup"><span data-stu-id="70895-115">Time when the history item occurred.</span></span> <span data-ttu-id="70895-116">[MobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="70895-116">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="70895-117">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="70895-117">Relationships</span></span>
<span data-ttu-id="70895-118">なし</span><span class="sxs-lookup"><span data-stu-id="70895-118">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="70895-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="70895-119">JSON Representation</span></span>
<span data-ttu-id="70895-120">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="70895-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mobileAppTroubleshootingAppUpdateHistory"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppTroubleshootingAppUpdateHistory",
  "occurrenceDateTime": "String (timestamp)"
}
```





