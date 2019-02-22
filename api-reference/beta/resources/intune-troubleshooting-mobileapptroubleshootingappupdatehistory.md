---
title: mobileAppTroubleshootingAppUpdateHistory リソースの種類
description: モバイルアプリのトラブルシューティングイベントに含まれる履歴アイテム。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3eadbec77e95dd90fd9ef819e468241bf8ef5c9e
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30153642"
---
# <a name="mobileapptroubleshootingappupdatehistory-resource-type"></a><span data-ttu-id="9efad-103">mobileAppTroubleshootingAppUpdateHistory リソースの種類</span><span class="sxs-lookup"><span data-stu-id="9efad-103">mobileAppTroubleshootingAppUpdateHistory resource type</span></span>

> <span data-ttu-id="9efad-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9efad-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9efad-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="9efad-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9efad-106">モバイルアプリのトラブルシューティングイベントに含まれる履歴アイテム。</span><span class="sxs-lookup"><span data-stu-id="9efad-106">History Item contained in the Mobile App Troubleshooting Event.</span></span>


<span data-ttu-id="9efad-107">[mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="9efad-107">Inherits from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="9efad-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9efad-108">Properties</span></span>
|<span data-ttu-id="9efad-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9efad-109">Property</span></span>|<span data-ttu-id="9efad-110">型</span><span class="sxs-lookup"><span data-stu-id="9efad-110">Type</span></span>|<span data-ttu-id="9efad-111">説明</span><span class="sxs-lookup"><span data-stu-id="9efad-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9efad-112">occurrenceDateTime</span><span class="sxs-lookup"><span data-stu-id="9efad-112">occurrenceDateTime</span></span>|<span data-ttu-id="9efad-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9efad-113">DateTimeOffset</span></span>|<span data-ttu-id="9efad-114">履歴アイテムが発生した時刻。</span><span class="sxs-lookup"><span data-stu-id="9efad-114">Time when the history item occurred.</span></span> <span data-ttu-id="9efad-115">[mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="9efad-115">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="9efad-116">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="9efad-116">Relationships</span></span>
<span data-ttu-id="9efad-117">なし</span><span class="sxs-lookup"><span data-stu-id="9efad-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9efad-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="9efad-118">JSON Representation</span></span>
<span data-ttu-id="9efad-119">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="9efad-119">Here is a JSON representation of the resource.</span></span>
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




