---
title: officeUserCheckinSummary リソースの種類
description: チェックインのテナント統計 (stats) を記述するエンティティです。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: d44c978ff1442c98038bf627397de5ca3a0ca3bf
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29411009"
---
# <a name="officeusercheckinsummary-resource-type"></a><span data-ttu-id="05773-103">officeUserCheckinSummary リソースの種類</span><span class="sxs-lookup"><span data-stu-id="05773-103">officeUserCheckinSummary resource type</span></span>

> <span data-ttu-id="05773-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="05773-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="05773-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="05773-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="05773-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="05773-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="05773-107">チェックインのテナント統計 (stats) を記述するエンティティです。</span><span class="sxs-lookup"><span data-stu-id="05773-107">Entity that describes  tenant check-in stats.</span></span>

## <a name="properties"></a><span data-ttu-id="05773-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="05773-108">Properties</span></span>
|<span data-ttu-id="05773-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="05773-109">Property</span></span>|<span data-ttu-id="05773-110">型</span><span class="sxs-lookup"><span data-stu-id="05773-110">Type</span></span>|<span data-ttu-id="05773-111">説明</span><span class="sxs-lookup"><span data-stu-id="05773-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="05773-112">succeededUserCount</span><span class="sxs-lookup"><span data-stu-id="05773-112">succeededUserCount</span></span>|<span data-ttu-id="05773-113">Int32</span><span class="sxs-lookup"><span data-stu-id="05773-113">Int32</span></span>|<span data-ttu-id="05773-114">成功したユーザーの合計は、過去 3 か月のアドインを確認します。</span><span class="sxs-lookup"><span data-stu-id="05773-114">Total successful user check ins for the last 3 months.</span></span>|
|<span data-ttu-id="05773-115">failedUserCount</span><span class="sxs-lookup"><span data-stu-id="05773-115">failedUserCount</span></span>|<span data-ttu-id="05773-116">Int32</span><span class="sxs-lookup"><span data-stu-id="05773-116">Int32</span></span>|<span data-ttu-id="05773-117">障害が発生したユーザーの合計は、過去 3 か月のアドインを確認します。</span><span class="sxs-lookup"><span data-stu-id="05773-117">Total failed user check ins for the last 3 months.</span></span>|

## <a name="relationships"></a><span data-ttu-id="05773-118">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="05773-118">Relationships</span></span>
<span data-ttu-id="05773-119">なし</span><span class="sxs-lookup"><span data-stu-id="05773-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="05773-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="05773-120">JSON Representation</span></span>
<span data-ttu-id="05773-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="05773-121">Here is a JSON representation of the resource.</span></span>
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



