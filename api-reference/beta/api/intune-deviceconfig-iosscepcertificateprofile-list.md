---
title: リスト iosScepCertificateProfiles
description: IosScepCertificateProfile オブジェクトのプロパティと関係を一覧表示します。
ms.openlocfilehash: 7b8772fc8e2c69d073c728f8d897773b53ca6f9e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27072298"
---
# <a name="list-iosscepcertificateprofiles"></a><span data-ttu-id="a3992-103">リスト iosScepCertificateProfiles</span><span class="sxs-lookup"><span data-stu-id="a3992-103">List iosScepCertificateProfiles</span></span>

> <span data-ttu-id="a3992-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="a3992-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a3992-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a3992-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a3992-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="a3992-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a3992-107">[IosScepCertificateProfile](../resources/intune-deviceconfig-iosscepcertificateprofile.md)オブジェクトのプロパティと関係を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="a3992-107">List properties and relationships of the [iosScepCertificateProfile](../resources/intune-deviceconfig-iosscepcertificateprofile.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a3992-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="a3992-108">Prerequisites</span></span>
<span data-ttu-id="a3992-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a3992-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a3992-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a3992-111">Permission type</span></span>|<span data-ttu-id="a3992-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="a3992-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a3992-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a3992-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a3992-114">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="a3992-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="a3992-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a3992-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a3992-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a3992-116">Not supported.</span></span>|
|<span data-ttu-id="a3992-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a3992-117">Application</span></span>|<span data-ttu-id="a3992-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a3992-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a3992-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a3992-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="a3992-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a3992-120">Request headers</span></span>
|<span data-ttu-id="a3992-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a3992-121">Header</span></span>|<span data-ttu-id="a3992-122">値</span><span class="sxs-lookup"><span data-stu-id="a3992-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a3992-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a3992-123">Authorization</span></span>|<span data-ttu-id="a3992-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="a3992-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a3992-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a3992-125">Accept</span></span>|<span data-ttu-id="a3992-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a3992-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a3992-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="a3992-127">Request body</span></span>
<span data-ttu-id="a3992-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="a3992-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a3992-129">応答</span><span class="sxs-lookup"><span data-stu-id="a3992-129">Response</span></span>
<span data-ttu-id="a3992-130">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に[iosScepCertificateProfile](../resources/intune-deviceconfig-iosscepcertificateprofile.md)オブジェクトのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="a3992-130">If successful, this method returns a `200 OK` response code and a collection of [iosScepCertificateProfile](../resources/intune-deviceconfig-iosscepcertificateprofile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a3992-131">例</span><span class="sxs-lookup"><span data-stu-id="a3992-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="a3992-132">要求</span><span class="sxs-lookup"><span data-stu-id="a3992-132">Request</span></span>
<span data-ttu-id="a3992-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="a3992-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="a3992-134">応答</span><span class="sxs-lookup"><span data-stu-id="a3992-134">Response</span></span>
<span data-ttu-id="a3992-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="a3992-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1516

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.iosScepCertificateProfile",
      "id": "0deb8dbf-8dbf-0deb-bf8d-eb0dbf8deb0d",
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
      "subjectNameFormat": "commonNameAsEmail",
      "subjectAlternativeNameType": "emailAddress",
      "certificateValidityPeriodValue": 14,
      "certificateValidityPeriodScale": "months",
      "scepServerUrls": [
        "Scep Server Urls value"
      ],
      "subjectNameFormatString": "Subject Name Format String value",
      "keyUsage": "digitalSignature",
      "keySize": "size2048",
      "extendedKeyUsages": [
        {
          "@odata.type": "microsoft.graph.extendedKeyUsage",
          "name": "Name value",
          "objectIdentifier": "Object Identifier value"
        }
      ],
      "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value",
      "certificateStore": "machine",
      "customSubjectAlternativeNames": [
        {
          "@odata.type": "microsoft.graph.customSubjectAlternativeName",
          "sanType": "emailAddress",
          "name": "Name value"
        }
      ]
    }
  ]
}
```





