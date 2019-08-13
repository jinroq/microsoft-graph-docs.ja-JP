---
title: ManagedDeviceCertificateState を取得する
description: ManagedDeviceCertificateState オブジェクトのプロパティとリレーションシップを読み取ります。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b73bf54cc6126671615b710a24a5455ddf548d99
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36345597"
---
# <a name="get-manageddevicecertificatestate"></a><span data-ttu-id="4b1ed-103">ManagedDeviceCertificateState を取得する</span><span class="sxs-lookup"><span data-stu-id="4b1ed-103">Get managedDeviceCertificateState</span></span>

> <span data-ttu-id="4b1ed-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4b1ed-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4b1ed-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="4b1ed-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4b1ed-106">[ManagedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="4b1ed-106">Read properties and relationships of the [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4b1ed-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="4b1ed-107">Prerequisites</span></span>
<span data-ttu-id="4b1ed-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4b1ed-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4b1ed-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="4b1ed-110">Permission type</span></span>|<span data-ttu-id="4b1ed-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="4b1ed-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4b1ed-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="4b1ed-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4b1ed-113">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="4b1ed-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="4b1ed-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="4b1ed-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4b1ed-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4b1ed-115">Not supported.</span></span>|
|<span data-ttu-id="4b1ed-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="4b1ed-116">Application</span></span>|<span data-ttu-id="4b1ed-117">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="4b1ed-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4b1ed-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="4b1ed-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosPkcsCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSScepCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidPkcsCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidScepCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosImportedPFXCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSImportedPFXCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidImportedPFXCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidWorkProfileScepCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidForWorkImportedPFXCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/microsoft.graph.androidForWorkPkcsCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/microsoft.graph.androidForWorkScepCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/microsoft.graph.windowsPhone81SCEPCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windows10PkcsCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windows81SCEPCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windows10ImportedPFXCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windowsPhone81ImportedPFXCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4b1ed-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="4b1ed-119">Optional query parameters</span></span>
<span data-ttu-id="4b1ed-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://docs.microsoft.com/en-us/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="4b1ed-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4b1ed-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4b1ed-121">Request headers</span></span>
|<span data-ttu-id="4b1ed-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4b1ed-122">Header</span></span>|<span data-ttu-id="4b1ed-123">値</span><span class="sxs-lookup"><span data-stu-id="4b1ed-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4b1ed-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="4b1ed-124">Authorization</span></span>|<span data-ttu-id="4b1ed-125">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="4b1ed-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4b1ed-126">承諾</span><span class="sxs-lookup"><span data-stu-id="4b1ed-126">Accept</span></span>|<span data-ttu-id="4b1ed-127">application/json</span><span class="sxs-lookup"><span data-stu-id="4b1ed-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4b1ed-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="4b1ed-128">Request body</span></span>
<span data-ttu-id="4b1ed-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="4b1ed-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4b1ed-130">応答</span><span class="sxs-lookup"><span data-stu-id="4b1ed-130">Response</span></span>
<span data-ttu-id="4b1ed-131">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="4b1ed-131">If successful, this method returns a `200 OK` response code and [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4b1ed-132">例</span><span class="sxs-lookup"><span data-stu-id="4b1ed-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="4b1ed-133">要求</span><span class="sxs-lookup"><span data-stu-id="4b1ed-133">Request</span></span>
<span data-ttu-id="4b1ed-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="4b1ed-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosPkcsCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
```

### <a name="response"></a><span data-ttu-id="4b1ed-135">応答</span><span class="sxs-lookup"><span data-stu-id="4b1ed-135">Response</span></span>
<span data-ttu-id="4b1ed-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="4b1ed-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1637

{
  "value": {
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
}
```






