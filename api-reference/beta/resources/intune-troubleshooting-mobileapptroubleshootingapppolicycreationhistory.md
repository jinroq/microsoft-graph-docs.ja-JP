---
title: mobileAppTroubleshootingAppPolicyCreationHistory リソースの種類
description: モバイルアプリのトラブルシューティングイベントに含まれる履歴アイテム。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a93b88f850e2fa220903362375774d8a6dded59c
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30160502"
---
# <a name="mobileapptroubleshootingapppolicycreationhistory-resource-type"></a><span data-ttu-id="3d988-103">mobileAppTroubleshootingAppPolicyCreationHistory リソースの種類</span><span class="sxs-lookup"><span data-stu-id="3d988-103">mobileAppTroubleshootingAppPolicyCreationHistory resource type</span></span>

> <span data-ttu-id="3d988-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3d988-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3d988-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="3d988-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3d988-106">モバイルアプリのトラブルシューティングイベントに含まれる履歴アイテム。</span><span class="sxs-lookup"><span data-stu-id="3d988-106">History Item contained in the Mobile App Troubleshooting Event.</span></span>


<span data-ttu-id="3d988-107">[mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="3d988-107">Inherits from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="3d988-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3d988-108">Properties</span></span>
|<span data-ttu-id="3d988-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3d988-109">Property</span></span>|<span data-ttu-id="3d988-110">型</span><span class="sxs-lookup"><span data-stu-id="3d988-110">Type</span></span>|<span data-ttu-id="3d988-111">説明</span><span class="sxs-lookup"><span data-stu-id="3d988-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3d988-112">occurrenceDateTime</span><span class="sxs-lookup"><span data-stu-id="3d988-112">occurrenceDateTime</span></span>|<span data-ttu-id="3d988-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3d988-113">DateTimeOffset</span></span>|<span data-ttu-id="3d988-114">履歴アイテムが発生した時刻。</span><span class="sxs-lookup"><span data-stu-id="3d988-114">Time when the history item occurred.</span></span> <span data-ttu-id="3d988-115">[mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="3d988-115">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|
|<span data-ttu-id="3d988-116">runstate</span><span class="sxs-lookup"><span data-stu-id="3d988-116">runState</span></span>|[<span data-ttu-id="3d988-117">runstate</span><span class="sxs-lookup"><span data-stu-id="3d988-117">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="3d988-118">アイテムの状態。</span><span class="sxs-lookup"><span data-stu-id="3d988-118">Status of the item.</span></span> <span data-ttu-id="3d988-119">可能な値は `unknown`、`success`、`fail` です。</span><span class="sxs-lookup"><span data-stu-id="3d988-119">Possible values are: `unknown`, `success`, `fail`.</span></span>|
|<span data-ttu-id="3d988-120">errorCode</span><span class="sxs-lookup"><span data-stu-id="3d988-120">errorCode</span></span>|<span data-ttu-id="3d988-121">String</span><span class="sxs-lookup"><span data-stu-id="3d988-121">String</span></span>|<span data-ttu-id="3d988-122">失敗のエラーコード。エラーがない場合は空です。</span><span class="sxs-lookup"><span data-stu-id="3d988-122">Error code for the failure, empty if no failure.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3d988-123">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="3d988-123">Relationships</span></span>
<span data-ttu-id="3d988-124">なし</span><span class="sxs-lookup"><span data-stu-id="3d988-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3d988-125">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="3d988-125">JSON Representation</span></span>
<span data-ttu-id="3d988-126">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="3d988-126">Here is a JSON representation of the resource.</span></span>
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




