---
title: officeUserCheckinSummary リソースの種類
description: チェックインのテナント統計 (stats) を記述するエンティティです。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: c2470b1e531f1b268d6797fe2692baf0031728b3
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27834022"
---
# <a name="officeusercheckinsummary-resource-type"></a><span data-ttu-id="6f60f-103">officeUserCheckinSummary リソースの種類</span><span class="sxs-lookup"><span data-stu-id="6f60f-103">officeUserCheckinSummary resource type</span></span>

> <span data-ttu-id="6f60f-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="6f60f-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6f60f-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6f60f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6f60f-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="6f60f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6f60f-107">チェックインのテナント統計 (stats) を記述するエンティティです。</span><span class="sxs-lookup"><span data-stu-id="6f60f-107">Entity that describes  tenant check-in stats.</span></span>
## <a name="properties"></a><span data-ttu-id="6f60f-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6f60f-108">Properties</span></span>
|<span data-ttu-id="6f60f-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6f60f-109">Property</span></span>|<span data-ttu-id="6f60f-110">種類</span><span class="sxs-lookup"><span data-stu-id="6f60f-110">Type</span></span>|<span data-ttu-id="6f60f-111">説明</span><span class="sxs-lookup"><span data-stu-id="6f60f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6f60f-112">succeededUserCount</span><span class="sxs-lookup"><span data-stu-id="6f60f-112">succeededUserCount</span></span>|<span data-ttu-id="6f60f-113">Int32</span><span class="sxs-lookup"><span data-stu-id="6f60f-113">Int32</span></span>|<span data-ttu-id="6f60f-114">成功したユーザーの合計は、過去 3 か月のアドインを確認します。</span><span class="sxs-lookup"><span data-stu-id="6f60f-114">Total successful user check ins for the last 3 months.</span></span>|
|<span data-ttu-id="6f60f-115">failedUserCount</span><span class="sxs-lookup"><span data-stu-id="6f60f-115">failedUserCount</span></span>|<span data-ttu-id="6f60f-116">Int32</span><span class="sxs-lookup"><span data-stu-id="6f60f-116">Int32</span></span>|<span data-ttu-id="6f60f-117">障害が発生したユーザーの合計は、過去 3 か月のアドインを確認します。</span><span class="sxs-lookup"><span data-stu-id="6f60f-117">Total failed user check ins for the last 3 months.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6f60f-118">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="6f60f-118">Relationships</span></span>
<span data-ttu-id="6f60f-119">なし</span><span class="sxs-lookup"><span data-stu-id="6f60f-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="6f60f-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="6f60f-120">JSON Representation</span></span>
<span data-ttu-id="6f60f-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="6f60f-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.officeUserCheckinSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.officeUserCheckinSummary",
  "succeededUserCount": 1024,
  "failedUserCount": 1024
}
```



