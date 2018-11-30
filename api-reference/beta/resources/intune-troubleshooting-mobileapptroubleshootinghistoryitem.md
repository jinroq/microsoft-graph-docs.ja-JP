---
title: mobileAppTroubleshootingHistoryItem リソースの種類
description: 履歴項目は、モバイル アプリケーションのトラブルシューティング イベントに含まれています。
ms.openlocfilehash: 8fdeb522cd714f9265bc9f453fb5381bd925c481
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27071905"
---
# <a name="mobileapptroubleshootinghistoryitem-resource-type"></a><span data-ttu-id="530fa-103">mobileAppTroubleshootingHistoryItem リソースの種類</span><span class="sxs-lookup"><span data-stu-id="530fa-103">mobileAppTroubleshootingHistoryItem resource type</span></span>

> <span data-ttu-id="530fa-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="530fa-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="530fa-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="530fa-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="530fa-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="530fa-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="530fa-107">履歴項目は、モバイル アプリケーションのトラブルシューティング イベントに含まれています。</span><span class="sxs-lookup"><span data-stu-id="530fa-107">History Item contained in the Mobile App Troubleshooting Event.</span></span>
## <a name="properties"></a><span data-ttu-id="530fa-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="530fa-108">Properties</span></span>
|<span data-ttu-id="530fa-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="530fa-109">Property</span></span>|<span data-ttu-id="530fa-110">型</span><span class="sxs-lookup"><span data-stu-id="530fa-110">Type</span></span>|<span data-ttu-id="530fa-111">説明</span><span class="sxs-lookup"><span data-stu-id="530fa-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="530fa-112">occurrenceDateTime</span><span class="sxs-lookup"><span data-stu-id="530fa-112">occurrenceDateTime</span></span>|<span data-ttu-id="530fa-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="530fa-113">DateTimeOffset</span></span>|<span data-ttu-id="530fa-114">履歴項目が発生した時刻です。</span><span class="sxs-lookup"><span data-stu-id="530fa-114">Time when the history item occurred.</span></span>|

## <a name="relationships"></a><span data-ttu-id="530fa-115">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="530fa-115">Relationships</span></span>
<span data-ttu-id="530fa-116">なし</span><span class="sxs-lookup"><span data-stu-id="530fa-116">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="530fa-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="530fa-117">JSON Representation</span></span>
<span data-ttu-id="530fa-118">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="530fa-118">Here is a JSON representation of the resource.</span></span>
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





