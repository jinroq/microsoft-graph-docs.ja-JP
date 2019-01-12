---
title: vppTokenLicenseSummary リソースの種類
description: トークンで指定されたアプリケーションのライセンスの概要です。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 0766fd4da996b57032154be98bbc22fd8c8a4a5b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27939960"
---
# <a name="vpptokenlicensesummary-resource-type"></a><span data-ttu-id="59785-103">vppTokenLicenseSummary リソースの種類</span><span class="sxs-lookup"><span data-stu-id="59785-103">vppTokenLicenseSummary resource type</span></span>

> <span data-ttu-id="59785-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="59785-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="59785-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="59785-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="59785-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="59785-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="59785-107">トークンで指定されたアプリケーションのライセンスの概要です。</span><span class="sxs-lookup"><span data-stu-id="59785-107">License summary of a given app in a token.</span></span>
## <a name="properties"></a><span data-ttu-id="59785-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="59785-108">Properties</span></span>
|<span data-ttu-id="59785-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="59785-109">Property</span></span>|<span data-ttu-id="59785-110">型</span><span class="sxs-lookup"><span data-stu-id="59785-110">Type</span></span>|<span data-ttu-id="59785-111">説明</span><span class="sxs-lookup"><span data-stu-id="59785-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="59785-112">vppTokenId</span><span class="sxs-lookup"><span data-stu-id="59785-112">vppTokenId</span></span>|<span data-ttu-id="59785-113">String</span><span class="sxs-lookup"><span data-stu-id="59785-113">String</span></span>|<span data-ttu-id="59785-114">VPP トークンの識別子です。</span><span class="sxs-lookup"><span data-stu-id="59785-114">Identifier of the VPP token.</span></span>|
|<span data-ttu-id="59785-115">appleId</span><span class="sxs-lookup"><span data-stu-id="59785-115">appleId</span></span>|<span data-ttu-id="59785-116">String</span><span class="sxs-lookup"><span data-stu-id="59785-116">String</span></span>|<span data-ttu-id="59785-117">特定の Apple ボリューム購入プログラムのトークンに関連付けられている Apple ID。</span><span class="sxs-lookup"><span data-stu-id="59785-117">The Apple Id associated with the given Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="59785-118">organizationName</span><span class="sxs-lookup"><span data-stu-id="59785-118">organizationName</span></span>|<span data-ttu-id="59785-119">String</span><span class="sxs-lookup"><span data-stu-id="59785-119">String</span></span>|<span data-ttu-id="59785-120">Apple ボリューム購入プログラム トークンに関連付けられている組織です。</span><span class="sxs-lookup"><span data-stu-id="59785-120">The organization associated with the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="59785-121">availableLicenseCount</span><span class="sxs-lookup"><span data-stu-id="59785-121">availableLicenseCount</span></span>|<span data-ttu-id="59785-122">Int32</span><span class="sxs-lookup"><span data-stu-id="59785-122">Int32</span></span>|<span data-ttu-id="59785-123">VPP のライセンスが使用可能な数です。</span><span class="sxs-lookup"><span data-stu-id="59785-123">The number of VPP licenses available.</span></span>|
|<span data-ttu-id="59785-124">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="59785-124">usedLicenseCount</span></span>|<span data-ttu-id="59785-125">Int32</span><span class="sxs-lookup"><span data-stu-id="59785-125">Int32</span></span>|<span data-ttu-id="59785-126">使用中の VPP ライセンスの数。</span><span class="sxs-lookup"><span data-stu-id="59785-126">The number of VPP licenses in use.</span></span>|

## <a name="relationships"></a><span data-ttu-id="59785-127">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="59785-127">Relationships</span></span>
<span data-ttu-id="59785-128">なし</span><span class="sxs-lookup"><span data-stu-id="59785-128">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="59785-129">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="59785-129">JSON Representation</span></span>
<span data-ttu-id="59785-130">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="59785-130">Here is a JSON representation of the resource.</span></span>
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





