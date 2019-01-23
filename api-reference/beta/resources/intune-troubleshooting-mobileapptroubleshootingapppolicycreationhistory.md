---
title: mobileAppTroubleshootingAppPolicyCreationHistory リソースの種類
description: 履歴項目は、モバイル アプリケーションのトラブルシューティング イベントに含まれています。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: e81f7f39cac934a89cf06d77fbcb80581267097b
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29394559"
---
# <a name="mobileapptroubleshootingapppolicycreationhistory-resource-type"></a><span data-ttu-id="8c6ba-103">mobileAppTroubleshootingAppPolicyCreationHistory リソースの種類</span><span class="sxs-lookup"><span data-stu-id="8c6ba-103">mobileAppTroubleshootingAppPolicyCreationHistory resource type</span></span>

> <span data-ttu-id="8c6ba-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="8c6ba-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="8c6ba-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8c6ba-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8c6ba-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="8c6ba-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8c6ba-107">履歴項目は、モバイル アプリケーションのトラブルシューティング イベントに含まれています。</span><span class="sxs-lookup"><span data-stu-id="8c6ba-107">History Item contained in the Mobile App Troubleshooting Event.</span></span>


<span data-ttu-id="8c6ba-108">[MobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="8c6ba-108">Inherits from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="8c6ba-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8c6ba-109">Properties</span></span>
|<span data-ttu-id="8c6ba-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8c6ba-110">Property</span></span>|<span data-ttu-id="8c6ba-111">型</span><span class="sxs-lookup"><span data-stu-id="8c6ba-111">Type</span></span>|<span data-ttu-id="8c6ba-112">説明</span><span class="sxs-lookup"><span data-stu-id="8c6ba-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8c6ba-113">occurrenceDateTime</span><span class="sxs-lookup"><span data-stu-id="8c6ba-113">occurrenceDateTime</span></span>|<span data-ttu-id="8c6ba-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8c6ba-114">DateTimeOffset</span></span>|<span data-ttu-id="8c6ba-115">履歴項目が発生した時刻です。</span><span class="sxs-lookup"><span data-stu-id="8c6ba-115">Time when the history item occurred.</span></span> <span data-ttu-id="8c6ba-116">[MobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="8c6ba-116">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|
|<span data-ttu-id="8c6ba-117">runState</span><span class="sxs-lookup"><span data-stu-id="8c6ba-117">runState</span></span>|[<span data-ttu-id="8c6ba-118">runState</span><span class="sxs-lookup"><span data-stu-id="8c6ba-118">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="8c6ba-119">項目の状態です。</span><span class="sxs-lookup"><span data-stu-id="8c6ba-119">Status of the item.</span></span> <span data-ttu-id="8c6ba-120">可能な値は、`unknown`、`success`、`fail` です。</span><span class="sxs-lookup"><span data-stu-id="8c6ba-120">Possible values are: `unknown`, `success`, `fail`.</span></span>|
|<span data-ttu-id="8c6ba-121">errorCode</span><span class="sxs-lookup"><span data-stu-id="8c6ba-121">errorCode</span></span>|<span data-ttu-id="8c6ba-122">String</span><span class="sxs-lookup"><span data-stu-id="8c6ba-122">String</span></span>|<span data-ttu-id="8c6ba-123">障害なしの場合は、空のエラーのエラー コードです。</span><span class="sxs-lookup"><span data-stu-id="8c6ba-123">Error code for the failure, empty if no failure.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8c6ba-124">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="8c6ba-124">Relationships</span></span>
<span data-ttu-id="8c6ba-125">なし</span><span class="sxs-lookup"><span data-stu-id="8c6ba-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8c6ba-126">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="8c6ba-126">JSON Representation</span></span>
<span data-ttu-id="8c6ba-127">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="8c6ba-127">Here is a JSON representation of the resource.</span></span>
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




