---
title: iosEduCertificateSettings リソースの種類
description: IOS EDU の信頼されたルートおよび PFX 証明書。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: dd063ec70dd794ffb151036ea7bbbda090829343
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36001257"
---
# <a name="ioseducertificatesettings-resource-type"></a><span data-ttu-id="29b4d-103">iosEduCertificateSettings リソースの種類</span><span class="sxs-lookup"><span data-stu-id="29b4d-103">iosEduCertificateSettings resource type</span></span>

> <span data-ttu-id="29b4d-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="29b4d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="29b4d-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="29b4d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="29b4d-106">IOS EDU の信頼されたルートおよび PFX 証明書。</span><span class="sxs-lookup"><span data-stu-id="29b4d-106">Trusted Root and PFX certificates for iOS EDU.</span></span>

## <a name="properties"></a><span data-ttu-id="29b4d-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="29b4d-107">Properties</span></span>
|<span data-ttu-id="29b4d-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="29b4d-108">Property</span></span>|<span data-ttu-id="29b4d-109">型</span><span class="sxs-lookup"><span data-stu-id="29b4d-109">Type</span></span>|<span data-ttu-id="29b4d-110">説明</span><span class="sxs-lookup"><span data-stu-id="29b4d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="29b4d-111">trustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="29b4d-111">trustedRootCertificate</span></span>|<span data-ttu-id="29b4d-112">Binary</span><span class="sxs-lookup"><span data-stu-id="29b4d-112">Binary</span></span>|<span data-ttu-id="29b4d-113">信頼されたルート証明書。</span><span class="sxs-lookup"><span data-stu-id="29b4d-113">Trusted Root Certificate.</span></span>|
|<span data-ttu-id="29b4d-114">certFileName</span><span class="sxs-lookup"><span data-stu-id="29b4d-114">certFileName</span></span>|<span data-ttu-id="29b4d-115">String</span><span class="sxs-lookup"><span data-stu-id="29b4d-115">String</span></span>|<span data-ttu-id="29b4d-116">UI に表示されるファイル名。</span><span class="sxs-lookup"><span data-stu-id="29b4d-116">File name to display in UI.</span></span>|
|<span data-ttu-id="29b4d-117">certificationAuthority</span><span class="sxs-lookup"><span data-stu-id="29b4d-117">certificationAuthority</span></span>|<span data-ttu-id="29b4d-118">String</span><span class="sxs-lookup"><span data-stu-id="29b4d-118">String</span></span>|<span data-ttu-id="29b4d-119">PKCS 証明機関。</span><span class="sxs-lookup"><span data-stu-id="29b4d-119">PKCS Certification Authority.</span></span>|
|<span data-ttu-id="29b4d-120">certificationAuthorityName</span><span class="sxs-lookup"><span data-stu-id="29b4d-120">certificationAuthorityName</span></span>|<span data-ttu-id="29b4d-121">String</span><span class="sxs-lookup"><span data-stu-id="29b4d-121">String</span></span>|<span data-ttu-id="29b4d-122">PKCS 証明機関名。</span><span class="sxs-lookup"><span data-stu-id="29b4d-122">PKCS Certification Authority Name.</span></span>|
|<span data-ttu-id="29b4d-123">certificateTemplateName</span><span class="sxs-lookup"><span data-stu-id="29b4d-123">certificateTemplateName</span></span>|<span data-ttu-id="29b4d-124">String</span><span class="sxs-lookup"><span data-stu-id="29b4d-124">String</span></span>|<span data-ttu-id="29b4d-125">PKCS 証明書テンプレート名。</span><span class="sxs-lookup"><span data-stu-id="29b4d-125">PKCS Certificate Template Name.</span></span>|
|<span data-ttu-id="29b4d-126">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="29b4d-126">renewalThresholdPercentage</span></span>|<span data-ttu-id="29b4d-127">Int32</span><span class="sxs-lookup"><span data-stu-id="29b4d-127">Int32</span></span>|<span data-ttu-id="29b4d-128">証明書の更新しきい値の割合。</span><span class="sxs-lookup"><span data-stu-id="29b4d-128">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="29b4d-129">有効な値は 1 ~ 99</span><span class="sxs-lookup"><span data-stu-id="29b4d-129">Valid values 1 to 99</span></span>|
|<span data-ttu-id="29b4d-130">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="29b4d-130">certificateValidityPeriodValue</span></span>|<span data-ttu-id="29b4d-131">Int32</span><span class="sxs-lookup"><span data-stu-id="29b4d-131">Int32</span></span>|<span data-ttu-id="29b4d-132">証明書の有効期間の値。</span><span class="sxs-lookup"><span data-stu-id="29b4d-132">Value for the Certificate Validity Period.</span></span>|
|<span data-ttu-id="29b4d-133">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="29b4d-133">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="29b4d-134">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="29b4d-134">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="29b4d-135">証明書の有効期間のスケール。</span><span class="sxs-lookup"><span data-stu-id="29b4d-135">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="29b4d-136">可能な値は、`days`、`months`、`years` です。</span><span class="sxs-lookup"><span data-stu-id="29b4d-136">Possible values are: `days`, `months`, `years`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="29b4d-137">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="29b4d-137">Relationships</span></span>
<span data-ttu-id="29b4d-138">なし</span><span class="sxs-lookup"><span data-stu-id="29b4d-138">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="29b4d-139">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="29b4d-139">JSON Representation</span></span>
<span data-ttu-id="29b4d-140">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="29b4d-140">Here is a JSON representation of the resource.</span></span>
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





