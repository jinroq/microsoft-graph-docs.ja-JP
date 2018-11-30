---
title: securityVendorInformation リソースの種類
description: " subProvider AppLocker を =)。"
ms.openlocfilehash: 0eef5b1d53f4b7b61af0ccede6e02ffc7bdf76ab
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27023135"
---
# <a name="securityvendorinformation-resource-type"></a><span data-ttu-id="e9983-103">securityVendorInformation リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e9983-103">securityVendorInformation resource type</span></span>

<span data-ttu-id="e9983-104">セキュリティ製品やサービスの仕入先、プロバイダー、および subprovider の詳細が含まれています (たとえば、ベンダー = Microsoft; プロバイダー = Windows Defender の分析ツールです。 subProvider AppLocker を =)。</span><span class="sxs-lookup"><span data-stu-id="e9983-104">Contains details about the security product/service vendor, provider, and subprovider (for example, vendor=Microsoft; provider=Windows Defender ATP; subProvider=AppLocker).</span></span>

## <a name="properties"></a><span data-ttu-id="e9983-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e9983-105">Properties</span></span>

| <span data-ttu-id="e9983-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e9983-106">Property</span></span>   | <span data-ttu-id="e9983-107">型</span><span class="sxs-lookup"><span data-stu-id="e9983-107">Type</span></span>|<span data-ttu-id="e9983-108">説明</span><span class="sxs-lookup"><span data-stu-id="e9983-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e9983-109">プロバイダー</span><span class="sxs-lookup"><span data-stu-id="e9983-109">provider</span></span> |<span data-ttu-id="e9983-110">String</span><span class="sxs-lookup"><span data-stu-id="e9983-110">String</span></span>|<span data-ttu-id="e9983-111">特定のプロバイダー (製品やサービスの仕入先会社ではありません)。たとえば、WindowsDefenderATP です。</span><span class="sxs-lookup"><span data-stu-id="e9983-111">Specific provider (product/service - not vendor company); for example, WindowsDefenderATP.</span></span>|
|<span data-ttu-id="e9983-112">providerVersion</span><span class="sxs-lookup"><span data-stu-id="e9983-112">providerVersion</span></span>|<span data-ttu-id="e9983-113">String</span><span class="sxs-lookup"><span data-stu-id="e9983-113">String</span></span>|<span data-ttu-id="e9983-114">Subprovider、それが存在する場合は、アラートを生成したプロバイダーのバージョンです。</span><span class="sxs-lookup"><span data-stu-id="e9983-114">Version of the provider or subprovider, if it exists, that generated the alert.</span></span> <span data-ttu-id="e9983-115">*Required*</span><span class="sxs-lookup"><span data-stu-id="e9983-115">*Required*</span></span>|
|<span data-ttu-id="e9983-116">subProvider</span><span class="sxs-lookup"><span data-stu-id="e9983-116">subProvider</span></span>|<span data-ttu-id="e9983-117">String</span><span class="sxs-lookup"><span data-stu-id="e9983-117">String</span></span>|<span data-ttu-id="e9983-118">特定の subprovider 下にあるプロバイダーを集約)。たとえば、WindowsDefenderATP.SmartScreen です。</span><span class="sxs-lookup"><span data-stu-id="e9983-118">Specific subprovider (under aggregating provider); for example, WindowsDefenderATP.SmartScreen.</span></span>|
|<span data-ttu-id="e9983-119">仕入先</span><span class="sxs-lookup"><span data-stu-id="e9983-119">vendor</span></span> |<span data-ttu-id="e9983-120">String</span><span class="sxs-lookup"><span data-stu-id="e9983-120">String</span></span>|<span data-ttu-id="e9983-121">アラート ベンダー (マイクロソフトでは、Dell の FireEye など) の名前。</span><span class="sxs-lookup"><span data-stu-id="e9983-121">Name of the alert vendor (for example, Microsoft, Dell, FireEye).</span></span> <span data-ttu-id="e9983-122">*Required*</span><span class="sxs-lookup"><span data-stu-id="e9983-122">*Required*</span></span>|


## <a name="json-representation"></a><span data-ttu-id="e9983-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e9983-123">JSON representation</span></span>

<span data-ttu-id="e9983-124">次は、リソースの JSON 表現です。</span><span class="sxs-lookup"><span data-stu-id="e9983-124">The folllowing is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.securityVendorInformation"
}-->

```json
{
  "provider": "String",
  "providerVersion": "String",
  "subProvider": "String",
  "vendor": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "securityVendorInformation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
