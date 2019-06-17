---
title: mobileAppTroubleshootingDeviceCheckinHistory リソースの種類
description: モバイルアプリのトラブルシューティングイベントに含まれる履歴アイテム。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e86c630e87b3d809087ec0c83a16d97097e34a60
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34981476"
---
# <a name="mobileapptroubleshootingdevicecheckinhistory-resource-type"></a><span data-ttu-id="cae5a-103">mobileAppTroubleshootingDeviceCheckinHistory リソースの種類</span><span class="sxs-lookup"><span data-stu-id="cae5a-103">mobileAppTroubleshootingDeviceCheckinHistory resource type</span></span>

> <span data-ttu-id="cae5a-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cae5a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cae5a-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="cae5a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cae5a-106">モバイルアプリのトラブルシューティングイベントに含まれる履歴アイテム。</span><span class="sxs-lookup"><span data-stu-id="cae5a-106">History Item contained in the Mobile App Troubleshooting Event.</span></span>


<span data-ttu-id="cae5a-107">[MobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="cae5a-107">Inherits from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="cae5a-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cae5a-108">Properties</span></span>
|<span data-ttu-id="cae5a-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cae5a-109">Property</span></span>|<span data-ttu-id="cae5a-110">型</span><span class="sxs-lookup"><span data-stu-id="cae5a-110">Type</span></span>|<span data-ttu-id="cae5a-111">説明</span><span class="sxs-lookup"><span data-stu-id="cae5a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cae5a-112">occurrenceDateTime</span><span class="sxs-lookup"><span data-stu-id="cae5a-112">occurrenceDateTime</span></span>|<span data-ttu-id="cae5a-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cae5a-113">DateTimeOffset</span></span>|<span data-ttu-id="cae5a-114">履歴アイテムが発生した時刻。</span><span class="sxs-lookup"><span data-stu-id="cae5a-114">Time when the history item occurred.</span></span> <span data-ttu-id="cae5a-115">[MobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="cae5a-115">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="cae5a-116">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="cae5a-116">Relationships</span></span>
<span data-ttu-id="cae5a-117">なし</span><span class="sxs-lookup"><span data-stu-id="cae5a-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="cae5a-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="cae5a-118">JSON Representation</span></span>
<span data-ttu-id="cae5a-119">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="cae5a-119">Here is a JSON representation of the resource.</span></span>
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





