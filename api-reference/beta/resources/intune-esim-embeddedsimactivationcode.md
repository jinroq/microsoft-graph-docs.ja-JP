---
title: embeddedSIMActivationCode リソースの種類
description: 携帯電話会社から提供された、埋め込まれた SIM ライセンス認証コード。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c96bc6530de0e8e6d1fde95fa71ffb6f1bdedb18
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34994882"
---
# <a name="embeddedsimactivationcode-resource-type"></a><span data-ttu-id="fabba-103">embeddedSIMActivationCode リソースの種類</span><span class="sxs-lookup"><span data-stu-id="fabba-103">embeddedSIMActivationCode resource type</span></span>

> <span data-ttu-id="fabba-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fabba-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fabba-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="fabba-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fabba-106">携帯電話会社から提供された、埋め込まれた SIM ライセンス認証コード。</span><span class="sxs-lookup"><span data-stu-id="fabba-106">The embedded SIM activation code as provided by the mobile operator.</span></span>

## <a name="properties"></a><span data-ttu-id="fabba-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fabba-107">Properties</span></span>
|<span data-ttu-id="fabba-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fabba-108">Property</span></span>|<span data-ttu-id="fabba-109">型</span><span class="sxs-lookup"><span data-stu-id="fabba-109">Type</span></span>|<span data-ttu-id="fabba-110">説明</span><span class="sxs-lookup"><span data-stu-id="fabba-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fabba-111">integratedCircuitCardIdentifier</span><span class="sxs-lookup"><span data-stu-id="fabba-111">integratedCircuitCardIdentifier</span></span>|<span data-ttu-id="fabba-112">String</span><span class="sxs-lookup"><span data-stu-id="fabba-112">String</span></span>|<span data-ttu-id="fabba-113">携帯電話会社が提供する、この組み込み SIM アクティブ化コードの Ic カード識別子 (ICCID)。</span><span class="sxs-lookup"><span data-stu-id="fabba-113">The Integrated Circuit Card Identifier (ICCID) for this embedded SIM activation code as provided by the mobile operator.</span></span>
<span data-ttu-id="fabba-114">入力は、次の正規表現に一致して\[いる\]{19}\[必要\]があります: ' ^ 0-9 0-9? $ '。</span><span class="sxs-lookup"><span data-stu-id="fabba-114">The input must match the following regular expression: '^\[0-9\]{19}\[0-9\]?$'.</span></span>|
|<span data-ttu-id="fabba-115">matchingIdentifier</span><span class="sxs-lookup"><span data-stu-id="fabba-115">matchingIdentifier</span></span>|<span data-ttu-id="fabba-116">String</span><span class="sxs-lookup"><span data-stu-id="fabba-116">String</span></span>|<span data-ttu-id="fabba-117">GSMA Association MatchingIdentifier (MatchingID) セクション4.1 で指定されているように、()。</span><span class="sxs-lookup"><span data-stu-id="fabba-117">The MatchingIdentifier (MatchingID) as specified in the GSMA Association SGP.22 RSP Technical Specification section 4.1.</span></span>
<span data-ttu-id="fabba-118">入力は、次の正規表現に一致する必要\[があります: ' ^ ZA\-\]-Z0-9 \* $ '。</span><span class="sxs-lookup"><span data-stu-id="fabba-118">The input must match the following regular expression: '^\[a-zA-Z0-9\-\]\*$'.</span></span>|
|<span data-ttu-id="fabba-119">smdpPlusServerAddress</span><span class="sxs-lookup"><span data-stu-id="fabba-119">smdpPlusServerAddress</span></span>|<span data-ttu-id="fabba-120">String</span><span class="sxs-lookup"><span data-stu-id="fabba-120">String</span></span>|<span data-ttu-id="fabba-121">GSM Association SPG .22 RSP Technical 仕様で指定されているとおりに、SM-DP + サーバーの完全修飾ドメイン名。</span><span class="sxs-lookup"><span data-stu-id="fabba-121">The fully qualified domain name of the SM-DP+ server as specified in the GSM Association SPG .22 RSP Technical Specification.</span></span>
<span data-ttu-id="fabba-122">入力は、次の正規表現に一致している\[必要があります: ' ^\](zA-\[Z0-\]9 +)\.\*) +\[a-zA-Z\]{2,}$ '。</span><span class="sxs-lookup"><span data-stu-id="fabba-122">The input must match the following regular expression: '^(\[a-zA-Z0-9\]+(-\[a-zA-Z0-9\]+)\*\.)+\[a-zA-Z\]{2,}$'.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fabba-123">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="fabba-123">Relationships</span></span>
<span data-ttu-id="fabba-124">なし</span><span class="sxs-lookup"><span data-stu-id="fabba-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fabba-125">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="fabba-125">JSON Representation</span></span>
<span data-ttu-id="fabba-126">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="fabba-126">Here is a JSON representation of the resource.</span></span>
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





