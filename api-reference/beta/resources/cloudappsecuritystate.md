---
title: cloudAppSecurityState リソースの種類
description: ステートフル (destinationServiceName、destinationServiceIp) は、クラウド アプリケーションについてを説明します。
ms.openlocfilehash: 915044c3084e3d9a9435d602ecc7ec809d2168f2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27070902"
---
# <a name="cloudappsecuritystate-resource-type"></a><span data-ttu-id="48667-103">cloudAppSecurityState リソースの種類</span><span class="sxs-lookup"><span data-stu-id="48667-103">cloudAppSecurityState resource type</span></span>

<span data-ttu-id="48667-104">ステートフル (destinationServiceName、destinationServiceIp) は、クラウド アプリケーションについてを説明します。</span><span class="sxs-lookup"><span data-stu-id="48667-104">Contains stateful information about the cloud application (destinationServiceName, destinationServiceIp).</span></span>

## <a name="properties"></a><span data-ttu-id="48667-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="48667-105">Properties</span></span>

| <span data-ttu-id="48667-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="48667-106">Property</span></span>     | <span data-ttu-id="48667-107">型</span><span class="sxs-lookup"><span data-stu-id="48667-107">Type</span></span>        | <span data-ttu-id="48667-108">説明</span><span class="sxs-lookup"><span data-stu-id="48667-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="48667-109">destinationServiceIp</span><span class="sxs-lookup"><span data-stu-id="48667-109">destinationServiceIp</span></span>|<span data-ttu-id="48667-110">String</span><span class="sxs-lookup"><span data-stu-id="48667-110">String</span></span>|<span data-ttu-id="48667-111">クラウド アプリケーションやサービスへの接続の宛先の IP アドレス。</span><span class="sxs-lookup"><span data-stu-id="48667-111">Destination IP Address of the connection to the cloud application/service.</span></span>|
|<span data-ttu-id="48667-112">destinationServiceName</span><span class="sxs-lookup"><span data-stu-id="48667-112">destinationServiceName</span></span>|<span data-ttu-id="48667-113">String</span><span class="sxs-lookup"><span data-stu-id="48667-113">String</span></span>|<span data-ttu-id="48667-114">クラウド アプリケーションとサービスの名前 (たとえば「Salesforce」、「ドロップ ボックス」など)。</span><span class="sxs-lookup"><span data-stu-id="48667-114">Cloud application/service name (for example "Salesforce", "DropBox", etc.).</span></span>|
|<span data-ttu-id="48667-115">riskScore</span><span class="sxs-lookup"><span data-stu-id="48667-115">riskScore</span></span>|<span data-ttu-id="48667-116">String</span><span class="sxs-lookup"><span data-stu-id="48667-116">String</span></span>|<span data-ttu-id="48667-117">プロバイダーによって生成されると計算されるリスク スコア クラウド アプリケーションとサービスのです。</span><span class="sxs-lookup"><span data-stu-id="48667-117">Provider-generated/calculated risk score of the Cloud Application/Service.</span></span> <span data-ttu-id="48667-118">0 - 1 パーセントに相当する値の範囲をお勧めします。</span><span class="sxs-lookup"><span data-stu-id="48667-118">Recommended value range of 0-1, which equates to a percentage.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="48667-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="48667-119">JSON representation</span></span>

<span data-ttu-id="48667-120">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="48667-120">The following is a JSON representation of the resource.</span></span>

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