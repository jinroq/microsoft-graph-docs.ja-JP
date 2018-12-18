---
title: iosEduCertificateSettings リソースの種類
description: 信頼されたルートと PFX 証明書 EDU の入出力数のです。
author: tfitzmac
ms.openlocfilehash: 8e373a7c878dd06870b13a32c428f837d741964c
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27332327"
---
# <a name="ioseducertificatesettings-resource-type"></a><span data-ttu-id="1cef6-103">iosEduCertificateSettings リソースの種類</span><span class="sxs-lookup"><span data-stu-id="1cef6-103">iosEduCertificateSettings resource type</span></span>

> <span data-ttu-id="1cef6-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="1cef6-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1cef6-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1cef6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1cef6-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="1cef6-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1cef6-107">信頼されたルートと PFX 証明書 EDU の入出力数のです。</span><span class="sxs-lookup"><span data-stu-id="1cef6-107">Trusted Root and PFX certificates for iOS EDU.</span></span>
## <a name="properties"></a><span data-ttu-id="1cef6-108">Properties</span><span class="sxs-lookup"><span data-stu-id="1cef6-108">Properties</span></span>
|<span data-ttu-id="1cef6-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1cef6-109">Property</span></span>|<span data-ttu-id="1cef6-110">種類</span><span class="sxs-lookup"><span data-stu-id="1cef6-110">Type</span></span>|<span data-ttu-id="1cef6-111">説明</span><span class="sxs-lookup"><span data-stu-id="1cef6-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1cef6-112">trustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="1cef6-112">trustedRootCertificate</span></span>|<span data-ttu-id="1cef6-113">Binary</span><span class="sxs-lookup"><span data-stu-id="1cef6-113">Binary</span></span>|<span data-ttu-id="1cef6-114">信頼されたルート証明書です。</span><span class="sxs-lookup"><span data-stu-id="1cef6-114">Trusted Root Certificate.</span></span>|
|<span data-ttu-id="1cef6-115">します</span><span class="sxs-lookup"><span data-stu-id="1cef6-115">certFileName</span></span>|<span data-ttu-id="1cef6-116">String</span><span class="sxs-lookup"><span data-stu-id="1cef6-116">String</span></span>|<span data-ttu-id="1cef6-117">UI に表示するファイル名です。</span><span class="sxs-lookup"><span data-stu-id="1cef6-117">File name to display in UI.</span></span>|
|<span data-ttu-id="1cef6-118">certificationAuthority</span><span class="sxs-lookup"><span data-stu-id="1cef6-118">certificationAuthority</span></span>|<span data-ttu-id="1cef6-119">String</span><span class="sxs-lookup"><span data-stu-id="1cef6-119">String</span></span>|<span data-ttu-id="1cef6-120">PKCS 証明機関。</span><span class="sxs-lookup"><span data-stu-id="1cef6-120">PKCS Certification Authority.</span></span>|
|<span data-ttu-id="1cef6-121">certificationAuthorityName</span><span class="sxs-lookup"><span data-stu-id="1cef6-121">certificationAuthorityName</span></span>|<span data-ttu-id="1cef6-122">String</span><span class="sxs-lookup"><span data-stu-id="1cef6-122">String</span></span>|<span data-ttu-id="1cef6-123">PKCS 証明機関の名前です。</span><span class="sxs-lookup"><span data-stu-id="1cef6-123">PKCS Certification Authority Name.</span></span>|
|<span data-ttu-id="1cef6-124">certificateTemplateName</span><span class="sxs-lookup"><span data-stu-id="1cef6-124">certificateTemplateName</span></span>|<span data-ttu-id="1cef6-125">String</span><span class="sxs-lookup"><span data-stu-id="1cef6-125">String</span></span>|<span data-ttu-id="1cef6-126">PKCS の証明書テンプレートの名前です。</span><span class="sxs-lookup"><span data-stu-id="1cef6-126">PKCS Certificate Template Name.</span></span>|
|<span data-ttu-id="1cef6-127">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="1cef6-127">renewalThresholdPercentage</span></span>|<span data-ttu-id="1cef6-128">Int32</span><span class="sxs-lookup"><span data-stu-id="1cef6-128">Int32</span></span>|<span data-ttu-id="1cef6-129">証明書の書き換えのしきい値の割合です。</span><span class="sxs-lookup"><span data-stu-id="1cef6-129">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="1cef6-130">1 から 99 までの有効な値</span><span class="sxs-lookup"><span data-stu-id="1cef6-130">Valid values 1 to 99</span></span>|
|<span data-ttu-id="1cef6-131">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="1cef6-131">certificateValidityPeriodValue</span></span>|<span data-ttu-id="1cef6-132">Int32</span><span class="sxs-lookup"><span data-stu-id="1cef6-132">Int32</span></span>|<span data-ttu-id="1cef6-133">証明書の有効期間の値です。</span><span class="sxs-lookup"><span data-stu-id="1cef6-133">Value for the Certificate Validity Period.</span></span>|
|<span data-ttu-id="1cef6-134">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="1cef6-134">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="1cef6-135">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="1cef6-135">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="1cef6-136">証明書の有効期間のスケールです。</span><span class="sxs-lookup"><span data-stu-id="1cef6-136">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="1cef6-137">可能な値は、`days`、`months`、`years` です。</span><span class="sxs-lookup"><span data-stu-id="1cef6-137">Possible values are: `days`, `months`, `years`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1cef6-138">関係</span><span class="sxs-lookup"><span data-stu-id="1cef6-138">Relationships</span></span>
<span data-ttu-id="1cef6-139">なし</span><span class="sxs-lookup"><span data-stu-id="1cef6-139">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="1cef6-140">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="1cef6-140">JSON Representation</span></span>
<span data-ttu-id="1cef6-141">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="1cef6-141">Here is a JSON representation of the resource.</span></span>
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





