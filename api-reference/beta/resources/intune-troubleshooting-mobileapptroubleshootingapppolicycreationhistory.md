---
title: mobileAppTroubleshootingAppPolicyCreationHistory リソースの種類
description: 履歴項目は、モバイル アプリケーションのトラブルシューティング イベントに含まれています。
ms.openlocfilehash: 7ca80443351e5c1b1232dc050cdf721ab7389351
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27072797"
---
# <a name="mobileapptroubleshootingapppolicycreationhistory-resource-type"></a><span data-ttu-id="fcfe8-103">mobileAppTroubleshootingAppPolicyCreationHistory リソースの種類</span><span class="sxs-lookup"><span data-stu-id="fcfe8-103">mobileAppTroubleshootingAppPolicyCreationHistory resource type</span></span>

> <span data-ttu-id="fcfe8-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="fcfe8-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fcfe8-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fcfe8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fcfe8-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="fcfe8-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fcfe8-107">履歴項目は、モバイル アプリケーションのトラブルシューティング イベントに含まれています。</span><span class="sxs-lookup"><span data-stu-id="fcfe8-107">History Item contained in the Mobile App Troubleshooting Event.</span></span>

<span data-ttu-id="fcfe8-108">[MobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="fcfe8-108">Inherits from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="fcfe8-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fcfe8-109">Properties</span></span>
|<span data-ttu-id="fcfe8-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fcfe8-110">Property</span></span>|<span data-ttu-id="fcfe8-111">型</span><span class="sxs-lookup"><span data-stu-id="fcfe8-111">Type</span></span>|<span data-ttu-id="fcfe8-112">説明</span><span class="sxs-lookup"><span data-stu-id="fcfe8-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fcfe8-113">occurrenceDateTime</span><span class="sxs-lookup"><span data-stu-id="fcfe8-113">occurrenceDateTime</span></span>|<span data-ttu-id="fcfe8-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fcfe8-114">DateTimeOffset</span></span>|<span data-ttu-id="fcfe8-115">履歴項目が発生した時刻です。</span><span class="sxs-lookup"><span data-stu-id="fcfe8-115">Time when the history item occurred.</span></span> <span data-ttu-id="fcfe8-116">[MobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="fcfe8-116">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|
|<span data-ttu-id="fcfe8-117">runState</span><span class="sxs-lookup"><span data-stu-id="fcfe8-117">runState</span></span>|[<span data-ttu-id="fcfe8-118">runState</span><span class="sxs-lookup"><span data-stu-id="fcfe8-118">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="fcfe8-119">項目の状態です。</span><span class="sxs-lookup"><span data-stu-id="fcfe8-119">Status of the item.</span></span> <span data-ttu-id="fcfe8-120">可能な値は、`unknown`、`success`、`fail` です。</span><span class="sxs-lookup"><span data-stu-id="fcfe8-120">Possible values are: `unknown`, `success`, `fail`.</span></span>|
|<span data-ttu-id="fcfe8-121">errorCode</span><span class="sxs-lookup"><span data-stu-id="fcfe8-121">errorCode</span></span>|<span data-ttu-id="fcfe8-122">String</span><span class="sxs-lookup"><span data-stu-id="fcfe8-122">String</span></span>|<span data-ttu-id="fcfe8-123">障害なしの場合は、空のエラーのエラー コードです。</span><span class="sxs-lookup"><span data-stu-id="fcfe8-123">Error code for the failure, empty if no failure.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fcfe8-124">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="fcfe8-124">Relationships</span></span>
<span data-ttu-id="fcfe8-125">なし</span><span class="sxs-lookup"><span data-stu-id="fcfe8-125">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="fcfe8-126">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="fcfe8-126">JSON Representation</span></span>
<span data-ttu-id="fcfe8-127">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="fcfe8-127">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mobileAppTroubleshootingAppPolicyCreationHistory"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppTroubleshootingAppPolicyCreationHistory",
  "occurrenceDateTime": "String (timestamp)",
  "runState": "String",
  "errorCode": "String"
}
```





