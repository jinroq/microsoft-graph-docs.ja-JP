---
title: iosEduCertificateSettings リソースの種類
description: 信頼されたルートと PFX 証明書 EDU の入出力数のです。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: d23b379dea7a75e4ae79029845cd6e9f956503c0
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29423553"
---
# <a name="ioseducertificatesettings-resource-type"></a><span data-ttu-id="80bdf-103">iosEduCertificateSettings リソースの種類</span><span class="sxs-lookup"><span data-stu-id="80bdf-103">iosEduCertificateSettings resource type</span></span>

> <span data-ttu-id="80bdf-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="80bdf-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="80bdf-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="80bdf-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="80bdf-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="80bdf-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="80bdf-107">信頼されたルートと PFX 証明書 EDU の入出力数のです。</span><span class="sxs-lookup"><span data-stu-id="80bdf-107">Trusted Root and PFX certificates for iOS EDU.</span></span>

## <a name="properties"></a><span data-ttu-id="80bdf-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="80bdf-108">Properties</span></span>
|<span data-ttu-id="80bdf-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="80bdf-109">Property</span></span>|<span data-ttu-id="80bdf-110">型</span><span class="sxs-lookup"><span data-stu-id="80bdf-110">Type</span></span>|<span data-ttu-id="80bdf-111">説明</span><span class="sxs-lookup"><span data-stu-id="80bdf-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="80bdf-112">trustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="80bdf-112">trustedRootCertificate</span></span>|<span data-ttu-id="80bdf-113">Binary</span><span class="sxs-lookup"><span data-stu-id="80bdf-113">Binary</span></span>|<span data-ttu-id="80bdf-114">信頼されたルート証明書です。</span><span class="sxs-lookup"><span data-stu-id="80bdf-114">Trusted Root Certificate.</span></span>|
|<span data-ttu-id="80bdf-115">します</span><span class="sxs-lookup"><span data-stu-id="80bdf-115">certFileName</span></span>|<span data-ttu-id="80bdf-116">String</span><span class="sxs-lookup"><span data-stu-id="80bdf-116">String</span></span>|<span data-ttu-id="80bdf-117">UI に表示するファイル名です。</span><span class="sxs-lookup"><span data-stu-id="80bdf-117">File name to display in UI.</span></span>|
|<span data-ttu-id="80bdf-118">certificationAuthority</span><span class="sxs-lookup"><span data-stu-id="80bdf-118">certificationAuthority</span></span>|<span data-ttu-id="80bdf-119">String</span><span class="sxs-lookup"><span data-stu-id="80bdf-119">String</span></span>|<span data-ttu-id="80bdf-120">PKCS 証明機関。</span><span class="sxs-lookup"><span data-stu-id="80bdf-120">PKCS Certification Authority.</span></span>|
|<span data-ttu-id="80bdf-121">certificationAuthorityName</span><span class="sxs-lookup"><span data-stu-id="80bdf-121">certificationAuthorityName</span></span>|<span data-ttu-id="80bdf-122">String</span><span class="sxs-lookup"><span data-stu-id="80bdf-122">String</span></span>|<span data-ttu-id="80bdf-123">PKCS 証明機関の名前です。</span><span class="sxs-lookup"><span data-stu-id="80bdf-123">PKCS Certification Authority Name.</span></span>|
|<span data-ttu-id="80bdf-124">certificateTemplateName</span><span class="sxs-lookup"><span data-stu-id="80bdf-124">certificateTemplateName</span></span>|<span data-ttu-id="80bdf-125">String</span><span class="sxs-lookup"><span data-stu-id="80bdf-125">String</span></span>|<span data-ttu-id="80bdf-126">PKCS の証明書テンプレートの名前です。</span><span class="sxs-lookup"><span data-stu-id="80bdf-126">PKCS Certificate Template Name.</span></span>|
|<span data-ttu-id="80bdf-127">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="80bdf-127">renewalThresholdPercentage</span></span>|<span data-ttu-id="80bdf-128">Int32</span><span class="sxs-lookup"><span data-stu-id="80bdf-128">Int32</span></span>|<span data-ttu-id="80bdf-129">証明書の書き換えのしきい値の割合です。</span><span class="sxs-lookup"><span data-stu-id="80bdf-129">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="80bdf-130">1 から 99 までの有効な値</span><span class="sxs-lookup"><span data-stu-id="80bdf-130">Valid values 1 to 99</span></span>|
|<span data-ttu-id="80bdf-131">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="80bdf-131">certificateValidityPeriodValue</span></span>|<span data-ttu-id="80bdf-132">Int32</span><span class="sxs-lookup"><span data-stu-id="80bdf-132">Int32</span></span>|<span data-ttu-id="80bdf-133">証明書の有効期間の値です。</span><span class="sxs-lookup"><span data-stu-id="80bdf-133">Value for the Certificate Validity Period.</span></span>|
|<span data-ttu-id="80bdf-134">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="80bdf-134">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="80bdf-135">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="80bdf-135">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="80bdf-136">証明書の有効期間のスケールです。</span><span class="sxs-lookup"><span data-stu-id="80bdf-136">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="80bdf-137">可能な値は、`days`、`months`、`years` です。</span><span class="sxs-lookup"><span data-stu-id="80bdf-137">Possible values are: `days`, `months`, `years`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="80bdf-138">関係</span><span class="sxs-lookup"><span data-stu-id="80bdf-138">Relationships</span></span>
<span data-ttu-id="80bdf-139">なし</span><span class="sxs-lookup"><span data-stu-id="80bdf-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="80bdf-140">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="80bdf-140">JSON Representation</span></span>
<span data-ttu-id="80bdf-141">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="80bdf-141">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosEduCertificateSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosEduCertificateSettings",
  "trustedRootCertificate": "binary",
  "certFileName": "String",
  "certificationAuthority": "String",
  "certificationAuthorityName": "String",
  "certificateTemplateName": "String",
  "renewalThresholdPercentage": 1024,
  "certificateValidityPeriodValue": 1024,
  "certificateValidityPeriodScale": "String"
}
```




