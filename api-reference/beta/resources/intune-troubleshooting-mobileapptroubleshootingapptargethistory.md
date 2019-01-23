---
title: mobileAppTroubleshootingAppTargetHistory リソースの種類
description: 履歴項目は、モバイル アプリケーションのトラブルシューティング イベントに含まれています。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: c0a1d37f86ebb43b7d697a9407ce0e3a479b2350
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29402966"
---
# <a name="mobileapptroubleshootingapptargethistory-resource-type"></a><span data-ttu-id="25b40-103">mobileAppTroubleshootingAppTargetHistory リソースの種類</span><span class="sxs-lookup"><span data-stu-id="25b40-103">mobileAppTroubleshootingAppTargetHistory resource type</span></span>

> <span data-ttu-id="25b40-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="25b40-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="25b40-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="25b40-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="25b40-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="25b40-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="25b40-107">履歴項目は、モバイル アプリケーションのトラブルシューティング イベントに含まれています。</span><span class="sxs-lookup"><span data-stu-id="25b40-107">History Item contained in the Mobile App Troubleshooting Event.</span></span>


<span data-ttu-id="25b40-108">[MobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="25b40-108">Inherits from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="25b40-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="25b40-109">Properties</span></span>
|<span data-ttu-id="25b40-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="25b40-110">Property</span></span>|<span data-ttu-id="25b40-111">型</span><span class="sxs-lookup"><span data-stu-id="25b40-111">Type</span></span>|<span data-ttu-id="25b40-112">説明</span><span class="sxs-lookup"><span data-stu-id="25b40-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="25b40-113">occurrenceDateTime</span><span class="sxs-lookup"><span data-stu-id="25b40-113">occurrenceDateTime</span></span>|<span data-ttu-id="25b40-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="25b40-114">DateTimeOffset</span></span>|<span data-ttu-id="25b40-115">履歴項目が発生した時刻です。</span><span class="sxs-lookup"><span data-stu-id="25b40-115">Time when the history item occurred.</span></span> <span data-ttu-id="25b40-116">[MobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="25b40-116">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|
|<span data-ttu-id="25b40-117">securityGroupId</span><span class="sxs-lookup"><span data-stu-id="25b40-117">securityGroupId</span></span>|<span data-ttu-id="25b40-118">String</span><span class="sxs-lookup"><span data-stu-id="25b40-118">String</span></span>|<span data-ttu-id="25b40-119">AAD セキュリティ グループの id が対象となります。</span><span class="sxs-lookup"><span data-stu-id="25b40-119">AAD security group id to which it was targeted.</span></span>|
|<span data-ttu-id="25b40-120">runState</span><span class="sxs-lookup"><span data-stu-id="25b40-120">runState</span></span>|[<span data-ttu-id="25b40-121">runState</span><span class="sxs-lookup"><span data-stu-id="25b40-121">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="25b40-122">項目の状態です。</span><span class="sxs-lookup"><span data-stu-id="25b40-122">Status of the item.</span></span> <span data-ttu-id="25b40-123">可能な値は、`unknown`、`success`、`fail` です。</span><span class="sxs-lookup"><span data-stu-id="25b40-123">Possible values are: `unknown`, `success`, `fail`.</span></span>|
|<span data-ttu-id="25b40-124">errorCode</span><span class="sxs-lookup"><span data-stu-id="25b40-124">errorCode</span></span>|<span data-ttu-id="25b40-125">String</span><span class="sxs-lookup"><span data-stu-id="25b40-125">String</span></span>|<span data-ttu-id="25b40-126">障害なしの場合は、空のエラーのエラー コードです。</span><span class="sxs-lookup"><span data-stu-id="25b40-126">Error code for the failure, empty if no failure.</span></span>|

## <a name="relationships"></a><span data-ttu-id="25b40-127">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="25b40-127">Relationships</span></span>
<span data-ttu-id="25b40-128">なし</span><span class="sxs-lookup"><span data-stu-id="25b40-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="25b40-129">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="25b40-129">JSON Representation</span></span>
<span data-ttu-id="25b40-130">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="25b40-130">Here is a JSON representation of the resource.</span></span>
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




