---
title: mobileAppTroubleshootingAppUpdateHistory リソースの種類
description: モバイルアプリのトラブルシューティングイベントに含まれる履歴アイテム。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c957f870f7a63506299a22b0b3496b6fa2096bd0
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32570632"
---
# <a name="mobileapptroubleshootingappupdatehistory-resource-type"></a><span data-ttu-id="4803f-103">mobileAppTroubleshootingAppUpdateHistory リソースの種類</span><span class="sxs-lookup"><span data-stu-id="4803f-103">mobileAppTroubleshootingAppUpdateHistory resource type</span></span>

> <span data-ttu-id="4803f-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4803f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4803f-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="4803f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4803f-106">モバイルアプリのトラブルシューティングイベントに含まれる履歴アイテム。</span><span class="sxs-lookup"><span data-stu-id="4803f-106">History Item contained in the Mobile App Troubleshooting Event.</span></span>


<span data-ttu-id="4803f-107">[mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="4803f-107">Inherits from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="4803f-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4803f-108">Properties</span></span>
|<span data-ttu-id="4803f-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4803f-109">Property</span></span>|<span data-ttu-id="4803f-110">型</span><span class="sxs-lookup"><span data-stu-id="4803f-110">Type</span></span>|<span data-ttu-id="4803f-111">説明</span><span class="sxs-lookup"><span data-stu-id="4803f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4803f-112">occurrenceDateTime</span><span class="sxs-lookup"><span data-stu-id="4803f-112">occurrenceDateTime</span></span>|<span data-ttu-id="4803f-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4803f-113">DateTimeOffset</span></span>|<span data-ttu-id="4803f-114">履歴アイテムが発生した時刻。</span><span class="sxs-lookup"><span data-stu-id="4803f-114">Time when the history item occurred.</span></span> <span data-ttu-id="4803f-115">[mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="4803f-115">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="4803f-116">関係</span><span class="sxs-lookup"><span data-stu-id="4803f-116">Relationships</span></span>
<span data-ttu-id="4803f-117">なし</span><span class="sxs-lookup"><span data-stu-id="4803f-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4803f-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="4803f-118">JSON Representation</span></span>
<span data-ttu-id="4803f-119">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="4803f-119">Here is a JSON representation of the resource.</span></span>
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



