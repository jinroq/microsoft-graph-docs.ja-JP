---
title: embeddedSIMActivationCode リソースの種類
description: 携帯電話会社から提供された、埋め込まれた SIM ライセンス認証コード。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 955dccb226332b297e30c4d40768f84936b04dbe
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30145228"
---
# <a name="embeddedsimactivationcode-resource-type"></a><span data-ttu-id="a92ca-103">embeddedSIMActivationCode リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a92ca-103">embeddedSIMActivationCode resource type</span></span>

> <span data-ttu-id="a92ca-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a92ca-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a92ca-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="a92ca-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a92ca-106">携帯電話会社から提供された、埋め込まれた SIM ライセンス認証コード。</span><span class="sxs-lookup"><span data-stu-id="a92ca-106">The embedded SIM activation code as provided by the mobile operator.</span></span>

## <a name="properties"></a><span data-ttu-id="a92ca-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a92ca-107">Properties</span></span>
|<span data-ttu-id="a92ca-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a92ca-108">Property</span></span>|<span data-ttu-id="a92ca-109">型</span><span class="sxs-lookup"><span data-stu-id="a92ca-109">Type</span></span>|<span data-ttu-id="a92ca-110">説明</span><span class="sxs-lookup"><span data-stu-id="a92ca-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a92ca-111">integratedCircuitCardIdentifier</span><span class="sxs-lookup"><span data-stu-id="a92ca-111">integratedCircuitCardIdentifier</span></span>|<span data-ttu-id="a92ca-112">String</span><span class="sxs-lookup"><span data-stu-id="a92ca-112">String</span></span>|<span data-ttu-id="a92ca-113">携帯電話会社が提供する、この組み込み SIM アクティブ化コードの ic カード識別子 (ICCID)。</span><span class="sxs-lookup"><span data-stu-id="a92ca-113">The Integrated Circuit Card Identifier (ICCID) for this embedded SIM activation code as provided by the mobile operator.</span></span>
<span data-ttu-id="a92ca-114">入力は、次の正規表現に一致して\[いる\]{19}\[必要\]があります。 ' ^ 0-9 0-9 ? $ '。</span><span class="sxs-lookup"><span data-stu-id="a92ca-114">The input must match the following regular expression: '^\[0-9\]{19}\[0-9\]?$'.</span></span>|
|<span data-ttu-id="a92ca-115">matchingIdentifier</span><span class="sxs-lookup"><span data-stu-id="a92ca-115">matchingIdentifier</span></span>|<span data-ttu-id="a92ca-116">String</span><span class="sxs-lookup"><span data-stu-id="a92ca-116">String</span></span>|<span data-ttu-id="a92ca-117">gsma Association MatchingIdentifier (MatchingID) セクション4.1 で指定されているように、()。</span><span class="sxs-lookup"><span data-stu-id="a92ca-117">The MatchingIdentifier (MatchingID) as specified in the GSMA Association SGP.22 RSP Technical Specification section 4.1.</span></span>
<span data-ttu-id="a92ca-118">入力は、次の正規表現に一致する必要\[があります: ' ^ zA\-\]-Z0-9 \* $ '。</span><span class="sxs-lookup"><span data-stu-id="a92ca-118">The input must match the following regular expression: '^\[a-zA-Z0-9\-\]\*$'.</span></span>|
|<span data-ttu-id="a92ca-119">smdpPlusServerAddress</span><span class="sxs-lookup"><span data-stu-id="a92ca-119">smdpPlusServerAddress</span></span>|<span data-ttu-id="a92ca-120">String</span><span class="sxs-lookup"><span data-stu-id="a92ca-120">String</span></span>|<span data-ttu-id="a92ca-121">GSM Association SPG .22 RSP Technical 仕様で指定されているとおりに、SM-DP + サーバーの完全修飾ドメイン名。</span><span class="sxs-lookup"><span data-stu-id="a92ca-121">The fully qualified domain name of the SM-DP+ server as specified in the GSM Association SPG .22 RSP Technical Specification.</span></span>
<span data-ttu-id="a92ca-122">入力は、次の正規表現に一致している\[必要があります: ' ^\](zA-\[Z0-\]9 +)\.\*) +\[a-zA-Z\]{2,}$ '。</span><span class="sxs-lookup"><span data-stu-id="a92ca-122">The input must match the following regular expression: '^(\[a-zA-Z0-9\]+(-\[a-zA-Z0-9\]+)\*\.)+\[a-zA-Z\]{2,}$'.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a92ca-123">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="a92ca-123">Relationships</span></span>
<span data-ttu-id="a92ca-124">なし</span><span class="sxs-lookup"><span data-stu-id="a92ca-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a92ca-125">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a92ca-125">JSON Representation</span></span>
<span data-ttu-id="a92ca-126">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="a92ca-126">Here is a JSON representation of the resource.</span></span>
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




