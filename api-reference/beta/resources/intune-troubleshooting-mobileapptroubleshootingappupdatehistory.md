---
title: mobileAppTroubleshootingAppUpdateHistory リソースの種類
description: 履歴項目は、モバイル アプリケーションのトラブルシューティング イベントに含まれています。
ms.openlocfilehash: d546475f568c279137e411d546765fe828c43975
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27070905"
---
# <a name="mobileapptroubleshootingappupdatehistory-resource-type"></a><span data-ttu-id="2365d-103">mobileAppTroubleshootingAppUpdateHistory リソースの種類</span><span class="sxs-lookup"><span data-stu-id="2365d-103">mobileAppTroubleshootingAppUpdateHistory resource type</span></span>

> <span data-ttu-id="2365d-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="2365d-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2365d-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2365d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2365d-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="2365d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2365d-107">履歴項目は、モバイル アプリケーションのトラブルシューティング イベントに含まれています。</span><span class="sxs-lookup"><span data-stu-id="2365d-107">History Item contained in the Mobile App Troubleshooting Event.</span></span>

<span data-ttu-id="2365d-108">[MobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="2365d-108">Inherits from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="2365d-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2365d-109">Properties</span></span>
|<span data-ttu-id="2365d-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2365d-110">Property</span></span>|<span data-ttu-id="2365d-111">型</span><span class="sxs-lookup"><span data-stu-id="2365d-111">Type</span></span>|<span data-ttu-id="2365d-112">説明</span><span class="sxs-lookup"><span data-stu-id="2365d-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2365d-113">occurrenceDateTime</span><span class="sxs-lookup"><span data-stu-id="2365d-113">occurrenceDateTime</span></span>|<span data-ttu-id="2365d-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2365d-114">DateTimeOffset</span></span>|<span data-ttu-id="2365d-115">履歴項目が発生した時刻です。</span><span class="sxs-lookup"><span data-stu-id="2365d-115">Time when the history item occurred.</span></span> <span data-ttu-id="2365d-116">[MobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="2365d-116">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="2365d-117">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="2365d-117">Relationships</span></span>
<span data-ttu-id="2365d-118">なし</span><span class="sxs-lookup"><span data-stu-id="2365d-118">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="2365d-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="2365d-119">JSON Representation</span></span>
<span data-ttu-id="2365d-120">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="2365d-120">Here is a JSON representation of the resource.</span></span>
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





