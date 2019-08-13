---
title: mobileAppTroubleshootingAppTargetHistory リソースの種類
description: モバイルアプリのトラブルシューティングイベントに含まれる履歴アイテム。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 3964702646476f35f7f6e9b7928b69fca83dc5e8
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36371307"
---
# <a name="mobileapptroubleshootingapptargethistory-resource-type"></a><span data-ttu-id="cdbd1-103">mobileAppTroubleshootingAppTargetHistory リソースの種類</span><span class="sxs-lookup"><span data-stu-id="cdbd1-103">mobileAppTroubleshootingAppTargetHistory resource type</span></span>

> <span data-ttu-id="cdbd1-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cdbd1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cdbd1-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="cdbd1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cdbd1-106">モバイルアプリのトラブルシューティングイベントに含まれる履歴アイテム。</span><span class="sxs-lookup"><span data-stu-id="cdbd1-106">History Item contained in the Mobile App Troubleshooting Event.</span></span>


<span data-ttu-id="cdbd1-107">[MobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="cdbd1-107">Inherits from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="cdbd1-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cdbd1-108">Properties</span></span>
|<span data-ttu-id="cdbd1-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cdbd1-109">Property</span></span>|<span data-ttu-id="cdbd1-110">型</span><span class="sxs-lookup"><span data-stu-id="cdbd1-110">Type</span></span>|<span data-ttu-id="cdbd1-111">説明</span><span class="sxs-lookup"><span data-stu-id="cdbd1-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cdbd1-112">occurrenceDateTime</span><span class="sxs-lookup"><span data-stu-id="cdbd1-112">occurrenceDateTime</span></span>|<span data-ttu-id="cdbd1-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cdbd1-113">DateTimeOffset</span></span>|<span data-ttu-id="cdbd1-114">履歴アイテムが発生した時刻。</span><span class="sxs-lookup"><span data-stu-id="cdbd1-114">Time when the history item occurred.</span></span> <span data-ttu-id="cdbd1-115">[MobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="cdbd1-115">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|
|<span data-ttu-id="cdbd1-116">securityGroupId</span><span class="sxs-lookup"><span data-stu-id="cdbd1-116">securityGroupId</span></span>|<span data-ttu-id="cdbd1-117">String</span><span class="sxs-lookup"><span data-stu-id="cdbd1-117">String</span></span>|<span data-ttu-id="cdbd1-118">対象となった AAD セキュリティグループ id。</span><span class="sxs-lookup"><span data-stu-id="cdbd1-118">AAD security group id to which it was targeted.</span></span>|
|<span data-ttu-id="cdbd1-119">runState</span><span class="sxs-lookup"><span data-stu-id="cdbd1-119">runState</span></span>|[<span data-ttu-id="cdbd1-120">runState</span><span class="sxs-lookup"><span data-stu-id="cdbd1-120">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="cdbd1-121">アイテムの状態。</span><span class="sxs-lookup"><span data-stu-id="cdbd1-121">Status of the item.</span></span> <span data-ttu-id="cdbd1-122">可能な値は、`unknown`、`success`、`fail`、`error`、`pending` です。</span><span class="sxs-lookup"><span data-stu-id="cdbd1-122">Possible values are: `unknown`, `success`, `fail`, `error`, `pending`.</span></span>|
|<span data-ttu-id="cdbd1-123">errorCode</span><span class="sxs-lookup"><span data-stu-id="cdbd1-123">errorCode</span></span>|<span data-ttu-id="cdbd1-124">String</span><span class="sxs-lookup"><span data-stu-id="cdbd1-124">String</span></span>|<span data-ttu-id="cdbd1-125">失敗のエラーコード。エラーがない場合は空です。</span><span class="sxs-lookup"><span data-stu-id="cdbd1-125">Error code for the failure, empty if no failure.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cdbd1-126">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="cdbd1-126">Relationships</span></span>
<span data-ttu-id="cdbd1-127">なし</span><span class="sxs-lookup"><span data-stu-id="cdbd1-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="cdbd1-128">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="cdbd1-128">JSON Representation</span></span>
<span data-ttu-id="cdbd1-129">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="cdbd1-129">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mobileAppTroubleshootingAppTargetHistory"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppTroubleshootingAppTargetHistory",
  "occurrenceDateTime": "String (timestamp)",
  "securityGroupId": "String",
  "runState": "String",
  "errorCode": "String"
}
```



