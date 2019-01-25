---
title: securityVendorInformation リソースの種類
description: " > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。"
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: e67a5306b1dd08933877dbe3e64cab766ccd6a96
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512179"
---
# <a name="securityvendorinformation-resource-type"></a><span data-ttu-id="6c92c-104">securityVendorInformation リソースの種類</span><span class="sxs-lookup"><span data-stu-id="6c92c-104">securityVendorInformation resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6c92c-105">セキュリティ製品やサービスの仕入先、プロバイダー、および subprovider の詳細が含まれています (たとえば、ベンダー = Microsoft; プロバイダー = Windows Defender の分析ツールです。 subProvider AppLocker を =)。</span><span class="sxs-lookup"><span data-stu-id="6c92c-105">Contains details about the security product/service vendor, provider, and subprovider (for example, vendor=Microsoft; provider=Windows Defender ATP; subProvider=AppLocker).</span></span>

## <a name="properties"></a><span data-ttu-id="6c92c-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6c92c-106">Properties</span></span>

| <span data-ttu-id="6c92c-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6c92c-107">Property</span></span>   | <span data-ttu-id="6c92c-108">型</span><span class="sxs-lookup"><span data-stu-id="6c92c-108">Type</span></span>|<span data-ttu-id="6c92c-109">説明</span><span class="sxs-lookup"><span data-stu-id="6c92c-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6c92c-110">Provider</span><span class="sxs-lookup"><span data-stu-id="6c92c-110">provider</span></span> |<span data-ttu-id="6c92c-111">String</span><span class="sxs-lookup"><span data-stu-id="6c92c-111">String</span></span>|<span data-ttu-id="6c92c-112">特定のプロバイダー (製品やサービスの仕入先会社ではありません)。たとえば、WindowsDefenderATP です。</span><span class="sxs-lookup"><span data-stu-id="6c92c-112">Specific provider (product/service - not vendor company); for example, WindowsDefenderATP.</span></span>|
|<span data-ttu-id="6c92c-113">providerVersion</span><span class="sxs-lookup"><span data-stu-id="6c92c-113">providerVersion</span></span>|<span data-ttu-id="6c92c-114">String</span><span class="sxs-lookup"><span data-stu-id="6c92c-114">String</span></span>|<span data-ttu-id="6c92c-115">Subprovider、それが存在する場合は、アラートを生成したプロバイダーのバージョンです。</span><span class="sxs-lookup"><span data-stu-id="6c92c-115">Version of the provider or subprovider, if it exists, that generated the alert.</span></span> <span data-ttu-id="6c92c-116">*Required*</span><span class="sxs-lookup"><span data-stu-id="6c92c-116">*Required*</span></span>|
|<span data-ttu-id="6c92c-117">subProvider</span><span class="sxs-lookup"><span data-stu-id="6c92c-117">subProvider</span></span>|<span data-ttu-id="6c92c-118">String</span><span class="sxs-lookup"><span data-stu-id="6c92c-118">String</span></span>|<span data-ttu-id="6c92c-119">特定の subprovider 下にあるプロバイダーを集約)。たとえば、WindowsDefenderATP.SmartScreen です。</span><span class="sxs-lookup"><span data-stu-id="6c92c-119">Specific subprovider (under aggregating provider); for example, WindowsDefenderATP.SmartScreen.</span></span>|
|<span data-ttu-id="6c92c-120">仕入先</span><span class="sxs-lookup"><span data-stu-id="6c92c-120">vendor</span></span> |<span data-ttu-id="6c92c-121">String</span><span class="sxs-lookup"><span data-stu-id="6c92c-121">String</span></span>|<span data-ttu-id="6c92c-122">アラート ベンダー (マイクロソフトでは、Dell の FireEye など) の名前。</span><span class="sxs-lookup"><span data-stu-id="6c92c-122">Name of the alert vendor (for example, Microsoft, Dell, FireEye).</span></span> <span data-ttu-id="6c92c-123">*Required*</span><span class="sxs-lookup"><span data-stu-id="6c92c-123">*Required*</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6c92c-124">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="6c92c-124">JSON representation</span></span>

<span data-ttu-id="6c92c-125">次は、リソースの JSON 表現です。</span><span class="sxs-lookup"><span data-stu-id="6c92c-125">The folllowing is a JSON representation of the resource.</span></span>
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
  "suppressions": [
    "Error: /api-reference/beta/resources/securityvendorinformation.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
