---
title: cloudappsecuritystate リソースの種類
description: クラウドアプリケーション (destinationservicename、destinationserviceip) に関するステートフルな情報を含みます。
localization_priority: Normal
ms.openlocfilehash: ff76adf1d3879c3dac3f19ae122d82c9523d5193
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32460661"
---
# <a name="cloudappsecuritystate-resource-type"></a><span data-ttu-id="5c318-103">cloudappsecuritystate リソースの種類</span><span class="sxs-lookup"><span data-stu-id="5c318-103">cloudAppSecurityState resource type</span></span>

<span data-ttu-id="5c318-104">クラウドアプリケーション (destinationservicename、destinationserviceip) に関するステートフルな情報を含みます。</span><span class="sxs-lookup"><span data-stu-id="5c318-104">Contains stateful information about the cloud application (destinationServiceName, destinationServiceIp).</span></span>

## <a name="properties"></a><span data-ttu-id="5c318-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5c318-105">Properties</span></span>

| <span data-ttu-id="5c318-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5c318-106">Property</span></span>     | <span data-ttu-id="5c318-107">型</span><span class="sxs-lookup"><span data-stu-id="5c318-107">Type</span></span>        | <span data-ttu-id="5c318-108">説明</span><span class="sxs-lookup"><span data-stu-id="5c318-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="5c318-109">destinationserviceip</span><span class="sxs-lookup"><span data-stu-id="5c318-109">destinationServiceIp</span></span>|<span data-ttu-id="5c318-110">String</span><span class="sxs-lookup"><span data-stu-id="5c318-110">String</span></span>|<span data-ttu-id="5c318-111">クラウドアプリケーション/サービスへの接続の宛先 IP アドレス。</span><span class="sxs-lookup"><span data-stu-id="5c318-111">Destination IP Address of the connection to the cloud application/service.</span></span>|
|<span data-ttu-id="5c318-112">destinationservicename</span><span class="sxs-lookup"><span data-stu-id="5c318-112">destinationServiceName</span></span>|<span data-ttu-id="5c318-113">String</span><span class="sxs-lookup"><span data-stu-id="5c318-113">String</span></span>|<span data-ttu-id="5c318-114">クラウドアプリケーション/サービス名 ("Salesforce"、"DropBox" など)。</span><span class="sxs-lookup"><span data-stu-id="5c318-114">Cloud application/service name (for example "Salesforce", "DropBox", etc.).</span></span>|
|<span data-ttu-id="5c318-115">riskScore</span><span class="sxs-lookup"><span data-stu-id="5c318-115">riskScore</span></span>|<span data-ttu-id="5c318-116">String</span><span class="sxs-lookup"><span data-stu-id="5c318-116">String</span></span>|<span data-ttu-id="5c318-117">プロバイダーが生成/計算する、クラウドアプリケーション/サービスのリスクスコア。</span><span class="sxs-lookup"><span data-stu-id="5c318-117">Provider-generated/calculated risk score of the Cloud Application/Service.</span></span> <span data-ttu-id="5c318-118">推奨値の範囲0-1。パーセンテージに相当します。</span><span class="sxs-lookup"><span data-stu-id="5c318-118">Recommended value range of 0-1, which equates to a percentage.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5c318-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="5c318-119">JSON representation</span></span>

<span data-ttu-id="5c318-120">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="5c318-120">The following is a JSON representation of the resource.</span></span>

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
