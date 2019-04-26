---
title: mobileAppTroubleshootingHistoryItem リソースの種類
description: モバイルアプリのトラブルシューティングイベントに含まれる履歴アイテム。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4bc87f30a970f305a309a320030cde419961660f
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32570069"
---
# <a name="mobileapptroubleshootinghistoryitem-resource-type"></a><span data-ttu-id="bf8b4-103">mobileAppTroubleshootingHistoryItem リソースの種類</span><span class="sxs-lookup"><span data-stu-id="bf8b4-103">mobileAppTroubleshootingHistoryItem resource type</span></span>

> <span data-ttu-id="bf8b4-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bf8b4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bf8b4-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="bf8b4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bf8b4-106">モバイルアプリのトラブルシューティングイベントに含まれる履歴アイテム。</span><span class="sxs-lookup"><span data-stu-id="bf8b4-106">History Item contained in the Mobile App Troubleshooting Event.</span></span>

## <a name="properties"></a><span data-ttu-id="bf8b4-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bf8b4-107">Properties</span></span>
|<span data-ttu-id="bf8b4-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bf8b4-108">Property</span></span>|<span data-ttu-id="bf8b4-109">型</span><span class="sxs-lookup"><span data-stu-id="bf8b4-109">Type</span></span>|<span data-ttu-id="bf8b4-110">説明</span><span class="sxs-lookup"><span data-stu-id="bf8b4-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bf8b4-111">occurrenceDateTime</span><span class="sxs-lookup"><span data-stu-id="bf8b4-111">occurrenceDateTime</span></span>|<span data-ttu-id="bf8b4-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bf8b4-112">DateTimeOffset</span></span>|<span data-ttu-id="bf8b4-113">履歴アイテムが発生した時刻。</span><span class="sxs-lookup"><span data-stu-id="bf8b4-113">Time when the history item occurred.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bf8b4-114">関係</span><span class="sxs-lookup"><span data-stu-id="bf8b4-114">Relationships</span></span>
<span data-ttu-id="bf8b4-115">なし</span><span class="sxs-lookup"><span data-stu-id="bf8b4-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bf8b4-116">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="bf8b4-116">JSON Representation</span></span>
<span data-ttu-id="bf8b4-117">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="bf8b4-117">Here is a JSON representation of the resource.</span></span>
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



