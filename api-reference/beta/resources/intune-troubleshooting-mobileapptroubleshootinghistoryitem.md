---
title: mobileAppTroubleshootingHistoryItem リソースの種類
description: モバイルアプリのトラブルシューティングイベントに含まれる履歴アイテム。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 0136d8e4627875cf3b49e2c1f876bfb7454ea165
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36010218"
---
# <a name="mobileapptroubleshootinghistoryitem-resource-type"></a><span data-ttu-id="d049b-103">mobileAppTroubleshootingHistoryItem リソースの種類</span><span class="sxs-lookup"><span data-stu-id="d049b-103">mobileAppTroubleshootingHistoryItem resource type</span></span>

> <span data-ttu-id="d049b-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d049b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d049b-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="d049b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d049b-106">モバイルアプリのトラブルシューティングイベントに含まれる履歴アイテム。</span><span class="sxs-lookup"><span data-stu-id="d049b-106">History Item contained in the Mobile App Troubleshooting Event.</span></span>

## <a name="properties"></a><span data-ttu-id="d049b-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d049b-107">Properties</span></span>
|<span data-ttu-id="d049b-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d049b-108">Property</span></span>|<span data-ttu-id="d049b-109">型</span><span class="sxs-lookup"><span data-stu-id="d049b-109">Type</span></span>|<span data-ttu-id="d049b-110">説明</span><span class="sxs-lookup"><span data-stu-id="d049b-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d049b-111">occurrenceDateTime</span><span class="sxs-lookup"><span data-stu-id="d049b-111">occurrenceDateTime</span></span>|<span data-ttu-id="d049b-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d049b-112">DateTimeOffset</span></span>|<span data-ttu-id="d049b-113">履歴アイテムが発生した時刻。</span><span class="sxs-lookup"><span data-stu-id="d049b-113">Time when the history item occurred.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d049b-114">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="d049b-114">Relationships</span></span>
<span data-ttu-id="d049b-115">なし</span><span class="sxs-lookup"><span data-stu-id="d049b-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d049b-116">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d049b-116">JSON Representation</span></span>
<span data-ttu-id="d049b-117">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="d049b-117">Here is a JSON representation of the resource.</span></span>
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





