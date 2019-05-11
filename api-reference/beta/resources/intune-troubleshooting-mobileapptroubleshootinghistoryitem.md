---
title: mobileAppTroubleshootingHistoryItem リソースの種類
description: モバイルアプリのトラブルシューティングイベントに含まれる履歴アイテム。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8e63de7a150f36529237aac6f5f0794c8407e13e
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33938675"
---
# <a name="mobileapptroubleshootinghistoryitem-resource-type"></a><span data-ttu-id="05b85-103">mobileAppTroubleshootingHistoryItem リソースの種類</span><span class="sxs-lookup"><span data-stu-id="05b85-103">mobileAppTroubleshootingHistoryItem resource type</span></span>

> <span data-ttu-id="05b85-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="05b85-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="05b85-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="05b85-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="05b85-106">モバイルアプリのトラブルシューティングイベントに含まれる履歴アイテム。</span><span class="sxs-lookup"><span data-stu-id="05b85-106">History Item contained in the Mobile App Troubleshooting Event.</span></span>

## <a name="properties"></a><span data-ttu-id="05b85-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="05b85-107">Properties</span></span>
|<span data-ttu-id="05b85-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="05b85-108">Property</span></span>|<span data-ttu-id="05b85-109">型</span><span class="sxs-lookup"><span data-stu-id="05b85-109">Type</span></span>|<span data-ttu-id="05b85-110">説明</span><span class="sxs-lookup"><span data-stu-id="05b85-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="05b85-111">occurrenceDateTime</span><span class="sxs-lookup"><span data-stu-id="05b85-111">occurrenceDateTime</span></span>|<span data-ttu-id="05b85-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="05b85-112">DateTimeOffset</span></span>|<span data-ttu-id="05b85-113">履歴アイテムが発生した時刻。</span><span class="sxs-lookup"><span data-stu-id="05b85-113">Time when the history item occurred.</span></span>|

## <a name="relationships"></a><span data-ttu-id="05b85-114">関係</span><span class="sxs-lookup"><span data-stu-id="05b85-114">Relationships</span></span>
<span data-ttu-id="05b85-115">なし</span><span class="sxs-lookup"><span data-stu-id="05b85-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="05b85-116">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="05b85-116">JSON Representation</span></span>
<span data-ttu-id="05b85-117">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="05b85-117">Here is a JSON representation of the resource.</span></span>
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




