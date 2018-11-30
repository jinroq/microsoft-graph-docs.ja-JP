---
title: securityVendorInformation リソースの種類
description: " > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。"
ms.openlocfilehash: 4016e274a82ad6a28101dbf5b053124b439a3cbf
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27072234"
---
# <a name="securityvendorinformation-resource-type"></a><span data-ttu-id="d7aaf-104">securityVendorInformation リソースの種類</span><span class="sxs-lookup"><span data-stu-id="d7aaf-104">securityVendorInformation resource type</span></span>

 > <span data-ttu-id="d7aaf-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="d7aaf-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d7aaf-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d7aaf-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d7aaf-107">セキュリティ製品やサービスの仕入先、プロバイダー、および subprovider の詳細が含まれています (たとえば、ベンダー = Microsoft; プロバイダー = Windows Defender の分析ツールです。 subProvider AppLocker を =)。</span><span class="sxs-lookup"><span data-stu-id="d7aaf-107">Contains details about the security product/service vendor, provider, and subprovider (for example, vendor=Microsoft; provider=Windows Defender ATP; subProvider=AppLocker).</span></span>

## <a name="properties"></a><span data-ttu-id="d7aaf-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d7aaf-108">Properties</span></span>

| <span data-ttu-id="d7aaf-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d7aaf-109">Property</span></span>   | <span data-ttu-id="d7aaf-110">型</span><span class="sxs-lookup"><span data-stu-id="d7aaf-110">Type</span></span>|<span data-ttu-id="d7aaf-111">説明</span><span class="sxs-lookup"><span data-stu-id="d7aaf-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d7aaf-112">プロバイダー</span><span class="sxs-lookup"><span data-stu-id="d7aaf-112">provider</span></span> |<span data-ttu-id="d7aaf-113">String</span><span class="sxs-lookup"><span data-stu-id="d7aaf-113">String</span></span>|<span data-ttu-id="d7aaf-114">特定のプロバイダー (製品やサービスの仕入先会社ではありません)。たとえば、WindowsDefenderATP です。</span><span class="sxs-lookup"><span data-stu-id="d7aaf-114">Specific provider (product/service - not vendor company); for example, WindowsDefenderATP.</span></span>|
|<span data-ttu-id="d7aaf-115">providerVersion</span><span class="sxs-lookup"><span data-stu-id="d7aaf-115">providerVersion</span></span>|<span data-ttu-id="d7aaf-116">String</span><span class="sxs-lookup"><span data-stu-id="d7aaf-116">String</span></span>|<span data-ttu-id="d7aaf-117">Subprovider、それが存在する場合は、アラートを生成したプロバイダーのバージョンです。</span><span class="sxs-lookup"><span data-stu-id="d7aaf-117">Version of the provider or subprovider, if it exists, that generated the alert.</span></span> <span data-ttu-id="d7aaf-118">*Required*</span><span class="sxs-lookup"><span data-stu-id="d7aaf-118">*Required*</span></span>|
|<span data-ttu-id="d7aaf-119">subProvider</span><span class="sxs-lookup"><span data-stu-id="d7aaf-119">subProvider</span></span>|<span data-ttu-id="d7aaf-120">String</span><span class="sxs-lookup"><span data-stu-id="d7aaf-120">String</span></span>|<span data-ttu-id="d7aaf-121">特定の subprovider 下にあるプロバイダーを集約)。たとえば、WindowsDefenderATP.SmartScreen です。</span><span class="sxs-lookup"><span data-stu-id="d7aaf-121">Specific subprovider (under aggregating provider); for example, WindowsDefenderATP.SmartScreen.</span></span>|
|<span data-ttu-id="d7aaf-122">仕入先</span><span class="sxs-lookup"><span data-stu-id="d7aaf-122">vendor</span></span> |<span data-ttu-id="d7aaf-123">String</span><span class="sxs-lookup"><span data-stu-id="d7aaf-123">String</span></span>|<span data-ttu-id="d7aaf-124">アラート ベンダー (マイクロソフトでは、Dell の FireEye など) の名前。</span><span class="sxs-lookup"><span data-stu-id="d7aaf-124">Name of the alert vendor (for example, Microsoft, Dell, FireEye).</span></span> <span data-ttu-id="d7aaf-125">*Required*</span><span class="sxs-lookup"><span data-stu-id="d7aaf-125">*Required*</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d7aaf-126">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d7aaf-126">JSON representation</span></span>

<span data-ttu-id="d7aaf-127">次は、リソースの JSON 表現です。</span><span class="sxs-lookup"><span data-stu-id="d7aaf-127">The folllowing is a JSON representation of the resource.</span></span>
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
