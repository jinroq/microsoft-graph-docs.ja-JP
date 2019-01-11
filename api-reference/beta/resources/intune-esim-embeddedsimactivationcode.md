---
title: embeddedSIMActivationCode リソースの種類
description: 携帯電話会社で提供される、埋め込みコードの SIM のアクティブ化します。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 41976b92cfe6b6f695631dbd6c0d928c6ae99271
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27878065"
---
# <a name="embeddedsimactivationcode-resource-type"></a><span data-ttu-id="9b739-103">embeddedSIMActivationCode リソースの種類</span><span class="sxs-lookup"><span data-stu-id="9b739-103">embeddedSIMActivationCode resource type</span></span>

> <span data-ttu-id="9b739-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="9b739-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9b739-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9b739-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9b739-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="9b739-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9b739-107">携帯電話会社で提供される、埋め込みコードの SIM のアクティブ化します。</span><span class="sxs-lookup"><span data-stu-id="9b739-107">The embedded SIM activation code as provided by the mobile operator.</span></span>
## <a name="properties"></a><span data-ttu-id="9b739-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9b739-108">Properties</span></span>
|<span data-ttu-id="9b739-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9b739-109">Property</span></span>|<span data-ttu-id="9b739-110">種類</span><span class="sxs-lookup"><span data-stu-id="9b739-110">Type</span></span>|<span data-ttu-id="9b739-111">説明</span><span class="sxs-lookup"><span data-stu-id="9b739-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9b739-112">integratedCircuitCardIdentifier</span><span class="sxs-lookup"><span data-stu-id="9b739-112">integratedCircuitCardIdentifier</span></span>|<span data-ttu-id="9b739-113">String</span><span class="sxs-lookup"><span data-stu-id="9b739-113">String</span></span>|<span data-ttu-id="9b739-114">この集積回路カードの識別子 (ICCID) では、携帯電話会社によって提供されると、SIM の有効化コードが埋め込まれています。</span><span class="sxs-lookup"><span data-stu-id="9b739-114">The Integrated Circuit Card Identifier (ICCID) for this embedded SIM activation code as provided by the mobile operator.</span></span>
<span data-ttu-id="9b739-115">入力が次の正規表現に一致する必要があります: '^\[0-9\]{19}\[0-9\]?$' です。</span><span class="sxs-lookup"><span data-stu-id="9b739-115">The input must match the following regular expression: '^\[0-9\]{19}\[0-9\]?$'.</span></span>|
|<span data-ttu-id="9b739-116">matchingIdentifier</span><span class="sxs-lookup"><span data-stu-id="9b739-116">matchingIdentifier</span></span>|<span data-ttu-id="9b739-117">String</span><span class="sxs-lookup"><span data-stu-id="9b739-117">String</span></span>|<span data-ttu-id="9b739-118">GSMA アソシエーション SGP.22 RSP 技術仕様セクション 4.1 で指定されている MatchingIdentifier (MatchingID)。</span><span class="sxs-lookup"><span data-stu-id="9b739-118">The MatchingIdentifier (MatchingID) as specified in the GSMA Association SGP.22 RSP Technical Specification section 4.1.</span></span>
<span data-ttu-id="9b739-119">入力が次の正規表現に一致する必要があります: ' ^\[a-zA-Z0-9\-\]\* $' です。</span><span class="sxs-lookup"><span data-stu-id="9b739-119">The input must match the following regular expression: '^\[a-zA-Z0-9\-\]\*$'.</span></span>|
|<span data-ttu-id="9b739-120">smdpPlusServerAddress</span><span class="sxs-lookup"><span data-stu-id="9b739-120">smdpPlusServerAddress</span></span>|<span data-ttu-id="9b739-121">String</span><span class="sxs-lookup"><span data-stu-id="9b739-121">String</span></span>|<span data-ttu-id="9b739-122">SM の完全修飾ドメイン名-DP + GSM 関連 SPG.22 RSP の技術的な仕様で指定されているサーバーです。</span><span class="sxs-lookup"><span data-stu-id="9b739-122">The fully qualified domain name of the SM-DP+ server as specified in the GSM Association SPG .22 RSP Technical Specification.</span></span>
<span data-ttu-id="9b739-123">入力が次の正規表現に一致する必要があります: ' ^ (\[、-zA-Z0-9\]+(-\[a-zA-Z0-9\]+) \*\.) +\[a, A-Z\]{2,}$' です。</span><span class="sxs-lookup"><span data-stu-id="9b739-123">The input must match the following regular expression: '^(\[a-zA-Z0-9\]+(-\[a-zA-Z0-9\]+)\*\.)+\[a-zA-Z\]{2,}$'.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9b739-124">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="9b739-124">Relationships</span></span>
<span data-ttu-id="9b739-125">なし</span><span class="sxs-lookup"><span data-stu-id="9b739-125">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="9b739-126">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="9b739-126">JSON Representation</span></span>
<span data-ttu-id="9b739-127">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="9b739-127">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.embeddedSIMActivationCode"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.embeddedSIMActivationCode",
  "integratedCircuitCardIdentifier": "String",
  "matchingIdentifier": "String",
  "smdpPlusServerAddress": "String"
}
```





