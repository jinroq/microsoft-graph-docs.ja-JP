---
title: vppTokenLicenseSummary リソースの種類
description: トークンで指定されたアプリケーションのライセンスの概要です。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 8fb84a549d95459db1e4b39c11b526f73db08752
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29395182"
---
# <a name="vpptokenlicensesummary-resource-type"></a><span data-ttu-id="2b314-103">vppTokenLicenseSummary リソースの種類</span><span class="sxs-lookup"><span data-stu-id="2b314-103">vppTokenLicenseSummary resource type</span></span>

> <span data-ttu-id="2b314-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="2b314-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="2b314-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2b314-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2b314-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="2b314-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2b314-107">トークンで指定されたアプリケーションのライセンスの概要です。</span><span class="sxs-lookup"><span data-stu-id="2b314-107">License summary of a given app in a token.</span></span>

## <a name="properties"></a><span data-ttu-id="2b314-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2b314-108">Properties</span></span>
|<span data-ttu-id="2b314-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2b314-109">Property</span></span>|<span data-ttu-id="2b314-110">型</span><span class="sxs-lookup"><span data-stu-id="2b314-110">Type</span></span>|<span data-ttu-id="2b314-111">説明</span><span class="sxs-lookup"><span data-stu-id="2b314-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2b314-112">vppTokenId</span><span class="sxs-lookup"><span data-stu-id="2b314-112">vppTokenId</span></span>|<span data-ttu-id="2b314-113">String</span><span class="sxs-lookup"><span data-stu-id="2b314-113">String</span></span>|<span data-ttu-id="2b314-114">VPP トークンの識別子です。</span><span class="sxs-lookup"><span data-stu-id="2b314-114">Identifier of the VPP token.</span></span>|
|<span data-ttu-id="2b314-115">appleId</span><span class="sxs-lookup"><span data-stu-id="2b314-115">appleId</span></span>|<span data-ttu-id="2b314-116">String</span><span class="sxs-lookup"><span data-stu-id="2b314-116">String</span></span>|<span data-ttu-id="2b314-117">特定の Apple ボリューム購入プログラムのトークンに関連付けられている Apple ID。</span><span class="sxs-lookup"><span data-stu-id="2b314-117">The Apple Id associated with the given Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="2b314-118">organizationName</span><span class="sxs-lookup"><span data-stu-id="2b314-118">organizationName</span></span>|<span data-ttu-id="2b314-119">String</span><span class="sxs-lookup"><span data-stu-id="2b314-119">String</span></span>|<span data-ttu-id="2b314-120">Apple ボリューム購入プログラム トークンに関連付けられている組織です。</span><span class="sxs-lookup"><span data-stu-id="2b314-120">The organization associated with the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="2b314-121">availableLicenseCount</span><span class="sxs-lookup"><span data-stu-id="2b314-121">availableLicenseCount</span></span>|<span data-ttu-id="2b314-122">Int32</span><span class="sxs-lookup"><span data-stu-id="2b314-122">Int32</span></span>|<span data-ttu-id="2b314-123">VPP のライセンスが使用可能な数です。</span><span class="sxs-lookup"><span data-stu-id="2b314-123">The number of VPP licenses available.</span></span>|
|<span data-ttu-id="2b314-124">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="2b314-124">usedLicenseCount</span></span>|<span data-ttu-id="2b314-125">Int32</span><span class="sxs-lookup"><span data-stu-id="2b314-125">Int32</span></span>|<span data-ttu-id="2b314-126">使用中の VPP ライセンスの数。</span><span class="sxs-lookup"><span data-stu-id="2b314-126">The number of VPP licenses in use.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2b314-127">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="2b314-127">Relationships</span></span>
<span data-ttu-id="2b314-128">なし</span><span class="sxs-lookup"><span data-stu-id="2b314-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2b314-129">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="2b314-129">JSON Representation</span></span>
<span data-ttu-id="2b314-130">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="2b314-130">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.vppTokenLicenseSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.vppTokenLicenseSummary",
  "vppTokenId": "String",
  "appleId": "String",
  "organizationName": "String",
  "availableLicenseCount": 1024,
  "usedLicenseCount": 1024
}
```




