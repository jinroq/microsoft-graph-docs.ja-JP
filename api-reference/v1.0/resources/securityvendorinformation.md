---
title: securityVendorInformation リソースの種類
description: " subProvider = AppLocker)。"
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 3fb959da2d6af10632f9113a33eb942492b679ef
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36034427"
---
# <a name="securityvendorinformation-resource-type"></a><span data-ttu-id="998ab-103">securityVendorInformation リソースの種類</span><span class="sxs-lookup"><span data-stu-id="998ab-103">securityVendorInformation resource type</span></span>

<span data-ttu-id="998ab-104">セキュリティ製品/サービスベンダー、プロバイダ、およびサブプロバイダに関する詳細情報が含まれています (たとえば、ベンダー = Microsoft; provider = Windows Defender ATP; subProvider = AppLocker)。</span><span class="sxs-lookup"><span data-stu-id="998ab-104">Contains details about the security product/service vendor, provider, and subprovider (for example, vendor=Microsoft; provider=Windows Defender ATP; subProvider=AppLocker).</span></span>

## <a name="properties"></a><span data-ttu-id="998ab-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="998ab-105">Properties</span></span>

| <span data-ttu-id="998ab-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="998ab-106">Property</span></span>   | <span data-ttu-id="998ab-107">型</span><span class="sxs-lookup"><span data-stu-id="998ab-107">Type</span></span>|<span data-ttu-id="998ab-108">説明</span><span class="sxs-lookup"><span data-stu-id="998ab-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="998ab-109">供給</span><span class="sxs-lookup"><span data-stu-id="998ab-109">provider</span></span> |<span data-ttu-id="998ab-110">String</span><span class="sxs-lookup"><span data-stu-id="998ab-110">String</span></span>|<span data-ttu-id="998ab-111">特定のプロバイダー (製品/サービス-ベンダー会社ではない)。たとえば、WindowsDefenderATP のようになります。</span><span class="sxs-lookup"><span data-stu-id="998ab-111">Specific provider (product/service - not vendor company); for example, WindowsDefenderATP.</span></span>|
|<span data-ttu-id="998ab-112">providerVersion</span><span class="sxs-lookup"><span data-stu-id="998ab-112">providerVersion</span></span>|<span data-ttu-id="998ab-113">String</span><span class="sxs-lookup"><span data-stu-id="998ab-113">String</span></span>|<span data-ttu-id="998ab-114">通知を生成したプロバイダーまたはサブプロバイダのバージョン (存在する場合)。</span><span class="sxs-lookup"><span data-stu-id="998ab-114">Version of the provider or subprovider, if it exists, that generated the alert.</span></span> <span data-ttu-id="998ab-115">*Required*</span><span class="sxs-lookup"><span data-stu-id="998ab-115">*Required*</span></span>|
|<span data-ttu-id="998ab-116">subProvider</span><span class="sxs-lookup"><span data-stu-id="998ab-116">subProvider</span></span>|<span data-ttu-id="998ab-117">String</span><span class="sxs-lookup"><span data-stu-id="998ab-117">String</span></span>|<span data-ttu-id="998ab-118">特定のサブプロバイダ (集計プロバイダーの場合)。たとえば、WindowsDefenderATP。</span><span class="sxs-lookup"><span data-stu-id="998ab-118">Specific subprovider (under aggregating provider); for example, WindowsDefenderATP.SmartScreen.</span></span>|
|<span data-ttu-id="998ab-119">ベンダ</span><span class="sxs-lookup"><span data-stu-id="998ab-119">vendor</span></span> |<span data-ttu-id="998ab-120">String</span><span class="sxs-lookup"><span data-stu-id="998ab-120">String</span></span>|<span data-ttu-id="998ab-121">通知ベンダーの名前 (Microsoft、Dell、焼討アイなど)。</span><span class="sxs-lookup"><span data-stu-id="998ab-121">Name of the alert vendor (for example, Microsoft, Dell, FireEye).</span></span> <span data-ttu-id="998ab-122">*Required*</span><span class="sxs-lookup"><span data-stu-id="998ab-122">*Required*</span></span>|


## <a name="json-representation"></a><span data-ttu-id="998ab-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="998ab-123">JSON representation</span></span>

<span data-ttu-id="998ab-124">Folllowing は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="998ab-124">The folllowing is a JSON representation of the resource.</span></span>
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
