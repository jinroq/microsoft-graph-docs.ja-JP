---
title: vpptokenlicensesummary リソースの種類
description: トークン内の特定のアプリのライセンスの概要。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f9c126323e0f5785752238ec64cfade2c34d5c24
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30161062"
---
# <a name="vpptokenlicensesummary-resource-type"></a><span data-ttu-id="4dfd2-103">vpptokenlicensesummary リソースの種類</span><span class="sxs-lookup"><span data-stu-id="4dfd2-103">vppTokenLicenseSummary resource type</span></span>

> <span data-ttu-id="4dfd2-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4dfd2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4dfd2-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="4dfd2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4dfd2-106">トークン内の特定のアプリのライセンスの概要。</span><span class="sxs-lookup"><span data-stu-id="4dfd2-106">License summary of a given app in a token.</span></span>

## <a name="properties"></a><span data-ttu-id="4dfd2-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4dfd2-107">Properties</span></span>
|<span data-ttu-id="4dfd2-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4dfd2-108">Property</span></span>|<span data-ttu-id="4dfd2-109">型</span><span class="sxs-lookup"><span data-stu-id="4dfd2-109">Type</span></span>|<span data-ttu-id="4dfd2-110">説明</span><span class="sxs-lookup"><span data-stu-id="4dfd2-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4dfd2-111">vppTokenId</span><span class="sxs-lookup"><span data-stu-id="4dfd2-111">vppTokenId</span></span>|<span data-ttu-id="4dfd2-112">String</span><span class="sxs-lookup"><span data-stu-id="4dfd2-112">String</span></span>|<span data-ttu-id="4dfd2-113">VPP トークンの識別子。</span><span class="sxs-lookup"><span data-stu-id="4dfd2-113">Identifier of the VPP token.</span></span>|
|<span data-ttu-id="4dfd2-114">appleId</span><span class="sxs-lookup"><span data-stu-id="4dfd2-114">appleId</span></span>|<span data-ttu-id="4dfd2-115">String</span><span class="sxs-lookup"><span data-stu-id="4dfd2-115">String</span></span>|<span data-ttu-id="4dfd2-116">特定の Apple ボリューム購入プログラムのトークンに関連付けられている Apple ID。</span><span class="sxs-lookup"><span data-stu-id="4dfd2-116">The Apple Id associated with the given Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="4dfd2-117">organizationName</span><span class="sxs-lookup"><span data-stu-id="4dfd2-117">organizationName</span></span>|<span data-ttu-id="4dfd2-118">String</span><span class="sxs-lookup"><span data-stu-id="4dfd2-118">String</span></span>|<span data-ttu-id="4dfd2-119">Apple volume purchase program のトークンに関連付けられている組織。</span><span class="sxs-lookup"><span data-stu-id="4dfd2-119">The organization associated with the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="4dfd2-120">availableLicenseCount</span><span class="sxs-lookup"><span data-stu-id="4dfd2-120">availableLicenseCount</span></span>|<span data-ttu-id="4dfd2-121">Int32</span><span class="sxs-lookup"><span data-stu-id="4dfd2-121">Int32</span></span>|<span data-ttu-id="4dfd2-122">使用可能な VPP ライセンスの数。</span><span class="sxs-lookup"><span data-stu-id="4dfd2-122">The number of VPP licenses available.</span></span>|
|<span data-ttu-id="4dfd2-123">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="4dfd2-123">usedLicenseCount</span></span>|<span data-ttu-id="4dfd2-124">Int32</span><span class="sxs-lookup"><span data-stu-id="4dfd2-124">Int32</span></span>|<span data-ttu-id="4dfd2-125">使用中の VPP ライセンスの数。</span><span class="sxs-lookup"><span data-stu-id="4dfd2-125">The number of VPP licenses in use.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4dfd2-126">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="4dfd2-126">Relationships</span></span>
<span data-ttu-id="4dfd2-127">なし</span><span class="sxs-lookup"><span data-stu-id="4dfd2-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4dfd2-128">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="4dfd2-128">JSON Representation</span></span>
<span data-ttu-id="4dfd2-129">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="4dfd2-129">Here is a JSON representation of the resource.</span></span>
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




