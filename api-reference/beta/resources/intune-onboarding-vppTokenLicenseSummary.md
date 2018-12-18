---
title: vppTokenLicenseSummary リソースの種類
description: トークンで指定されたアプリケーションのライセンスの概要です。
author: tfitzmac
ms.openlocfilehash: 7847c6265ed526d50215567918698c7732adf947
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27319979"
---
# <a name="vpptokenlicensesummary-resource-type"></a><span data-ttu-id="b2f1a-103">vppTokenLicenseSummary リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b2f1a-103">vppTokenLicenseSummary resource type</span></span>

> <span data-ttu-id="b2f1a-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="b2f1a-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b2f1a-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b2f1a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b2f1a-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="b2f1a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b2f1a-107">トークンで指定されたアプリケーションのライセンスの概要です。</span><span class="sxs-lookup"><span data-stu-id="b2f1a-107">License summary of a given app in a token.</span></span>
## <a name="properties"></a><span data-ttu-id="b2f1a-108">Properties</span><span class="sxs-lookup"><span data-stu-id="b2f1a-108">Properties</span></span>
|<span data-ttu-id="b2f1a-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b2f1a-109">Property</span></span>|<span data-ttu-id="b2f1a-110">種類</span><span class="sxs-lookup"><span data-stu-id="b2f1a-110">Type</span></span>|<span data-ttu-id="b2f1a-111">説明</span><span class="sxs-lookup"><span data-stu-id="b2f1a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b2f1a-112">vppTokenId</span><span class="sxs-lookup"><span data-stu-id="b2f1a-112">vppTokenId</span></span>|<span data-ttu-id="b2f1a-113">String</span><span class="sxs-lookup"><span data-stu-id="b2f1a-113">String</span></span>|<span data-ttu-id="b2f1a-114">VPP トークンの識別子です。</span><span class="sxs-lookup"><span data-stu-id="b2f1a-114">Identifier of the VPP token.</span></span>|
|<span data-ttu-id="b2f1a-115">appleId</span><span class="sxs-lookup"><span data-stu-id="b2f1a-115">appleId</span></span>|<span data-ttu-id="b2f1a-116">String</span><span class="sxs-lookup"><span data-stu-id="b2f1a-116">String</span></span>|<span data-ttu-id="b2f1a-117">特定の Apple ボリューム購入プログラムのトークンに関連付けられている Apple ID。</span><span class="sxs-lookup"><span data-stu-id="b2f1a-117">The Apple Id associated with the given Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="b2f1a-118">organizationName</span><span class="sxs-lookup"><span data-stu-id="b2f1a-118">organizationName</span></span>|<span data-ttu-id="b2f1a-119">String</span><span class="sxs-lookup"><span data-stu-id="b2f1a-119">String</span></span>|<span data-ttu-id="b2f1a-120">Apple ボリューム購入プログラム トークンに関連付けられている組織です。</span><span class="sxs-lookup"><span data-stu-id="b2f1a-120">The organization associated with the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="b2f1a-121">availableLicenseCount</span><span class="sxs-lookup"><span data-stu-id="b2f1a-121">availableLicenseCount</span></span>|<span data-ttu-id="b2f1a-122">Int32</span><span class="sxs-lookup"><span data-stu-id="b2f1a-122">Int32</span></span>|<span data-ttu-id="b2f1a-123">VPP のライセンスが使用可能な数です。</span><span class="sxs-lookup"><span data-stu-id="b2f1a-123">The number of VPP licenses available.</span></span>|
|<span data-ttu-id="b2f1a-124">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="b2f1a-124">usedLicenseCount</span></span>|<span data-ttu-id="b2f1a-125">Int32</span><span class="sxs-lookup"><span data-stu-id="b2f1a-125">Int32</span></span>|<span data-ttu-id="b2f1a-126">使用中の VPP ライセンスの数。</span><span class="sxs-lookup"><span data-stu-id="b2f1a-126">The number of VPP licenses in use.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b2f1a-127">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="b2f1a-127">Relationships</span></span>
<span data-ttu-id="b2f1a-128">なし</span><span class="sxs-lookup"><span data-stu-id="b2f1a-128">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="b2f1a-129">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b2f1a-129">JSON Representation</span></span>
<span data-ttu-id="b2f1a-130">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="b2f1a-130">Here is a JSON representation of the resource.</span></span>
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





