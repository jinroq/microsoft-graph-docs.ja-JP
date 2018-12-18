---
title: mobileAppTroubleshootingHistoryItem リソースの種類
description: 履歴項目は、モバイル アプリケーションのトラブルシューティング イベントに含まれています。
author: tfitzmac
ms.openlocfilehash: 132039a0b6e457ebd2ca3e545f6f15dd4ad7ac58
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27329527"
---
# <a name="mobileapptroubleshootinghistoryitem-resource-type"></a><span data-ttu-id="4ecc1-103">mobileAppTroubleshootingHistoryItem リソースの種類</span><span class="sxs-lookup"><span data-stu-id="4ecc1-103">mobileAppTroubleshootingHistoryItem resource type</span></span>

> <span data-ttu-id="4ecc1-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="4ecc1-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4ecc1-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4ecc1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4ecc1-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="4ecc1-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4ecc1-107">履歴項目は、モバイル アプリケーションのトラブルシューティング イベントに含まれています。</span><span class="sxs-lookup"><span data-stu-id="4ecc1-107">History Item contained in the Mobile App Troubleshooting Event.</span></span>
## <a name="properties"></a><span data-ttu-id="4ecc1-108">Properties</span><span class="sxs-lookup"><span data-stu-id="4ecc1-108">Properties</span></span>
|<span data-ttu-id="4ecc1-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4ecc1-109">Property</span></span>|<span data-ttu-id="4ecc1-110">種類</span><span class="sxs-lookup"><span data-stu-id="4ecc1-110">Type</span></span>|<span data-ttu-id="4ecc1-111">説明</span><span class="sxs-lookup"><span data-stu-id="4ecc1-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4ecc1-112">occurrenceDateTime</span><span class="sxs-lookup"><span data-stu-id="4ecc1-112">occurrenceDateTime</span></span>|<span data-ttu-id="4ecc1-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4ecc1-113">DateTimeOffset</span></span>|<span data-ttu-id="4ecc1-114">履歴項目が発生した時刻です。</span><span class="sxs-lookup"><span data-stu-id="4ecc1-114">Time when the history item occurred.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4ecc1-115">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="4ecc1-115">Relationships</span></span>
<span data-ttu-id="4ecc1-116">なし</span><span class="sxs-lookup"><span data-stu-id="4ecc1-116">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="4ecc1-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="4ecc1-117">JSON Representation</span></span>
<span data-ttu-id="4ecc1-118">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="4ecc1-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mobileAppTroubleshootingHistoryItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppTroubleshootingHistoryItem",
  "occurrenceDateTime": "String (timestamp)"
}
```





