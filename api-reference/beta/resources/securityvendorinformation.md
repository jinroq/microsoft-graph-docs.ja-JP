---
title: securityVendorInformation リソースの種類
description: " > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでは、これらの API の使用はサポートされていません。"
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: 7f48c27ba94d8419ce244143a48cf6ab04dd080e
ms.sourcegitcommit: 88ddd033de0f36eedade277d57c922ebd0db5bba
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/02/2019
ms.locfileid: "30364585"
---
# <a name="securityvendorinformation-resource-type"></a><span data-ttu-id="040d0-104">securityVendorInformation リソースの種類</span><span class="sxs-lookup"><span data-stu-id="040d0-104">securityVendorInformation resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="040d0-105">セキュリティ製品/サービスベンダー、プロバイダ、およびサブプロバイダに関する詳細情報が含まれています (たとえば、ベンダー = Microsoft; provider = Windows Defender ATP; subprovider = AppLocker)。</span><span class="sxs-lookup"><span data-stu-id="040d0-105">Contains details about the security product/service vendor, provider, and subprovider (for example, vendor=Microsoft; provider=Windows Defender ATP; subProvider=AppLocker).</span></span>

## <a name="properties"></a><span data-ttu-id="040d0-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="040d0-106">Properties</span></span>

| <span data-ttu-id="040d0-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="040d0-107">Property</span></span>   | <span data-ttu-id="040d0-108">型</span><span class="sxs-lookup"><span data-stu-id="040d0-108">Type</span></span>|<span data-ttu-id="040d0-109">説明</span><span class="sxs-lookup"><span data-stu-id="040d0-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="040d0-110">供給</span><span class="sxs-lookup"><span data-stu-id="040d0-110">provider</span></span> |<span data-ttu-id="040d0-111">String</span><span class="sxs-lookup"><span data-stu-id="040d0-111">String</span></span>|<span data-ttu-id="040d0-112">特定のプロバイダー (製品/サービス-ベンダー会社ではない)。たとえば、windowsdefenderatp のようになります。</span><span class="sxs-lookup"><span data-stu-id="040d0-112">Specific provider (product/service - not vendor company); for example, WindowsDefenderATP.</span></span>|
|<span data-ttu-id="040d0-113">providerversion</span><span class="sxs-lookup"><span data-stu-id="040d0-113">providerVersion</span></span>|<span data-ttu-id="040d0-114">String</span><span class="sxs-lookup"><span data-stu-id="040d0-114">String</span></span>|<span data-ttu-id="040d0-115">通知を生成したプロバイダーまたはサブプロバイダのバージョン (存在する場合)。</span><span class="sxs-lookup"><span data-stu-id="040d0-115">Version of the provider or subprovider, if it exists, that generated the alert.</span></span> <span data-ttu-id="040d0-116">**Required**</span><span class="sxs-lookup"><span data-stu-id="040d0-116">**Required**</span></span>|
|<span data-ttu-id="040d0-117">subprovider</span><span class="sxs-lookup"><span data-stu-id="040d0-117">subProvider</span></span>|<span data-ttu-id="040d0-118">String</span><span class="sxs-lookup"><span data-stu-id="040d0-118">String</span></span>|<span data-ttu-id="040d0-119">特定のサブプロバイダ (集計プロバイダーの場合)。たとえば、windowsdefenderatp。</span><span class="sxs-lookup"><span data-stu-id="040d0-119">Specific subprovider (under aggregating provider); for example, WindowsDefenderATP.SmartScreen.</span></span>|
|<span data-ttu-id="040d0-120">ベンダ</span><span class="sxs-lookup"><span data-stu-id="040d0-120">vendor</span></span> |<span data-ttu-id="040d0-121">String</span><span class="sxs-lookup"><span data-stu-id="040d0-121">String</span></span>|<span data-ttu-id="040d0-122">通知ベンダーの名前 (Microsoft、Dell、焼討アイなど)。</span><span class="sxs-lookup"><span data-stu-id="040d0-122">Name of the alert vendor (for example, Microsoft, Dell, FireEye).</span></span> <span data-ttu-id="040d0-123">**Required**</span><span class="sxs-lookup"><span data-stu-id="040d0-123">**Required**</span></span>|

## <a name="json-representation"></a><span data-ttu-id="040d0-124">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="040d0-124">JSON representation</span></span>

<span data-ttu-id="040d0-125">folllowing は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="040d0-125">The folllowing is a JSON representation of the resource.</span></span>
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
