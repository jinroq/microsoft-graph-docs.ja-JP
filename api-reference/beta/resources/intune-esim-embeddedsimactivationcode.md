---
title: embeddedSIMActivationCode リソースの種類
description: 携帯電話会社で提供される、埋め込みコードの SIM のアクティブ化します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 74f1725ab8f12cb103144dc1897e9bf965c5361b
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29422468"
---
# <a name="embeddedsimactivationcode-resource-type"></a><span data-ttu-id="f8e41-103">embeddedSIMActivationCode リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f8e41-103">embeddedSIMActivationCode resource type</span></span>

> <span data-ttu-id="f8e41-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="f8e41-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="f8e41-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f8e41-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f8e41-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="f8e41-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f8e41-107">携帯電話会社で提供される、埋め込みコードの SIM のアクティブ化します。</span><span class="sxs-lookup"><span data-stu-id="f8e41-107">The embedded SIM activation code as provided by the mobile operator.</span></span>

## <a name="properties"></a><span data-ttu-id="f8e41-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f8e41-108">Properties</span></span>
|<span data-ttu-id="f8e41-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f8e41-109">Property</span></span>|<span data-ttu-id="f8e41-110">型</span><span class="sxs-lookup"><span data-stu-id="f8e41-110">Type</span></span>|<span data-ttu-id="f8e41-111">説明</span><span class="sxs-lookup"><span data-stu-id="f8e41-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f8e41-112">integratedCircuitCardIdentifier</span><span class="sxs-lookup"><span data-stu-id="f8e41-112">integratedCircuitCardIdentifier</span></span>|<span data-ttu-id="f8e41-113">String</span><span class="sxs-lookup"><span data-stu-id="f8e41-113">String</span></span>|<span data-ttu-id="f8e41-114">この集積回路カードの識別子 (ICCID) では、携帯電話会社によって提供されると、SIM の有効化コードが埋め込まれています。</span><span class="sxs-lookup"><span data-stu-id="f8e41-114">The Integrated Circuit Card Identifier (ICCID) for this embedded SIM activation code as provided by the mobile operator.</span></span>
<span data-ttu-id="f8e41-115">入力が次の正規表現に一致する必要があります: '^\[0-9\]{19}\[0-9\]?$' です。</span><span class="sxs-lookup"><span data-stu-id="f8e41-115">The input must match the following regular expression: '^\[0-9\]{19}\[0-9\]?$'.</span></span>|
|<span data-ttu-id="f8e41-116">matchingIdentifier</span><span class="sxs-lookup"><span data-stu-id="f8e41-116">matchingIdentifier</span></span>|<span data-ttu-id="f8e41-117">String</span><span class="sxs-lookup"><span data-stu-id="f8e41-117">String</span></span>|<span data-ttu-id="f8e41-118">GSMA アソシエーション SGP.22 RSP 技術仕様セクション 4.1 で指定されている MatchingIdentifier (MatchingID)。</span><span class="sxs-lookup"><span data-stu-id="f8e41-118">The MatchingIdentifier (MatchingID) as specified in the GSMA Association SGP.22 RSP Technical Specification section 4.1.</span></span>
<span data-ttu-id="f8e41-119">入力が次の正規表現に一致する必要があります: ' ^\[a-zA-Z0-9\-\]\* $' です。</span><span class="sxs-lookup"><span data-stu-id="f8e41-119">The input must match the following regular expression: '^\[a-zA-Z0-9\-\]\*$'.</span></span>|
|<span data-ttu-id="f8e41-120">smdpPlusServerAddress</span><span class="sxs-lookup"><span data-stu-id="f8e41-120">smdpPlusServerAddress</span></span>|<span data-ttu-id="f8e41-121">String</span><span class="sxs-lookup"><span data-stu-id="f8e41-121">String</span></span>|<span data-ttu-id="f8e41-122">SM の完全修飾ドメイン名-DP + GSM 関連 SPG.22 RSP の技術的な仕様で指定されているサーバーです。</span><span class="sxs-lookup"><span data-stu-id="f8e41-122">The fully qualified domain name of the SM-DP+ server as specified in the GSM Association SPG .22 RSP Technical Specification.</span></span>
<span data-ttu-id="f8e41-123">入力が次の正規表現に一致する必要があります: ' ^ (\[、-zA-Z0-9\]+(-\[a-zA-Z0-9\]+) \*\.) +\[a, A-Z\]{2,}$' です。</span><span class="sxs-lookup"><span data-stu-id="f8e41-123">The input must match the following regular expression: '^(\[a-zA-Z0-9\]+(-\[a-zA-Z0-9\]+)\*\.)+\[a-zA-Z\]{2,}$'.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f8e41-124">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="f8e41-124">Relationships</span></span>
<span data-ttu-id="f8e41-125">なし</span><span class="sxs-lookup"><span data-stu-id="f8e41-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f8e41-126">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f8e41-126">JSON Representation</span></span>
<span data-ttu-id="f8e41-127">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="f8e41-127">Here is a JSON representation of the resource.</span></span>
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




