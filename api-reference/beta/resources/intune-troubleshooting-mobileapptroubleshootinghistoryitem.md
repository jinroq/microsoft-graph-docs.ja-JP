---
title: mobileAppTroubleshootingHistoryItem リソースの種類
description: モバイルアプリのトラブルシューティングイベントに含まれる履歴アイテム。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4bc87f30a970f305a309a320030cde419961660f
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31794618"
---
# <a name="mobileapptroubleshootinghistoryitem-resource-type"></a><span data-ttu-id="09679-103">mobileAppTroubleshootingHistoryItem リソースの種類</span><span class="sxs-lookup"><span data-stu-id="09679-103">mobileAppTroubleshootingHistoryItem resource type</span></span>

> <span data-ttu-id="09679-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="09679-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="09679-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="09679-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="09679-106">モバイルアプリのトラブルシューティングイベントに含まれる履歴アイテム。</span><span class="sxs-lookup"><span data-stu-id="09679-106">History Item contained in the Mobile App Troubleshooting Event.</span></span>

## <a name="properties"></a><span data-ttu-id="09679-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="09679-107">Properties</span></span>
|<span data-ttu-id="09679-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="09679-108">Property</span></span>|<span data-ttu-id="09679-109">型</span><span class="sxs-lookup"><span data-stu-id="09679-109">Type</span></span>|<span data-ttu-id="09679-110">説明</span><span class="sxs-lookup"><span data-stu-id="09679-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="09679-111">occurrenceDateTime</span><span class="sxs-lookup"><span data-stu-id="09679-111">occurrenceDateTime</span></span>|<span data-ttu-id="09679-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="09679-112">DateTimeOffset</span></span>|<span data-ttu-id="09679-113">履歴アイテムが発生した時刻。</span><span class="sxs-lookup"><span data-stu-id="09679-113">Time when the history item occurred.</span></span>|

## <a name="relationships"></a><span data-ttu-id="09679-114">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="09679-114">Relationships</span></span>
<span data-ttu-id="09679-115">なし</span><span class="sxs-lookup"><span data-stu-id="09679-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="09679-116">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="09679-116">JSON Representation</span></span>
<span data-ttu-id="09679-117">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="09679-117">Here is a JSON representation of the resource.</span></span>
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



