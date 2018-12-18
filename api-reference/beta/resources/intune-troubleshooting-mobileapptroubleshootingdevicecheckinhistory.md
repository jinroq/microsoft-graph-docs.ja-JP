---
title: mobileAppTroubleshootingDeviceCheckinHistory リソースの種類
description: 履歴項目は、モバイル アプリケーションのトラブルシューティング イベントに含まれています。
author: tfitzmac
ms.openlocfilehash: aadaf94a2b021e6207a1639ec215445d602b4c3f
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27312937"
---
# <a name="mobileapptroubleshootingdevicecheckinhistory-resource-type"></a><span data-ttu-id="dc21f-103">mobileAppTroubleshootingDeviceCheckinHistory リソースの種類</span><span class="sxs-lookup"><span data-stu-id="dc21f-103">mobileAppTroubleshootingDeviceCheckinHistory resource type</span></span>

> <span data-ttu-id="dc21f-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="dc21f-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="dc21f-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="dc21f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="dc21f-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="dc21f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="dc21f-107">履歴項目は、モバイル アプリケーションのトラブルシューティング イベントに含まれています。</span><span class="sxs-lookup"><span data-stu-id="dc21f-107">History Item contained in the Mobile App Troubleshooting Event.</span></span>

<span data-ttu-id="dc21f-108">[MobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="dc21f-108">Inherits from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="dc21f-109">Properties</span><span class="sxs-lookup"><span data-stu-id="dc21f-109">Properties</span></span>
|<span data-ttu-id="dc21f-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="dc21f-110">Property</span></span>|<span data-ttu-id="dc21f-111">種類</span><span class="sxs-lookup"><span data-stu-id="dc21f-111">Type</span></span>|<span data-ttu-id="dc21f-112">説明</span><span class="sxs-lookup"><span data-stu-id="dc21f-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dc21f-113">occurrenceDateTime</span><span class="sxs-lookup"><span data-stu-id="dc21f-113">occurrenceDateTime</span></span>|<span data-ttu-id="dc21f-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dc21f-114">DateTimeOffset</span></span>|<span data-ttu-id="dc21f-115">履歴項目が発生した時刻です。</span><span class="sxs-lookup"><span data-stu-id="dc21f-115">Time when the history item occurred.</span></span> <span data-ttu-id="dc21f-116">[MobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="dc21f-116">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="dc21f-117">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="dc21f-117">Relationships</span></span>
<span data-ttu-id="dc21f-118">なし</span><span class="sxs-lookup"><span data-stu-id="dc21f-118">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="dc21f-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="dc21f-119">JSON Representation</span></span>
<span data-ttu-id="dc21f-120">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="dc21f-120">Here is a JSON representation of the resource.</span></span>
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





