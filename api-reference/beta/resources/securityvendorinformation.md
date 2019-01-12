---
title: securityVendorInformation リソースの種類
description: " > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。"
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: 0137abd7a9df0df94f73e18d7efa201008031ff6
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27939925"
---
# <a name="securityvendorinformation-resource-type"></a><span data-ttu-id="21f7b-104">securityVendorInformation リソースの種類</span><span class="sxs-lookup"><span data-stu-id="21f7b-104">securityVendorInformation resource type</span></span>

 > <span data-ttu-id="21f7b-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="21f7b-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="21f7b-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="21f7b-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="21f7b-107">セキュリティ製品やサービスの仕入先、プロバイダー、および subprovider の詳細が含まれています (たとえば、ベンダー = Microsoft; プロバイダー = Windows Defender の分析ツールです。 subProvider AppLocker を =)。</span><span class="sxs-lookup"><span data-stu-id="21f7b-107">Contains details about the security product/service vendor, provider, and subprovider (for example, vendor=Microsoft; provider=Windows Defender ATP; subProvider=AppLocker).</span></span>

## <a name="properties"></a><span data-ttu-id="21f7b-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="21f7b-108">Properties</span></span>

| <span data-ttu-id="21f7b-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="21f7b-109">Property</span></span>   | <span data-ttu-id="21f7b-110">種類</span><span class="sxs-lookup"><span data-stu-id="21f7b-110">Type</span></span>|<span data-ttu-id="21f7b-111">説明</span><span class="sxs-lookup"><span data-stu-id="21f7b-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="21f7b-112">プロバイダー</span><span class="sxs-lookup"><span data-stu-id="21f7b-112">provider</span></span> |<span data-ttu-id="21f7b-113">String</span><span class="sxs-lookup"><span data-stu-id="21f7b-113">String</span></span>|<span data-ttu-id="21f7b-114">特定のプロバイダー (製品やサービスの仕入先会社ではありません)。たとえば、WindowsDefenderATP です。</span><span class="sxs-lookup"><span data-stu-id="21f7b-114">Specific provider (product/service - not vendor company); for example, WindowsDefenderATP.</span></span>|
|<span data-ttu-id="21f7b-115">providerVersion</span><span class="sxs-lookup"><span data-stu-id="21f7b-115">providerVersion</span></span>|<span data-ttu-id="21f7b-116">String</span><span class="sxs-lookup"><span data-stu-id="21f7b-116">String</span></span>|<span data-ttu-id="21f7b-117">Subprovider、それが存在する場合は、アラートを生成したプロバイダーのバージョンです。</span><span class="sxs-lookup"><span data-stu-id="21f7b-117">Version of the provider or subprovider, if it exists, that generated the alert.</span></span> <span data-ttu-id="21f7b-118">*Required*</span><span class="sxs-lookup"><span data-stu-id="21f7b-118">*Required*</span></span>|
|<span data-ttu-id="21f7b-119">subProvider</span><span class="sxs-lookup"><span data-stu-id="21f7b-119">subProvider</span></span>|<span data-ttu-id="21f7b-120">String</span><span class="sxs-lookup"><span data-stu-id="21f7b-120">String</span></span>|<span data-ttu-id="21f7b-121">特定の subprovider 下にあるプロバイダーを集約)。たとえば、WindowsDefenderATP.SmartScreen です。</span><span class="sxs-lookup"><span data-stu-id="21f7b-121">Specific subprovider (under aggregating provider); for example, WindowsDefenderATP.SmartScreen.</span></span>|
|<span data-ttu-id="21f7b-122">仕入先</span><span class="sxs-lookup"><span data-stu-id="21f7b-122">vendor</span></span> |<span data-ttu-id="21f7b-123">String</span><span class="sxs-lookup"><span data-stu-id="21f7b-123">String</span></span>|<span data-ttu-id="21f7b-124">アラート ベンダー (マイクロソフトでは、Dell の FireEye など) の名前。</span><span class="sxs-lookup"><span data-stu-id="21f7b-124">Name of the alert vendor (for example, Microsoft, Dell, FireEye).</span></span> <span data-ttu-id="21f7b-125">*Required*</span><span class="sxs-lookup"><span data-stu-id="21f7b-125">*Required*</span></span>|

## <a name="json-representation"></a><span data-ttu-id="21f7b-126">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="21f7b-126">JSON representation</span></span>

<span data-ttu-id="21f7b-127">次は、リソースの JSON 表現です。</span><span class="sxs-lookup"><span data-stu-id="21f7b-127">The folllowing is a JSON representation of the resource.</span></span>
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
