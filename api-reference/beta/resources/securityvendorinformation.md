---
title: securityVendorInformation リソースの種類
description: " > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでは、これらの API の使用はサポートされていません。"
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: d543bf16617ed28d50d2e7082372ff2014cd24c5
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33343302"
---
# <a name="securityvendorinformation-resource-type"></a><span data-ttu-id="cbe2c-104">securityVendorInformation リソースの種類</span><span class="sxs-lookup"><span data-stu-id="cbe2c-104">securityVendorInformation resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cbe2c-105">セキュリティ製品/サービスベンダー、プロバイダ、およびサブプロバイダに関する詳細情報が含まれています (たとえば、ベンダー = Microsoft; provider = Windows Defender ATP; subprovider = AppLocker)。</span><span class="sxs-lookup"><span data-stu-id="cbe2c-105">Contains details about the security product/service vendor, provider, and subprovider (for example, vendor=Microsoft; provider=Windows Defender ATP; subProvider=AppLocker).</span></span>

## <a name="properties"></a><span data-ttu-id="cbe2c-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cbe2c-106">Properties</span></span>

| <span data-ttu-id="cbe2c-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cbe2c-107">Property</span></span>   | <span data-ttu-id="cbe2c-108">型</span><span class="sxs-lookup"><span data-stu-id="cbe2c-108">Type</span></span>|<span data-ttu-id="cbe2c-109">説明</span><span class="sxs-lookup"><span data-stu-id="cbe2c-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cbe2c-110">供給</span><span class="sxs-lookup"><span data-stu-id="cbe2c-110">provider</span></span> |<span data-ttu-id="cbe2c-111">String</span><span class="sxs-lookup"><span data-stu-id="cbe2c-111">String</span></span>|<span data-ttu-id="cbe2c-112">特定のプロバイダー (製品/サービス-ベンダー会社ではない)。たとえば、windowsdefenderatp のようになります。</span><span class="sxs-lookup"><span data-stu-id="cbe2c-112">Specific provider (product/service - not vendor company); for example, WindowsDefenderATP.</span></span>|
|<span data-ttu-id="cbe2c-113">providerversion</span><span class="sxs-lookup"><span data-stu-id="cbe2c-113">providerVersion</span></span>|<span data-ttu-id="cbe2c-114">String</span><span class="sxs-lookup"><span data-stu-id="cbe2c-114">String</span></span>|<span data-ttu-id="cbe2c-115">通知を生成したプロバイダーまたはサブプロバイダのバージョン (存在する場合)。</span><span class="sxs-lookup"><span data-stu-id="cbe2c-115">Version of the provider or subprovider, if it exists, that generated the alert.</span></span> <span data-ttu-id="cbe2c-116">**必須**</span><span class="sxs-lookup"><span data-stu-id="cbe2c-116">**Required**</span></span>|
|<span data-ttu-id="cbe2c-117">subprovider</span><span class="sxs-lookup"><span data-stu-id="cbe2c-117">subProvider</span></span>|<span data-ttu-id="cbe2c-118">String</span><span class="sxs-lookup"><span data-stu-id="cbe2c-118">String</span></span>|<span data-ttu-id="cbe2c-119">特定のサブプロバイダ (集計プロバイダーの場合)。たとえば、windowsdefenderatp。</span><span class="sxs-lookup"><span data-stu-id="cbe2c-119">Specific subprovider (under aggregating provider); for example, WindowsDefenderATP.SmartScreen.</span></span>|
|<span data-ttu-id="cbe2c-120">ベンダ</span><span class="sxs-lookup"><span data-stu-id="cbe2c-120">vendor</span></span> |<span data-ttu-id="cbe2c-121">String</span><span class="sxs-lookup"><span data-stu-id="cbe2c-121">String</span></span>|<span data-ttu-id="cbe2c-122">通知ベンダーの名前 (Microsoft、Dell、焼討アイなど)。</span><span class="sxs-lookup"><span data-stu-id="cbe2c-122">Name of the alert vendor (for example, Microsoft, Dell, FireEye).</span></span> <span data-ttu-id="cbe2c-123">**必須**</span><span class="sxs-lookup"><span data-stu-id="cbe2c-123">**Required**</span></span>|

## <a name="json-representation"></a><span data-ttu-id="cbe2c-124">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="cbe2c-124">JSON representation</span></span>

<span data-ttu-id="cbe2c-125">folllowing は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="cbe2c-125">The folllowing is a JSON representation of the resource.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "securityVendorInformation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
