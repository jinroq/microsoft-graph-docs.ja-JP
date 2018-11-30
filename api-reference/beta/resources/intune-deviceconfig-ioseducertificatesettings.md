---
title: iosEduCertificateSettings リソースの種類
description: 信頼されたルートと PFX 証明書 EDU の入出力数のです。
ms.openlocfilehash: 348b8231ed87c46180c54eb5ebfe24d671c9015b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27068263"
---
# <a name="ioseducertificatesettings-resource-type"></a><span data-ttu-id="e02c8-103">iosEduCertificateSettings リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e02c8-103">iosEduCertificateSettings resource type</span></span>

> <span data-ttu-id="e02c8-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="e02c8-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e02c8-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e02c8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e02c8-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="e02c8-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e02c8-107">信頼されたルートと PFX 証明書 EDU の入出力数のです。</span><span class="sxs-lookup"><span data-stu-id="e02c8-107">Trusted Root and PFX certificates for iOS EDU.</span></span>
## <a name="properties"></a><span data-ttu-id="e02c8-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e02c8-108">Properties</span></span>
|<span data-ttu-id="e02c8-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e02c8-109">Property</span></span>|<span data-ttu-id="e02c8-110">型</span><span class="sxs-lookup"><span data-stu-id="e02c8-110">Type</span></span>|<span data-ttu-id="e02c8-111">説明</span><span class="sxs-lookup"><span data-stu-id="e02c8-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e02c8-112">trustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="e02c8-112">trustedRootCertificate</span></span>|<span data-ttu-id="e02c8-113">バイナリ</span><span class="sxs-lookup"><span data-stu-id="e02c8-113">Binary</span></span>|<span data-ttu-id="e02c8-114">信頼されたルート証明書です。</span><span class="sxs-lookup"><span data-stu-id="e02c8-114">Trusted Root Certificate.</span></span>|
|<span data-ttu-id="e02c8-115">します</span><span class="sxs-lookup"><span data-stu-id="e02c8-115">certFileName</span></span>|<span data-ttu-id="e02c8-116">String</span><span class="sxs-lookup"><span data-stu-id="e02c8-116">String</span></span>|<span data-ttu-id="e02c8-117">UI に表示するファイル名です。</span><span class="sxs-lookup"><span data-stu-id="e02c8-117">File name to display in UI.</span></span>|
|<span data-ttu-id="e02c8-118">certificationAuthority</span><span class="sxs-lookup"><span data-stu-id="e02c8-118">certificationAuthority</span></span>|<span data-ttu-id="e02c8-119">String</span><span class="sxs-lookup"><span data-stu-id="e02c8-119">String</span></span>|<span data-ttu-id="e02c8-120">PKCS 証明機関。</span><span class="sxs-lookup"><span data-stu-id="e02c8-120">PKCS Certification Authority.</span></span>|
|<span data-ttu-id="e02c8-121">certificationAuthorityName</span><span class="sxs-lookup"><span data-stu-id="e02c8-121">certificationAuthorityName</span></span>|<span data-ttu-id="e02c8-122">String</span><span class="sxs-lookup"><span data-stu-id="e02c8-122">String</span></span>|<span data-ttu-id="e02c8-123">PKCS 証明機関の名前です。</span><span class="sxs-lookup"><span data-stu-id="e02c8-123">PKCS Certification Authority Name.</span></span>|
|<span data-ttu-id="e02c8-124">certificateTemplateName</span><span class="sxs-lookup"><span data-stu-id="e02c8-124">certificateTemplateName</span></span>|<span data-ttu-id="e02c8-125">String</span><span class="sxs-lookup"><span data-stu-id="e02c8-125">String</span></span>|<span data-ttu-id="e02c8-126">PKCS の証明書テンプレートの名前です。</span><span class="sxs-lookup"><span data-stu-id="e02c8-126">PKCS Certificate Template Name.</span></span>|
|<span data-ttu-id="e02c8-127">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="e02c8-127">renewalThresholdPercentage</span></span>|<span data-ttu-id="e02c8-128">Int32</span><span class="sxs-lookup"><span data-stu-id="e02c8-128">Int32</span></span>|<span data-ttu-id="e02c8-129">証明書の書き換えのしきい値の割合です。</span><span class="sxs-lookup"><span data-stu-id="e02c8-129">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="e02c8-130">1 から 99 までの有効な値</span><span class="sxs-lookup"><span data-stu-id="e02c8-130">Valid values 1 to 99</span></span>|
|<span data-ttu-id="e02c8-131">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="e02c8-131">certificateValidityPeriodValue</span></span>|<span data-ttu-id="e02c8-132">Int32</span><span class="sxs-lookup"><span data-stu-id="e02c8-132">Int32</span></span>|<span data-ttu-id="e02c8-133">証明書の有効期間の値です。</span><span class="sxs-lookup"><span data-stu-id="e02c8-133">Value for the Certificate Validity Period.</span></span>|
|<span data-ttu-id="e02c8-134">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="e02c8-134">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="e02c8-135">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="e02c8-135">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="e02c8-136">証明書の有効期間のスケールです。</span><span class="sxs-lookup"><span data-stu-id="e02c8-136">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="e02c8-137">可能な値は、`days`、`months`、`years` です。</span><span class="sxs-lookup"><span data-stu-id="e02c8-137">Possible values are: `days`, `months`, `years`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e02c8-138">関係</span><span class="sxs-lookup"><span data-stu-id="e02c8-138">Relationships</span></span>
<span data-ttu-id="e02c8-139">なし</span><span class="sxs-lookup"><span data-stu-id="e02c8-139">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="e02c8-140">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e02c8-140">JSON Representation</span></span>
<span data-ttu-id="e02c8-141">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="e02c8-141">Here is a JSON representation of the resource.</span></span>
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





