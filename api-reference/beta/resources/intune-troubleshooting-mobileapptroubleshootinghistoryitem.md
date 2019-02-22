---
title: mobileAppTroubleshootingHistoryItem リソースの種類
description: モバイルアプリのトラブルシューティングイベントに含まれる履歴アイテム。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fbc37488f478c47b0b097c4fd8a54b09273bc5c3
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30160859"
---
# <a name="mobileapptroubleshootinghistoryitem-resource-type"></a><span data-ttu-id="bf2d2-103">mobileAppTroubleshootingHistoryItem リソースの種類</span><span class="sxs-lookup"><span data-stu-id="bf2d2-103">mobileAppTroubleshootingHistoryItem resource type</span></span>

> <span data-ttu-id="bf2d2-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bf2d2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bf2d2-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="bf2d2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bf2d2-106">モバイルアプリのトラブルシューティングイベントに含まれる履歴アイテム。</span><span class="sxs-lookup"><span data-stu-id="bf2d2-106">History Item contained in the Mobile App Troubleshooting Event.</span></span>

## <a name="properties"></a><span data-ttu-id="bf2d2-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bf2d2-107">Properties</span></span>
|<span data-ttu-id="bf2d2-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bf2d2-108">Property</span></span>|<span data-ttu-id="bf2d2-109">型</span><span class="sxs-lookup"><span data-stu-id="bf2d2-109">Type</span></span>|<span data-ttu-id="bf2d2-110">説明</span><span class="sxs-lookup"><span data-stu-id="bf2d2-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bf2d2-111">occurrenceDateTime</span><span class="sxs-lookup"><span data-stu-id="bf2d2-111">occurrenceDateTime</span></span>|<span data-ttu-id="bf2d2-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bf2d2-112">DateTimeOffset</span></span>|<span data-ttu-id="bf2d2-113">履歴アイテムが発生した時刻。</span><span class="sxs-lookup"><span data-stu-id="bf2d2-113">Time when the history item occurred.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bf2d2-114">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="bf2d2-114">Relationships</span></span>
<span data-ttu-id="bf2d2-115">なし</span><span class="sxs-lookup"><span data-stu-id="bf2d2-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bf2d2-116">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="bf2d2-116">JSON Representation</span></span>
<span data-ttu-id="bf2d2-117">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="bf2d2-117">Here is a JSON representation of the resource.</span></span>
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




