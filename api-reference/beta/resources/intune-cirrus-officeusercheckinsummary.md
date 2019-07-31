---
title: officeUserCheckinSummary リソースの種類
description: テナントのチェックイン統計を記述するエンティティ。
localization_priority: Normal
author: rolyon
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c364fe1a6da382ed8947b4b2bf63d2bce203d6ad
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36004800"
---
# <a name="officeusercheckinsummary-resource-type"></a><span data-ttu-id="67ae9-103">officeUserCheckinSummary リソースの種類</span><span class="sxs-lookup"><span data-stu-id="67ae9-103">officeUserCheckinSummary resource type</span></span>

> <span data-ttu-id="67ae9-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="67ae9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="67ae9-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="67ae9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="67ae9-106">テナントのチェックイン統計を記述するエンティティ。</span><span class="sxs-lookup"><span data-stu-id="67ae9-106">Entity that describes  tenant check-in stats.</span></span>

## <a name="properties"></a><span data-ttu-id="67ae9-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="67ae9-107">Properties</span></span>
|<span data-ttu-id="67ae9-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="67ae9-108">Property</span></span>|<span data-ttu-id="67ae9-109">型</span><span class="sxs-lookup"><span data-stu-id="67ae9-109">Type</span></span>|<span data-ttu-id="67ae9-110">説明</span><span class="sxs-lookup"><span data-stu-id="67ae9-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="67ae9-111">succeededUserCount</span><span class="sxs-lookup"><span data-stu-id="67ae9-111">succeededUserCount</span></span>|<span data-ttu-id="67ae9-112">Int32</span><span class="sxs-lookup"><span data-stu-id="67ae9-112">Int32</span></span>|<span data-ttu-id="67ae9-113">過去3か月間の成功したユーザーチェックインの合計数。</span><span class="sxs-lookup"><span data-stu-id="67ae9-113">Total successful user check ins for the last 3 months.</span></span>|
|<span data-ttu-id="67ae9-114">failedUserCount</span><span class="sxs-lookup"><span data-stu-id="67ae9-114">failedUserCount</span></span>|<span data-ttu-id="67ae9-115">Int32</span><span class="sxs-lookup"><span data-stu-id="67ae9-115">Int32</span></span>|<span data-ttu-id="67ae9-116">過去3か月間のユーザーチェックに失敗した合計数。</span><span class="sxs-lookup"><span data-stu-id="67ae9-116">Total failed user check ins for the last 3 months.</span></span>|

## <a name="relationships"></a><span data-ttu-id="67ae9-117">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="67ae9-117">Relationships</span></span>
<span data-ttu-id="67ae9-118">なし</span><span class="sxs-lookup"><span data-stu-id="67ae9-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="67ae9-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="67ae9-119">JSON Representation</span></span>
<span data-ttu-id="67ae9-120">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="67ae9-120">Here is a JSON representation of the resource.</span></span>
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



