---
title: iosEduCertificateSettings リソースの種類
description: iOS EDU の信頼されたルートおよび PFX 証明書。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8d9060c28744bae52d4690bf75487e298d58d2a1
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32571717"
---
# <a name="ioseducertificatesettings-resource-type"></a><span data-ttu-id="92e70-103">iosEduCertificateSettings リソースの種類</span><span class="sxs-lookup"><span data-stu-id="92e70-103">iosEduCertificateSettings resource type</span></span>

> <span data-ttu-id="92e70-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="92e70-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="92e70-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="92e70-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="92e70-106">iOS EDU の信頼されたルートおよび PFX 証明書。</span><span class="sxs-lookup"><span data-stu-id="92e70-106">Trusted Root and PFX certificates for iOS EDU.</span></span>

## <a name="properties"></a><span data-ttu-id="92e70-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="92e70-107">Properties</span></span>
|<span data-ttu-id="92e70-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="92e70-108">Property</span></span>|<span data-ttu-id="92e70-109">型</span><span class="sxs-lookup"><span data-stu-id="92e70-109">Type</span></span>|<span data-ttu-id="92e70-110">説明</span><span class="sxs-lookup"><span data-stu-id="92e70-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="92e70-111">trustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="92e70-111">trustedRootCertificate</span></span>|<span data-ttu-id="92e70-112">Binary</span><span class="sxs-lookup"><span data-stu-id="92e70-112">Binary</span></span>|<span data-ttu-id="92e70-113">信頼されたルート証明書。</span><span class="sxs-lookup"><span data-stu-id="92e70-113">Trusted Root Certificate.</span></span>|
|<span data-ttu-id="92e70-114">certfilename</span><span class="sxs-lookup"><span data-stu-id="92e70-114">certFileName</span></span>|<span data-ttu-id="92e70-115">String</span><span class="sxs-lookup"><span data-stu-id="92e70-115">String</span></span>|<span data-ttu-id="92e70-116">UI に表示されるファイル名。</span><span class="sxs-lookup"><span data-stu-id="92e70-116">File name to display in UI.</span></span>|
|<span data-ttu-id="92e70-117">certificationAuthority</span><span class="sxs-lookup"><span data-stu-id="92e70-117">certificationAuthority</span></span>|<span data-ttu-id="92e70-118">String</span><span class="sxs-lookup"><span data-stu-id="92e70-118">String</span></span>|<span data-ttu-id="92e70-119">PKCS 証明機関。</span><span class="sxs-lookup"><span data-stu-id="92e70-119">PKCS Certification Authority.</span></span>|
|<span data-ttu-id="92e70-120">certificationAuthorityName</span><span class="sxs-lookup"><span data-stu-id="92e70-120">certificationAuthorityName</span></span>|<span data-ttu-id="92e70-121">String</span><span class="sxs-lookup"><span data-stu-id="92e70-121">String</span></span>|<span data-ttu-id="92e70-122">PKCS 証明機関名。</span><span class="sxs-lookup"><span data-stu-id="92e70-122">PKCS Certification Authority Name.</span></span>|
|<span data-ttu-id="92e70-123">certificatetemplatename</span><span class="sxs-lookup"><span data-stu-id="92e70-123">certificateTemplateName</span></span>|<span data-ttu-id="92e70-124">String</span><span class="sxs-lookup"><span data-stu-id="92e70-124">String</span></span>|<span data-ttu-id="92e70-125">PKCS 証明書テンプレート名。</span><span class="sxs-lookup"><span data-stu-id="92e70-125">PKCS Certificate Template Name.</span></span>|
|<span data-ttu-id="92e70-126">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="92e70-126">renewalThresholdPercentage</span></span>|<span data-ttu-id="92e70-127">Int32</span><span class="sxs-lookup"><span data-stu-id="92e70-127">Int32</span></span>|<span data-ttu-id="92e70-128">証明書の更新しきい値の割合。</span><span class="sxs-lookup"><span data-stu-id="92e70-128">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="92e70-129">有効な値は 1 ~ 99</span><span class="sxs-lookup"><span data-stu-id="92e70-129">Valid values 1 to 99</span></span>|
|<span data-ttu-id="92e70-130">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="92e70-130">certificateValidityPeriodValue</span></span>|<span data-ttu-id="92e70-131">Int32</span><span class="sxs-lookup"><span data-stu-id="92e70-131">Int32</span></span>|<span data-ttu-id="92e70-132">証明書の有効期間の値。</span><span class="sxs-lookup"><span data-stu-id="92e70-132">Value for the Certificate Validity Period.</span></span>|
|<span data-ttu-id="92e70-133">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="92e70-133">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="92e70-134">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="92e70-134">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="92e70-135">証明書の有効期間のスケール。</span><span class="sxs-lookup"><span data-stu-id="92e70-135">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="92e70-136">可能な値は、`days`、`months`、`years` です。</span><span class="sxs-lookup"><span data-stu-id="92e70-136">Possible values are: `days`, `months`, `years`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="92e70-137">関係</span><span class="sxs-lookup"><span data-stu-id="92e70-137">Relationships</span></span>
<span data-ttu-id="92e70-138">なし</span><span class="sxs-lookup"><span data-stu-id="92e70-138">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="92e70-139">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="92e70-139">JSON Representation</span></span>
<span data-ttu-id="92e70-140">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="92e70-140">Here is a JSON representation of the resource.</span></span>
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





