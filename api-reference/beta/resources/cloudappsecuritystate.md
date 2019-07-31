---
title: cloudAppSecurityState リソースの種類
description: クラウドアプリケーション (destinationServiceName、destinationServiceIp) に関するステートフルな情報を含みます。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 515c567c2360d0d37ddcba6c805f6723312b8030
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36012927"
---
# <a name="cloudappsecuritystate-resource-type"></a><span data-ttu-id="33efb-103">cloudAppSecurityState リソースの種類</span><span class="sxs-lookup"><span data-stu-id="33efb-103">cloudAppSecurityState resource type</span></span>

<span data-ttu-id="33efb-104">クラウドアプリケーション (destinationServiceName、destinationServiceIp) に関するステートフルな情報を含みます。</span><span class="sxs-lookup"><span data-stu-id="33efb-104">Contains stateful information about the cloud application (destinationServiceName, destinationServiceIp).</span></span>

## <a name="properties"></a><span data-ttu-id="33efb-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="33efb-105">Properties</span></span>

| <span data-ttu-id="33efb-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="33efb-106">Property</span></span>     | <span data-ttu-id="33efb-107">型</span><span class="sxs-lookup"><span data-stu-id="33efb-107">Type</span></span>        | <span data-ttu-id="33efb-108">説明</span><span class="sxs-lookup"><span data-stu-id="33efb-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="33efb-109">destinationServiceIp</span><span class="sxs-lookup"><span data-stu-id="33efb-109">destinationServiceIp</span></span>|<span data-ttu-id="33efb-110">String</span><span class="sxs-lookup"><span data-stu-id="33efb-110">String</span></span>|<span data-ttu-id="33efb-111">クラウドアプリケーション/サービスへの接続の宛先 IP アドレス。</span><span class="sxs-lookup"><span data-stu-id="33efb-111">Destination IP Address of the connection to the cloud application/service.</span></span>|
|<span data-ttu-id="33efb-112">destinationServiceName</span><span class="sxs-lookup"><span data-stu-id="33efb-112">destinationServiceName</span></span>|<span data-ttu-id="33efb-113">String</span><span class="sxs-lookup"><span data-stu-id="33efb-113">String</span></span>|<span data-ttu-id="33efb-114">クラウドアプリケーション/サービス名 ("Salesforce"、"DropBox" など)。</span><span class="sxs-lookup"><span data-stu-id="33efb-114">Cloud application/service name (for example "Salesforce", "DropBox", etc.).</span></span>|
|<span data-ttu-id="33efb-115">riskScore</span><span class="sxs-lookup"><span data-stu-id="33efb-115">riskScore</span></span>|<span data-ttu-id="33efb-116">String</span><span class="sxs-lookup"><span data-stu-id="33efb-116">String</span></span>|<span data-ttu-id="33efb-117">プロバイダーが生成/計算する、クラウドアプリケーション/サービスのリスクスコア。</span><span class="sxs-lookup"><span data-stu-id="33efb-117">Provider-generated/calculated risk score of the Cloud Application/Service.</span></span> <span data-ttu-id="33efb-118">推奨値の範囲0-1。パーセンテージに相当します。</span><span class="sxs-lookup"><span data-stu-id="33efb-118">Recommended value range of 0-1, which equates to a percentage.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="33efb-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="33efb-119">JSON representation</span></span>

<span data-ttu-id="33efb-120">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="33efb-120">The following is a JSON representation of the resource.</span></span>

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
