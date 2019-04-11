---
title: windowscertificateprofilebase を取得する
description: windowscertificateprofilebase オブジェクトのプロパティとリレーションシップを読み取ります。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: dc404b3a784dde62ca38aaa53d2c0140164260a9
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31798566"
---
# <a name="get-windowscertificateprofilebase"></a><span data-ttu-id="148f0-103">windowscertificateprofilebase を取得する</span><span class="sxs-lookup"><span data-stu-id="148f0-103">Get windowsCertificateProfileBase</span></span>

> <span data-ttu-id="148f0-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="148f0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="148f0-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="148f0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="148f0-106">[windowscertificateprofilebase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="148f0-106">Read properties and relationships of the [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="148f0-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="148f0-107">Prerequisites</span></span>
<span data-ttu-id="148f0-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="148f0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="148f0-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="148f0-110">Permission type</span></span>|<span data-ttu-id="148f0-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="148f0-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="148f0-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="148f0-112">Delegated (work or school account)</span></span>|<span data-ttu-id="148f0-113">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="148f0-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="148f0-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="148f0-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="148f0-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="148f0-115">Not supported.</span></span>|
|<span data-ttu-id="148f0-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="148f0-116">Application</span></span>|<span data-ttu-id="148f0-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="148f0-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="148f0-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="148f0-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windows10VpnConfiguration/identityCertificate
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication
```

## <a name="optional-query-parameters"></a><span data-ttu-id="148f0-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="148f0-119">Optional query parameters</span></span>
<span data-ttu-id="148f0-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://docs.microsoft.com/en-us/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="148f0-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="148f0-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="148f0-121">Request headers</span></span>
|<span data-ttu-id="148f0-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="148f0-122">Header</span></span>|<span data-ttu-id="148f0-123">値</span><span class="sxs-lookup"><span data-stu-id="148f0-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="148f0-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="148f0-124">Authorization</span></span>|<span data-ttu-id="148f0-125">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="148f0-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="148f0-126">承諾</span><span class="sxs-lookup"><span data-stu-id="148f0-126">Accept</span></span>|<span data-ttu-id="148f0-127">application/json</span><span class="sxs-lookup"><span data-stu-id="148f0-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="148f0-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="148f0-128">Request body</span></span>
<span data-ttu-id="148f0-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="148f0-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="148f0-130">応答</span><span class="sxs-lookup"><span data-stu-id="148f0-130">Response</span></span>
<span data-ttu-id="148f0-131">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[windowscertificateprofilebase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="148f0-131">If successful, this method returns a `200 OK` response code and [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="148f0-132">例</span><span class="sxs-lookup"><span data-stu-id="148f0-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="148f0-133">要求</span><span class="sxs-lookup"><span data-stu-id="148f0-133">Request</span></span>
<span data-ttu-id="148f0-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="148f0-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windows10VpnConfiguration/identityCertificate
```

### <a name="response"></a><span data-ttu-id="148f0-135">応答</span><span class="sxs-lookup"><span data-stu-id="148f0-135">Response</span></span>
<span data-ttu-id="148f0-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="148f0-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 761

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsCertificateProfileBase",
    "id": "c0979ce1-9ce1-c097-e19c-97c0e19c97c0",
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
    "keyStorageProvider": "useTpmKspOtherwiseFail",
    "subjectNameFormat": "commonNameIncludingEmail",
    "subjectAlternativeNameType": "emailAddress",
    "certificateValidityPeriodValue": 14,
    "certificateValidityPeriodScale": "months"
  }
}
```





