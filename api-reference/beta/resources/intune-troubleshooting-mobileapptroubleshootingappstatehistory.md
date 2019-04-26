---
title: mobileAppTroubleshootingAppStateHistory リソースの種類
description: モバイルアプリのトラブルシューティングイベントに含まれる履歴アイテム。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 75285b5dec8b3b3808f2e81a4655d9298d12d486
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32570667"
---
# <a name="mobileapptroubleshootingappstatehistory-resource-type"></a><span data-ttu-id="e0000-103">mobileAppTroubleshootingAppStateHistory リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e0000-103">mobileAppTroubleshootingAppStateHistory resource type</span></span>

> <span data-ttu-id="e0000-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e0000-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e0000-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="e0000-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e0000-106">モバイルアプリのトラブルシューティングイベントに含まれる履歴アイテム。</span><span class="sxs-lookup"><span data-stu-id="e0000-106">History Item contained in the Mobile App Troubleshooting Event.</span></span>


<span data-ttu-id="e0000-107">[mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="e0000-107">Inherits from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="e0000-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e0000-108">Properties</span></span>
|<span data-ttu-id="e0000-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e0000-109">Property</span></span>|<span data-ttu-id="e0000-110">型</span><span class="sxs-lookup"><span data-stu-id="e0000-110">Type</span></span>|<span data-ttu-id="e0000-111">説明</span><span class="sxs-lookup"><span data-stu-id="e0000-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e0000-112">occurrenceDateTime</span><span class="sxs-lookup"><span data-stu-id="e0000-112">occurrenceDateTime</span></span>|<span data-ttu-id="e0000-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e0000-113">DateTimeOffset</span></span>|<span data-ttu-id="e0000-114">履歴アイテムが発生した時刻。</span><span class="sxs-lookup"><span data-stu-id="e0000-114">Time when the history item occurred.</span></span> <span data-ttu-id="e0000-115">[mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="e0000-115">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|
|<span data-ttu-id="e0000-116">actionType</span><span class="sxs-lookup"><span data-stu-id="e0000-116">actionType</span></span>|[<span data-ttu-id="e0000-117">mobileAppActionType</span><span class="sxs-lookup"><span data-stu-id="e0000-117">mobileAppActionType</span></span>](../resources/intune-troubleshooting-mobileappactiontype.md)|<span data-ttu-id="e0000-118">対象となった AAD セキュリティグループ id。</span><span class="sxs-lookup"><span data-stu-id="e0000-118">AAD security group id to which it was targeted.</span></span> <span data-ttu-id="e0000-119">可能な値は、`unknown`、`installCommandSent`、`installed`、`uninstalled`、`userRequestedInstall` です。</span><span class="sxs-lookup"><span data-stu-id="e0000-119">Possible values are: `unknown`, `installCommandSent`, `installed`, `uninstalled`, `userRequestedInstall`.</span></span>|
|<span data-ttu-id="e0000-120">runstate</span><span class="sxs-lookup"><span data-stu-id="e0000-120">runState</span></span>|[<span data-ttu-id="e0000-121">runstate</span><span class="sxs-lookup"><span data-stu-id="e0000-121">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="e0000-122">アイテムの状態。</span><span class="sxs-lookup"><span data-stu-id="e0000-122">Status of the item.</span></span> <span data-ttu-id="e0000-123">可能な値は `unknown`、`success`、`fail` です。</span><span class="sxs-lookup"><span data-stu-id="e0000-123">Possible values are: `unknown`, `success`, `fail`.</span></span>|
|<span data-ttu-id="e0000-124">errorCode</span><span class="sxs-lookup"><span data-stu-id="e0000-124">errorCode</span></span>|<span data-ttu-id="e0000-125">String</span><span class="sxs-lookup"><span data-stu-id="e0000-125">String</span></span>|<span data-ttu-id="e0000-126">失敗のエラーコード。エラーがない場合は空です。</span><span class="sxs-lookup"><span data-stu-id="e0000-126">Error code for the failure, empty if no failure.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e0000-127">関係</span><span class="sxs-lookup"><span data-stu-id="e0000-127">Relationships</span></span>
<span data-ttu-id="e0000-128">なし</span><span class="sxs-lookup"><span data-stu-id="e0000-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e0000-129">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e0000-129">JSON Representation</span></span>
<span data-ttu-id="e0000-130">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="e0000-130">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mobileAppTroubleshootingAppStateHistory"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppTroubleshootingAppStateHistory",
  "occurrenceDateTime": "String (timestamp)",
  "actionType": "String",
  "runState": "String",
  "errorCode": "String"
}
```



