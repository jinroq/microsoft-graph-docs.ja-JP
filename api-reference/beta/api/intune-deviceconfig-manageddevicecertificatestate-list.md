---
title: リスト managedDeviceCertificateStates
description: ManagedDeviceCertificateState オブジェクトのプロパティと関係を一覧表示します。
ms.openlocfilehash: 7cc5d4f2a1aed40ebb9ea6e40298b435aad58485
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27072299"
---
# <a name="list-manageddevicecertificatestates"></a><span data-ttu-id="dc61c-103">リスト managedDeviceCertificateStates</span><span class="sxs-lookup"><span data-stu-id="dc61c-103">List managedDeviceCertificateStates</span></span>

> <span data-ttu-id="dc61c-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="dc61c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="dc61c-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="dc61c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="dc61c-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="dc61c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="dc61c-107">[ManagedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md)オブジェクトのプロパティと関係を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="dc61c-107">List properties and relationships of the [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="dc61c-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="dc61c-108">Prerequisites</span></span>
<span data-ttu-id="dc61c-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="dc61c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dc61c-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="dc61c-111">Permission type</span></span>|<span data-ttu-id="dc61c-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="dc61c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dc61c-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="dc61c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="dc61c-114">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="dc61c-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="dc61c-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="dc61c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dc61c-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="dc61c-116">Not supported.</span></span>|
|<span data-ttu-id="dc61c-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="dc61c-117">Application</span></span>|<span data-ttu-id="dc61c-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="dc61c-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="dc61c-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="dc61c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosPkcsCertificateProfile/managedDeviceCertificateStates
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/managedDeviceCertificateStates
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSScepCertificateProfile/managedDeviceCertificateStates
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidPkcsCertificateProfile/managedDeviceCertificateStates
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidScepCertificateProfile/managedDeviceCertificateStates
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosImportedPFXCertificateProfile/managedDeviceCertificateStates
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSImportedPFXCertificateProfile/managedDeviceCertificateStates
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidImportedPFXCertificateProfile/managedDeviceCertificateStates
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidWorkProfileScepCertificateProfile/managedDeviceCertificateStates
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidForWorkImportedPFXCertificateProfile/managedDeviceCertificateStates
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/microsoft.graph.androidForWorkPkcsCertificateProfile/managedDeviceCertificateStates
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/microsoft.graph.androidForWorkScepCertificateProfile/managedDeviceCertificateStates
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/microsoft.graph.windowsPhone81SCEPCertificateProfile/managedDeviceCertificateStates
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windows10PkcsCertificateProfile/managedDeviceCertificateStates
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windows81SCEPCertificateProfile/managedDeviceCertificateStates
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windows10ImportedPFXCertificateProfile/managedDeviceCertificateStates
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windowsPhone81ImportedPFXCertificateProfile/managedDeviceCertificateStates
```

## <a name="request-headers"></a><span data-ttu-id="dc61c-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="dc61c-120">Request headers</span></span>
|<span data-ttu-id="dc61c-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="dc61c-121">Header</span></span>|<span data-ttu-id="dc61c-122">値</span><span class="sxs-lookup"><span data-stu-id="dc61c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dc61c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="dc61c-123">Authorization</span></span>|<span data-ttu-id="dc61c-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="dc61c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dc61c-125">Accept</span><span class="sxs-lookup"><span data-stu-id="dc61c-125">Accept</span></span>|<span data-ttu-id="dc61c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="dc61c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dc61c-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="dc61c-127">Request body</span></span>
<span data-ttu-id="dc61c-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="dc61c-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dc61c-129">応答</span><span class="sxs-lookup"><span data-stu-id="dc61c-129">Response</span></span>
<span data-ttu-id="dc61c-130">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に[managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md)オブジェクトのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="dc61c-130">If successful, this method returns a `200 OK` response code and a collection of [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dc61c-131">例</span><span class="sxs-lookup"><span data-stu-id="dc61c-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="dc61c-132">要求</span><span class="sxs-lookup"><span data-stu-id="dc61c-132">Request</span></span>
<span data-ttu-id="dc61c-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="dc61c-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosPkcsCertificateProfile/managedDeviceCertificateStates
```

### <a name="response"></a><span data-ttu-id="dc61c-134">応答</span><span class="sxs-lookup"><span data-stu-id="dc61c-134">Response</span></span>
<span data-ttu-id="dc61c-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="dc61c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1703

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedDeviceCertificateState",
      "id": "d99bc884-c884-d99b-84c8-9bd984c89bd9",
      "devicePlatform": "androidForWork",
      "certificateKeyUsage": "digitalSignature",
      "certificateValidityPeriodUnits": "months",
      "certificateIssuanceState": "challengeIssued",
      "certificateKeyStorageProvider": "useTpmKspOtherwiseFail",
      "certificateSubjectNameFormat": "commonNameIncludingEmail",
      "certificateSubjectAlternativeNameFormat": "emailAddress",
      "certificateRevokeStatus": "pending",
      "certificateProfileDisplayName": "Certificate Profile Display Name value",
      "deviceDisplayName": "Device Display Name value",
      "userDisplayName": "User Display Name value",
      "certificateExpirationDateTime": "2017-01-01T00:02:14.9489247-08:00",
      "certificateLastIssuanceStateChangedDateTime": "2017-01-01T00:00:27.7468732-08:00",
      "lastCertificateStateChangeDateTime": "2017-01-01T00:01:10.7144639-08:00",
      "certificateIssuer": "Certificate Issuer value",
      "certificateThumbprint": "Certificate Thumbprint value",
      "certificateSerialNumber": "Certificate Serial Number value",
      "certificateKeyLength": 4,
      "certificateEnhancedKeyUsage": "Certificate Enhanced Key Usage value",
      "certificateValidityPeriod": 9,
      "certificateSubjectNameFormatString": "Certificate Subject Name Format String value",
      "certificateSubjectAlternativeNameFormatString": "Certificate Subject Alternative Name Format String value",
      "certificateIssuanceDateTime": "2016-12-31T23:59:41.5044473-08:00",
      "certificateErrorCode": 4
    }
  ]
}
```





