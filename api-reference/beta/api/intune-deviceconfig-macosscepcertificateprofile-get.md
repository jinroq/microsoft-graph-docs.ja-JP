---
title: MacOSScepCertificateProfile を取得します。
description: MacOSScepCertificateProfile オブジェクトのプロパティと関係を参照してください。
author: tfitzmac
ms.openlocfilehash: 5f44b0eae6f7a1c38897d9f90737c58f5d5e2c8a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27330115"
---
# <a name="get-macosscepcertificateprofile"></a><span data-ttu-id="00767-103">MacOSScepCertificateProfile を取得します。</span><span class="sxs-lookup"><span data-stu-id="00767-103">Get macOSScepCertificateProfile</span></span>

> <span data-ttu-id="00767-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="00767-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="00767-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="00767-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="00767-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="00767-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="00767-107">[MacOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md)オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="00767-107">Read properties and relationships of the [macOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="00767-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="00767-108">Prerequisites</span></span>
<span data-ttu-id="00767-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="00767-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="00767-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="00767-111">Permission type</span></span>|<span data-ttu-id="00767-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="00767-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="00767-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="00767-113">Delegated (work or school account)</span></span>|<span data-ttu-id="00767-114">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="00767-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="00767-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="00767-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="00767-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="00767-116">Not supported.</span></span>|
|<span data-ttu-id="00767-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="00767-117">Application</span></span>|<span data-ttu-id="00767-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="00767-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="00767-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="00767-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="00767-120">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="00767-120">Optional query parameters</span></span>
<span data-ttu-id="00767-121">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="00767-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="00767-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="00767-122">Request headers</span></span>
|<span data-ttu-id="00767-123">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="00767-123">Header</span></span>|<span data-ttu-id="00767-124">値</span><span class="sxs-lookup"><span data-stu-id="00767-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="00767-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="00767-125">Authorization</span></span>|<span data-ttu-id="00767-126">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="00767-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="00767-127">Accept</span><span class="sxs-lookup"><span data-stu-id="00767-127">Accept</span></span>|<span data-ttu-id="00767-128">application/json</span><span class="sxs-lookup"><span data-stu-id="00767-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="00767-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="00767-129">Request body</span></span>
<span data-ttu-id="00767-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="00767-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="00767-131">応答</span><span class="sxs-lookup"><span data-stu-id="00767-131">Response</span></span>
<span data-ttu-id="00767-132">かどうかは成功すると、このメソッドが返されます、 `200 OK` 、応答の本体で応答コードと[macOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md)のオブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="00767-132">If successful, this method returns a `200 OK` response code and [macOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="00767-133">例</span><span class="sxs-lookup"><span data-stu-id="00767-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="00767-134">要求</span><span class="sxs-lookup"><span data-stu-id="00767-134">Request</span></span>
<span data-ttu-id="00767-135">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="00767-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="00767-136">応答</span><span class="sxs-lookup"><span data-stu-id="00767-136">Response</span></span>
<span data-ttu-id="00767-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="00767-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1218

{
  "value": {
    "@odata.type": "#microsoft.graph.macOSScepCertificateProfile",
    "id": "78c3929d-929d-78c3-9d92-c3789d92c378",
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
    "hashAlgorithm": "sha2",
    "extendedKeyUsages": [
      {
        "@odata.type": "microsoft.graph.extendedKeyUsage",
        "name": "Name value",
        "objectIdentifier": "Object Identifier value"
      }
    ],
    "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value"
  }
}
```





