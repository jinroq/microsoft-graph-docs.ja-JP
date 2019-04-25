---
title: securityVendorInformation リソースの種類
description: " subprovider = AppLocker)。"
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: fb5dee36da08332fd5c36f7ee4e578cc9fb7deaa
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32549700"
---
# <a name="securityvendorinformation-resource-type"></a><span data-ttu-id="40e55-103">securityVendorInformation リソースの種類</span><span class="sxs-lookup"><span data-stu-id="40e55-103">securityVendorInformation resource type</span></span>

<span data-ttu-id="40e55-104">セキュリティ製品/サービスベンダー、プロバイダ、およびサブプロバイダに関する詳細情報が含まれています (たとえば、ベンダー = Microsoft; provider = Windows Defender ATP; subprovider = AppLocker)。</span><span class="sxs-lookup"><span data-stu-id="40e55-104">Contains details about the security product/service vendor, provider, and subprovider (for example, vendor=Microsoft; provider=Windows Defender ATP; subProvider=AppLocker).</span></span>

## <a name="properties"></a><span data-ttu-id="40e55-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="40e55-105">Properties</span></span>

| <span data-ttu-id="40e55-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="40e55-106">Property</span></span>   | <span data-ttu-id="40e55-107">型</span><span class="sxs-lookup"><span data-stu-id="40e55-107">Type</span></span>|<span data-ttu-id="40e55-108">説明</span><span class="sxs-lookup"><span data-stu-id="40e55-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="40e55-109">供給</span><span class="sxs-lookup"><span data-stu-id="40e55-109">provider</span></span> |<span data-ttu-id="40e55-110">String</span><span class="sxs-lookup"><span data-stu-id="40e55-110">String</span></span>|<span data-ttu-id="40e55-111">特定のプロバイダー (製品/サービス-ベンダー会社ではない)。たとえば、windowsdefenderatp のようになります。</span><span class="sxs-lookup"><span data-stu-id="40e55-111">Specific provider (product/service - not vendor company); for example, WindowsDefenderATP.</span></span>|
|<span data-ttu-id="40e55-112">providerversion</span><span class="sxs-lookup"><span data-stu-id="40e55-112">providerVersion</span></span>|<span data-ttu-id="40e55-113">String</span><span class="sxs-lookup"><span data-stu-id="40e55-113">String</span></span>|<span data-ttu-id="40e55-114">通知を生成したプロバイダーまたはサブプロバイダのバージョン (存在する場合)。</span><span class="sxs-lookup"><span data-stu-id="40e55-114">Version of the provider or subprovider, if it exists, that generated the alert.</span></span> <span data-ttu-id="40e55-115">*必須*</span><span class="sxs-lookup"><span data-stu-id="40e55-115">*Required*</span></span>|
|<span data-ttu-id="40e55-116">subprovider</span><span class="sxs-lookup"><span data-stu-id="40e55-116">subProvider</span></span>|<span data-ttu-id="40e55-117">String</span><span class="sxs-lookup"><span data-stu-id="40e55-117">String</span></span>|<span data-ttu-id="40e55-118">特定のサブプロバイダ (集計プロバイダーの場合)。たとえば、windowsdefenderatp。</span><span class="sxs-lookup"><span data-stu-id="40e55-118">Specific subprovider (under aggregating provider); for example, WindowsDefenderATP.SmartScreen.</span></span>|
|<span data-ttu-id="40e55-119">ベンダ</span><span class="sxs-lookup"><span data-stu-id="40e55-119">vendor</span></span> |<span data-ttu-id="40e55-120">String</span><span class="sxs-lookup"><span data-stu-id="40e55-120">String</span></span>|<span data-ttu-id="40e55-121">通知ベンダーの名前 (Microsoft、Dell、焼討アイなど)。</span><span class="sxs-lookup"><span data-stu-id="40e55-121">Name of the alert vendor (for example, Microsoft, Dell, FireEye).</span></span> <span data-ttu-id="40e55-122">*必須*</span><span class="sxs-lookup"><span data-stu-id="40e55-122">*Required*</span></span>|


## <a name="json-representation"></a><span data-ttu-id="40e55-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="40e55-123">JSON representation</span></span>

<span data-ttu-id="40e55-124">folllowing は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="40e55-124">The folllowing is a JSON representation of the resource.</span></span>
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
