---
title: mobileAppTroubleshootingAppTargetHistory リソースの種類
description: モバイルアプリのトラブルシューティングイベントに含まれる履歴アイテム。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 47a00ec29f91c81c513ef509e763c4071c106b1e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36010211"
---
# <a name="mobileapptroubleshootingapptargethistory-resource-type"></a><span data-ttu-id="c1812-103">mobileAppTroubleshootingAppTargetHistory リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c1812-103">mobileAppTroubleshootingAppTargetHistory resource type</span></span>

> <span data-ttu-id="c1812-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c1812-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c1812-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="c1812-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c1812-106">モバイルアプリのトラブルシューティングイベントに含まれる履歴アイテム。</span><span class="sxs-lookup"><span data-stu-id="c1812-106">History Item contained in the Mobile App Troubleshooting Event.</span></span>


<span data-ttu-id="c1812-107">[MobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="c1812-107">Inherits from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c1812-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c1812-108">Properties</span></span>
|<span data-ttu-id="c1812-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c1812-109">Property</span></span>|<span data-ttu-id="c1812-110">型</span><span class="sxs-lookup"><span data-stu-id="c1812-110">Type</span></span>|<span data-ttu-id="c1812-111">説明</span><span class="sxs-lookup"><span data-stu-id="c1812-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c1812-112">occurrenceDateTime</span><span class="sxs-lookup"><span data-stu-id="c1812-112">occurrenceDateTime</span></span>|<span data-ttu-id="c1812-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c1812-113">DateTimeOffset</span></span>|<span data-ttu-id="c1812-114">履歴アイテムが発生した時刻。</span><span class="sxs-lookup"><span data-stu-id="c1812-114">Time when the history item occurred.</span></span> <span data-ttu-id="c1812-115">[MobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="c1812-115">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|
|<span data-ttu-id="c1812-116">securityGroupId</span><span class="sxs-lookup"><span data-stu-id="c1812-116">securityGroupId</span></span>|<span data-ttu-id="c1812-117">String</span><span class="sxs-lookup"><span data-stu-id="c1812-117">String</span></span>|<span data-ttu-id="c1812-118">対象となった AAD セキュリティグループ id。</span><span class="sxs-lookup"><span data-stu-id="c1812-118">AAD security group id to which it was targeted.</span></span>|
|<span data-ttu-id="c1812-119">runState</span><span class="sxs-lookup"><span data-stu-id="c1812-119">runState</span></span>|[<span data-ttu-id="c1812-120">runState</span><span class="sxs-lookup"><span data-stu-id="c1812-120">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="c1812-121">アイテムの状態。</span><span class="sxs-lookup"><span data-stu-id="c1812-121">Status of the item.</span></span> <span data-ttu-id="c1812-122">可能な値は、`unknown`、`success`、`fail` です。</span><span class="sxs-lookup"><span data-stu-id="c1812-122">Possible values are: `unknown`, `success`, `fail`.</span></span>|
|<span data-ttu-id="c1812-123">errorCode</span><span class="sxs-lookup"><span data-stu-id="c1812-123">errorCode</span></span>|<span data-ttu-id="c1812-124">String</span><span class="sxs-lookup"><span data-stu-id="c1812-124">String</span></span>|<span data-ttu-id="c1812-125">失敗のエラーコード。エラーがない場合は空です。</span><span class="sxs-lookup"><span data-stu-id="c1812-125">Error code for the failure, empty if no failure.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c1812-126">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="c1812-126">Relationships</span></span>
<span data-ttu-id="c1812-127">なし</span><span class="sxs-lookup"><span data-stu-id="c1812-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c1812-128">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c1812-128">JSON Representation</span></span>
<span data-ttu-id="c1812-129">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="c1812-129">Here is a JSON representation of the resource.</span></span>
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





