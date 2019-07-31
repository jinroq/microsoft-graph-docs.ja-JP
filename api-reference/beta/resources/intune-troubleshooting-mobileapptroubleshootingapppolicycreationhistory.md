---
title: mobileAppTroubleshootingAppPolicyCreationHistory リソースの種類
description: モバイルアプリのトラブルシューティングイベントに含まれる履歴アイテム。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 4cbbdd3159982ac82031e654890d90741fd48d15
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36010197"
---
# <a name="mobileapptroubleshootingapppolicycreationhistory-resource-type"></a><span data-ttu-id="3a58c-103">mobileAppTroubleshootingAppPolicyCreationHistory リソースの種類</span><span class="sxs-lookup"><span data-stu-id="3a58c-103">mobileAppTroubleshootingAppPolicyCreationHistory resource type</span></span>

> <span data-ttu-id="3a58c-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3a58c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3a58c-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="3a58c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3a58c-106">モバイルアプリのトラブルシューティングイベントに含まれる履歴アイテム。</span><span class="sxs-lookup"><span data-stu-id="3a58c-106">History Item contained in the Mobile App Troubleshooting Event.</span></span>


<span data-ttu-id="3a58c-107">[MobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="3a58c-107">Inherits from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="3a58c-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3a58c-108">Properties</span></span>
|<span data-ttu-id="3a58c-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3a58c-109">Property</span></span>|<span data-ttu-id="3a58c-110">型</span><span class="sxs-lookup"><span data-stu-id="3a58c-110">Type</span></span>|<span data-ttu-id="3a58c-111">説明</span><span class="sxs-lookup"><span data-stu-id="3a58c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3a58c-112">occurrenceDateTime</span><span class="sxs-lookup"><span data-stu-id="3a58c-112">occurrenceDateTime</span></span>|<span data-ttu-id="3a58c-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3a58c-113">DateTimeOffset</span></span>|<span data-ttu-id="3a58c-114">履歴アイテムが発生した時刻。</span><span class="sxs-lookup"><span data-stu-id="3a58c-114">Time when the history item occurred.</span></span> <span data-ttu-id="3a58c-115">[MobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="3a58c-115">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|
|<span data-ttu-id="3a58c-116">runState</span><span class="sxs-lookup"><span data-stu-id="3a58c-116">runState</span></span>|[<span data-ttu-id="3a58c-117">runState</span><span class="sxs-lookup"><span data-stu-id="3a58c-117">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="3a58c-118">アイテムの状態。</span><span class="sxs-lookup"><span data-stu-id="3a58c-118">Status of the item.</span></span> <span data-ttu-id="3a58c-119">可能な値は、`unknown`、`success`、`fail` です。</span><span class="sxs-lookup"><span data-stu-id="3a58c-119">Possible values are: `unknown`, `success`, `fail`.</span></span>|
|<span data-ttu-id="3a58c-120">errorCode</span><span class="sxs-lookup"><span data-stu-id="3a58c-120">errorCode</span></span>|<span data-ttu-id="3a58c-121">String</span><span class="sxs-lookup"><span data-stu-id="3a58c-121">String</span></span>|<span data-ttu-id="3a58c-122">失敗のエラーコード。エラーがない場合は空です。</span><span class="sxs-lookup"><span data-stu-id="3a58c-122">Error code for the failure, empty if no failure.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3a58c-123">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="3a58c-123">Relationships</span></span>
<span data-ttu-id="3a58c-124">なし</span><span class="sxs-lookup"><span data-stu-id="3a58c-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3a58c-125">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="3a58c-125">JSON Representation</span></span>
<span data-ttu-id="3a58c-126">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="3a58c-126">Here is a JSON representation of the resource.</span></span>
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





