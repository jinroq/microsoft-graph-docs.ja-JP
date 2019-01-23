---
title: ManagedDeviceCertificateState を取得します。
description: ManagedDeviceCertificateState オブジェクトのプロパティと関係を参照してください。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: a38731606957ade6c718b030045b236636f5acbf
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29403792"
---
# <a name="get-manageddevicecertificatestate"></a><span data-ttu-id="bc2f1-103">ManagedDeviceCertificateState を取得します。</span><span class="sxs-lookup"><span data-stu-id="bc2f1-103">Get managedDeviceCertificateState</span></span>

> <span data-ttu-id="bc2f1-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="bc2f1-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="bc2f1-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bc2f1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bc2f1-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="bc2f1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bc2f1-107">[ManagedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md)オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="bc2f1-107">Read properties and relationships of the [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bc2f1-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="bc2f1-108">Prerequisites</span></span>
<span data-ttu-id="bc2f1-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="bc2f1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="bc2f1-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="bc2f1-111">Permission type</span></span>|<span data-ttu-id="bc2f1-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="bc2f1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bc2f1-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="bc2f1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="bc2f1-114">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="bc2f1-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="bc2f1-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="bc2f1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bc2f1-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bc2f1-116">Not supported.</span></span>|
|<span data-ttu-id="bc2f1-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="bc2f1-117">Application</span></span>|<span data-ttu-id="bc2f1-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bc2f1-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bc2f1-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="bc2f1-119">HTTP Request</span></span>
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

## <a name="optional-query-parameters"></a><span data-ttu-id="bc2f1-120">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="bc2f1-120">Optional query parameters</span></span>
<span data-ttu-id="bc2f1-121">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://docs.microsoft.com/en-us/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="bc2f1-121">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bc2f1-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="bc2f1-122">Request headers</span></span>
|<span data-ttu-id="bc2f1-123">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="bc2f1-123">Header</span></span>|<span data-ttu-id="bc2f1-124">値</span><span class="sxs-lookup"><span data-stu-id="bc2f1-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bc2f1-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="bc2f1-125">Authorization</span></span>|<span data-ttu-id="bc2f1-126">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="bc2f1-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bc2f1-127">Accept</span><span class="sxs-lookup"><span data-stu-id="bc2f1-127">Accept</span></span>|<span data-ttu-id="bc2f1-128">application/json</span><span class="sxs-lookup"><span data-stu-id="bc2f1-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bc2f1-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="bc2f1-129">Request body</span></span>
<span data-ttu-id="bc2f1-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="bc2f1-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bc2f1-131">応答</span><span class="sxs-lookup"><span data-stu-id="bc2f1-131">Response</span></span>
<span data-ttu-id="bc2f1-132">かどうかは成功すると、このメソッドが返されます、 `200 OK` 、応答の本体で応答コードと[managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md)のオブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="bc2f1-132">If successful, this method returns a `200 OK` response code and [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bc2f1-133">例</span><span class="sxs-lookup"><span data-stu-id="bc2f1-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="bc2f1-134">要求</span><span class="sxs-lookup"><span data-stu-id="bc2f1-134">Request</span></span>
<span data-ttu-id="bc2f1-135">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="bc2f1-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosPkcsCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
```

### <a name="response"></a><span data-ttu-id="bc2f1-136">応答</span><span class="sxs-lookup"><span data-stu-id="bc2f1-136">Response</span></span>
<span data-ttu-id="bc2f1-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="bc2f1-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




