---
title: mobileAppTroubleshootingHistoryItem リソースの種類
description: 履歴項目は、モバイル アプリケーションのトラブルシューティング イベントに含まれています。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 28245267a7c05f03bedd21c8dc0de17198de213c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29400068"
---
# <a name="mobileapptroubleshootinghistoryitem-resource-type"></a><span data-ttu-id="22f36-103">mobileAppTroubleshootingHistoryItem リソースの種類</span><span class="sxs-lookup"><span data-stu-id="22f36-103">mobileAppTroubleshootingHistoryItem resource type</span></span>

> <span data-ttu-id="22f36-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="22f36-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="22f36-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="22f36-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="22f36-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="22f36-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="22f36-107">履歴項目は、モバイル アプリケーションのトラブルシューティング イベントに含まれています。</span><span class="sxs-lookup"><span data-stu-id="22f36-107">History Item contained in the Mobile App Troubleshooting Event.</span></span>

## <a name="properties"></a><span data-ttu-id="22f36-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="22f36-108">Properties</span></span>
|<span data-ttu-id="22f36-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="22f36-109">Property</span></span>|<span data-ttu-id="22f36-110">型</span><span class="sxs-lookup"><span data-stu-id="22f36-110">Type</span></span>|<span data-ttu-id="22f36-111">説明</span><span class="sxs-lookup"><span data-stu-id="22f36-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="22f36-112">occurrenceDateTime</span><span class="sxs-lookup"><span data-stu-id="22f36-112">occurrenceDateTime</span></span>|<span data-ttu-id="22f36-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="22f36-113">DateTimeOffset</span></span>|<span data-ttu-id="22f36-114">履歴項目が発生した時刻です。</span><span class="sxs-lookup"><span data-stu-id="22f36-114">Time when the history item occurred.</span></span>|

## <a name="relationships"></a><span data-ttu-id="22f36-115">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="22f36-115">Relationships</span></span>
<span data-ttu-id="22f36-116">なし</span><span class="sxs-lookup"><span data-stu-id="22f36-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="22f36-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="22f36-117">JSON Representation</span></span>
<span data-ttu-id="22f36-118">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="22f36-118">Here is a JSON representation of the resource.</span></span>
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




