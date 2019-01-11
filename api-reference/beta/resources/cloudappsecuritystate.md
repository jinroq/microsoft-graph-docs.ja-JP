---
title: cloudAppSecurityState リソースの種類
description: ステートフル (destinationServiceName、destinationServiceIp) は、クラウド アプリケーションについてを説明します。
localization_priority: Normal
ms.openlocfilehash: ff76adf1d3879c3dac3f19ae122d82c9523d5193
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27850870"
---
# <a name="cloudappsecuritystate-resource-type"></a><span data-ttu-id="eda4a-103">cloudAppSecurityState リソースの種類</span><span class="sxs-lookup"><span data-stu-id="eda4a-103">cloudAppSecurityState resource type</span></span>

<span data-ttu-id="eda4a-104">ステートフル (destinationServiceName、destinationServiceIp) は、クラウド アプリケーションについてを説明します。</span><span class="sxs-lookup"><span data-stu-id="eda4a-104">Contains stateful information about the cloud application (destinationServiceName, destinationServiceIp).</span></span>

## <a name="properties"></a><span data-ttu-id="eda4a-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="eda4a-105">Properties</span></span>

| <span data-ttu-id="eda4a-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="eda4a-106">Property</span></span>     | <span data-ttu-id="eda4a-107">種類</span><span class="sxs-lookup"><span data-stu-id="eda4a-107">Type</span></span>        | <span data-ttu-id="eda4a-108">説明</span><span class="sxs-lookup"><span data-stu-id="eda4a-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="eda4a-109">destinationServiceIp</span><span class="sxs-lookup"><span data-stu-id="eda4a-109">destinationServiceIp</span></span>|<span data-ttu-id="eda4a-110">String</span><span class="sxs-lookup"><span data-stu-id="eda4a-110">String</span></span>|<span data-ttu-id="eda4a-111">クラウド アプリケーションやサービスへの接続の宛先の IP アドレス。</span><span class="sxs-lookup"><span data-stu-id="eda4a-111">Destination IP Address of the connection to the cloud application/service.</span></span>|
|<span data-ttu-id="eda4a-112">destinationServiceName</span><span class="sxs-lookup"><span data-stu-id="eda4a-112">destinationServiceName</span></span>|<span data-ttu-id="eda4a-113">String</span><span class="sxs-lookup"><span data-stu-id="eda4a-113">String</span></span>|<span data-ttu-id="eda4a-114">クラウド アプリケーションとサービスの名前 (たとえば「Salesforce」、「ドロップ ボックス」など)。</span><span class="sxs-lookup"><span data-stu-id="eda4a-114">Cloud application/service name (for example "Salesforce", "DropBox", etc.).</span></span>|
|<span data-ttu-id="eda4a-115">riskScore</span><span class="sxs-lookup"><span data-stu-id="eda4a-115">riskScore</span></span>|<span data-ttu-id="eda4a-116">String</span><span class="sxs-lookup"><span data-stu-id="eda4a-116">String</span></span>|<span data-ttu-id="eda4a-117">プロバイダーによって生成されると計算されるリスク スコア クラウド アプリケーションとサービスのです。</span><span class="sxs-lookup"><span data-stu-id="eda4a-117">Provider-generated/calculated risk score of the Cloud Application/Service.</span></span> <span data-ttu-id="eda4a-118">0 - 1 パーセントに相当する値の範囲をお勧めします。</span><span class="sxs-lookup"><span data-stu-id="eda4a-118">Recommended value range of 0-1, which equates to a percentage.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="eda4a-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="eda4a-119">JSON representation</span></span>

<span data-ttu-id="eda4a-120">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="eda4a-120">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.cloudAppSecurityState"
}-->

```json
{
  "destinationServiceIp": "String",
  "destinationServiceName": "String",
  "riskScore": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "cloudAppSecurityState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
