---
title: リスト androidWorkProfilePkcsCertificateProfiles
description: AndroidWorkProfilePkcsCertificateProfile オブジェクトのプロパティと関係を一覧表示します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 68f89a766929bdf85356002c35d93b85a155c876
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27958069"
---
# <a name="list-androidworkprofilepkcscertificateprofiles"></a><span data-ttu-id="23aef-103">リスト androidWorkProfilePkcsCertificateProfiles</span><span class="sxs-lookup"><span data-stu-id="23aef-103">List androidWorkProfilePkcsCertificateProfiles</span></span>

> <span data-ttu-id="23aef-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="23aef-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="23aef-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="23aef-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="23aef-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="23aef-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="23aef-107">[AndroidWorkProfilePkcsCertificateProfile](../resources/intune-deviceconfig-androidworkprofilepkcscertificateprofile.md)オブジェクトのプロパティと関係を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="23aef-107">List properties and relationships of the [androidWorkProfilePkcsCertificateProfile](../resources/intune-deviceconfig-androidworkprofilepkcscertificateprofile.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="23aef-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="23aef-108">Prerequisites</span></span>
<span data-ttu-id="23aef-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="23aef-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="23aef-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="23aef-111">Permission type</span></span>|<span data-ttu-id="23aef-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="23aef-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="23aef-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="23aef-113">Delegated (work or school account)</span></span>|<span data-ttu-id="23aef-114">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="23aef-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="23aef-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="23aef-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="23aef-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="23aef-116">Not supported.</span></span>|
|<span data-ttu-id="23aef-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="23aef-117">Application</span></span>|<span data-ttu-id="23aef-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="23aef-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="23aef-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="23aef-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="23aef-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="23aef-120">Request headers</span></span>
|<span data-ttu-id="23aef-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="23aef-121">Header</span></span>|<span data-ttu-id="23aef-122">値</span><span class="sxs-lookup"><span data-stu-id="23aef-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="23aef-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="23aef-123">Authorization</span></span>|<span data-ttu-id="23aef-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="23aef-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="23aef-125">Accept</span><span class="sxs-lookup"><span data-stu-id="23aef-125">Accept</span></span>|<span data-ttu-id="23aef-126">application/json</span><span class="sxs-lookup"><span data-stu-id="23aef-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="23aef-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="23aef-127">Request body</span></span>
<span data-ttu-id="23aef-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="23aef-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="23aef-129">応答</span><span class="sxs-lookup"><span data-stu-id="23aef-129">Response</span></span>
<span data-ttu-id="23aef-130">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に[androidWorkProfilePkcsCertificateProfile](../resources/intune-deviceconfig-androidworkprofilepkcscertificateprofile.md)オブジェクトのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="23aef-130">If successful, this method returns a `200 OK` response code and a collection of [androidWorkProfilePkcsCertificateProfile](../resources/intune-deviceconfig-androidworkprofilepkcscertificateprofile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="23aef-131">例</span><span class="sxs-lookup"><span data-stu-id="23aef-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="23aef-132">要求</span><span class="sxs-lookup"><span data-stu-id="23aef-132">Request</span></span>
<span data-ttu-id="23aef-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="23aef-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="23aef-134">応答</span><span class="sxs-lookup"><span data-stu-id="23aef-134">Response</span></span>
<span data-ttu-id="23aef-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="23aef-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1282

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.androidWorkProfilePkcsCertificateProfile",
      "id": "a7d4a505-a505-a7d4-05a5-d4a705a5d4a7",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "supportsScopeTags": true,
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "displayName": "Display Name value",
      "version": 7,
      "renewalThresholdPercentage": 10,
      "subjectNameFormat": "commonNameIncludingEmail",
      "certificateValidityPeriodValue": 14,
      "certificateValidityPeriodScale": "months",
      "extendedKeyUsages": [
        {
          "@odata.type": "microsoft.graph.extendedKeyUsage",
          "name": "Name value",
          "objectIdentifier": "Object Identifier value"
        }
      ],
      "certificationAuthority": "Certification Authority value",
      "certificationAuthorityName": "Certification Authority Name value",
      "certificateTemplateName": "Certificate Template Name value",
      "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value",
      "subjectAlternativeNameType": "emailAddress"
    }
  ]
}
```





