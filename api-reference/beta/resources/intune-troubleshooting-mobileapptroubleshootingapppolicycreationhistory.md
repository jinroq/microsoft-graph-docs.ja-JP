---
title: mobileAppTroubleshootingAppPolicyCreationHistory リソースの種類
description: モバイルアプリのトラブルシューティングイベントに含まれる履歴アイテム。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 416a5c7171a03db48d0b349a2a6415a940e5b798
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34988070"
---
# <a name="mobileapptroubleshootingapppolicycreationhistory-resource-type"></a><span data-ttu-id="d08cb-103">mobileAppTroubleshootingAppPolicyCreationHistory リソースの種類</span><span class="sxs-lookup"><span data-stu-id="d08cb-103">mobileAppTroubleshootingAppPolicyCreationHistory resource type</span></span>

> <span data-ttu-id="d08cb-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d08cb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d08cb-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="d08cb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d08cb-106">モバイルアプリのトラブルシューティングイベントに含まれる履歴アイテム。</span><span class="sxs-lookup"><span data-stu-id="d08cb-106">History Item contained in the Mobile App Troubleshooting Event.</span></span>


<span data-ttu-id="d08cb-107">[MobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="d08cb-107">Inherits from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="d08cb-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d08cb-108">Properties</span></span>
|<span data-ttu-id="d08cb-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d08cb-109">Property</span></span>|<span data-ttu-id="d08cb-110">型</span><span class="sxs-lookup"><span data-stu-id="d08cb-110">Type</span></span>|<span data-ttu-id="d08cb-111">説明</span><span class="sxs-lookup"><span data-stu-id="d08cb-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d08cb-112">occurrenceDateTime</span><span class="sxs-lookup"><span data-stu-id="d08cb-112">occurrenceDateTime</span></span>|<span data-ttu-id="d08cb-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d08cb-113">DateTimeOffset</span></span>|<span data-ttu-id="d08cb-114">履歴アイテムが発生した時刻。</span><span class="sxs-lookup"><span data-stu-id="d08cb-114">Time when the history item occurred.</span></span> <span data-ttu-id="d08cb-115">[MobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="d08cb-115">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|
|<span data-ttu-id="d08cb-116">runState</span><span class="sxs-lookup"><span data-stu-id="d08cb-116">runState</span></span>|[<span data-ttu-id="d08cb-117">runState</span><span class="sxs-lookup"><span data-stu-id="d08cb-117">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="d08cb-118">アイテムの状態。</span><span class="sxs-lookup"><span data-stu-id="d08cb-118">Status of the item.</span></span> <span data-ttu-id="d08cb-119">可能な値は、`unknown`、`success`、`fail` です。</span><span class="sxs-lookup"><span data-stu-id="d08cb-119">Possible values are: `unknown`, `success`, `fail`.</span></span>|
|<span data-ttu-id="d08cb-120">errorCode</span><span class="sxs-lookup"><span data-stu-id="d08cb-120">errorCode</span></span>|<span data-ttu-id="d08cb-121">String</span><span class="sxs-lookup"><span data-stu-id="d08cb-121">String</span></span>|<span data-ttu-id="d08cb-122">失敗のエラーコード。エラーがない場合は空です。</span><span class="sxs-lookup"><span data-stu-id="d08cb-122">Error code for the failure, empty if no failure.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d08cb-123">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="d08cb-123">Relationships</span></span>
<span data-ttu-id="d08cb-124">なし</span><span class="sxs-lookup"><span data-stu-id="d08cb-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d08cb-125">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d08cb-125">JSON Representation</span></span>
<span data-ttu-id="d08cb-126">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="d08cb-126">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mobileAppTroubleshootingAppPolicyCreationHistory"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppTroubleshootingAppPolicyCreationHistory",
  "occurrenceDateTime": "String (timestamp)",
  "runState": "String",
  "errorCode": "String"
}
```





