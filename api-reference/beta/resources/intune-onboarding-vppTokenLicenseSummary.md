---
title: vppTokenLicenseSummary リソースの種類
description: トークン内の特定のアプリのライセンスの概要。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: f421da54543d74009cb921ec429e3795e31d8572
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36375395"
---
# <a name="vpptokenlicensesummary-resource-type"></a><span data-ttu-id="8a301-103">vppTokenLicenseSummary リソースの種類</span><span class="sxs-lookup"><span data-stu-id="8a301-103">vppTokenLicenseSummary resource type</span></span>

> <span data-ttu-id="8a301-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8a301-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8a301-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="8a301-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8a301-106">トークン内の特定のアプリのライセンスの概要。</span><span class="sxs-lookup"><span data-stu-id="8a301-106">License summary of a given app in a token.</span></span>

## <a name="properties"></a><span data-ttu-id="8a301-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8a301-107">Properties</span></span>
|<span data-ttu-id="8a301-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8a301-108">Property</span></span>|<span data-ttu-id="8a301-109">型</span><span class="sxs-lookup"><span data-stu-id="8a301-109">Type</span></span>|<span data-ttu-id="8a301-110">説明</span><span class="sxs-lookup"><span data-stu-id="8a301-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8a301-111">vppTokenId</span><span class="sxs-lookup"><span data-stu-id="8a301-111">vppTokenId</span></span>|<span data-ttu-id="8a301-112">String</span><span class="sxs-lookup"><span data-stu-id="8a301-112">String</span></span>|<span data-ttu-id="8a301-113">VPP トークンの識別子。</span><span class="sxs-lookup"><span data-stu-id="8a301-113">Identifier of the VPP token.</span></span>|
|<span data-ttu-id="8a301-114">appleId</span><span class="sxs-lookup"><span data-stu-id="8a301-114">appleId</span></span>|<span data-ttu-id="8a301-115">String</span><span class="sxs-lookup"><span data-stu-id="8a301-115">String</span></span>|<span data-ttu-id="8a301-116">特定の Apple ボリューム購入プログラムのトークンに関連付けられている Apple ID。</span><span class="sxs-lookup"><span data-stu-id="8a301-116">The Apple Id associated with the given Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="8a301-117">organizationName</span><span class="sxs-lookup"><span data-stu-id="8a301-117">organizationName</span></span>|<span data-ttu-id="8a301-118">String</span><span class="sxs-lookup"><span data-stu-id="8a301-118">String</span></span>|<span data-ttu-id="8a301-119">Apple Volume Purchase Program のトークンに関連付けられている組織。</span><span class="sxs-lookup"><span data-stu-id="8a301-119">The organization associated with the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="8a301-120">availableLicenseCount</span><span class="sxs-lookup"><span data-stu-id="8a301-120">availableLicenseCount</span></span>|<span data-ttu-id="8a301-121">Int32</span><span class="sxs-lookup"><span data-stu-id="8a301-121">Int32</span></span>|<span data-ttu-id="8a301-122">使用可能な VPP ライセンスの数。</span><span class="sxs-lookup"><span data-stu-id="8a301-122">The number of VPP licenses available.</span></span>|
|<span data-ttu-id="8a301-123">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="8a301-123">usedLicenseCount</span></span>|<span data-ttu-id="8a301-124">Int32</span><span class="sxs-lookup"><span data-stu-id="8a301-124">Int32</span></span>|<span data-ttu-id="8a301-125">使用中の VPP ライセンスの数。</span><span class="sxs-lookup"><span data-stu-id="8a301-125">The number of VPP licenses in use.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8a301-126">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="8a301-126">Relationships</span></span>
<span data-ttu-id="8a301-127">なし</span><span class="sxs-lookup"><span data-stu-id="8a301-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8a301-128">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="8a301-128">JSON Representation</span></span>
<span data-ttu-id="8a301-129">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="8a301-129">Here is a JSON representation of the resource.</span></span>
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



