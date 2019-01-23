---
title: WindowsPhone81CertificateProfileBase を取得します。
description: WindowsPhone81CertificateProfileBase オブジェクトのプロパティと関係を参照してください。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: a416dc1f9c4bf2f12e9983b96aa7f041e854add9
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29408062"
---
# <a name="get-windowsphone81certificateprofilebase"></a><span data-ttu-id="161bc-103">WindowsPhone81CertificateProfileBase を取得します。</span><span class="sxs-lookup"><span data-stu-id="161bc-103">Get windowsPhone81CertificateProfileBase</span></span>

> <span data-ttu-id="161bc-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="161bc-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="161bc-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="161bc-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="161bc-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="161bc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="161bc-107">[WindowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="161bc-107">Read properties and relationships of the [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="161bc-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="161bc-108">Prerequisites</span></span>
<span data-ttu-id="161bc-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="161bc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="161bc-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="161bc-111">Permission type</span></span>|<span data-ttu-id="161bc-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="161bc-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="161bc-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="161bc-113">Delegated (work or school account)</span></span>|<span data-ttu-id="161bc-114">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="161bc-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="161bc-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="161bc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="161bc-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="161bc-116">Not supported.</span></span>|
|<span data-ttu-id="161bc-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="161bc-117">Application</span></span>|<span data-ttu-id="161bc-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="161bc-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="161bc-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="161bc-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate
```

## <a name="optional-query-parameters"></a><span data-ttu-id="161bc-120">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="161bc-120">Optional query parameters</span></span>
<span data-ttu-id="161bc-121">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://docs.microsoft.com/en-us/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="161bc-121">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="161bc-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="161bc-122">Request headers</span></span>
|<span data-ttu-id="161bc-123">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="161bc-123">Header</span></span>|<span data-ttu-id="161bc-124">値</span><span class="sxs-lookup"><span data-stu-id="161bc-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="161bc-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="161bc-125">Authorization</span></span>|<span data-ttu-id="161bc-126">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="161bc-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="161bc-127">Accept</span><span class="sxs-lookup"><span data-stu-id="161bc-127">Accept</span></span>|<span data-ttu-id="161bc-128">application/json</span><span class="sxs-lookup"><span data-stu-id="161bc-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="161bc-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="161bc-129">Request body</span></span>
<span data-ttu-id="161bc-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="161bc-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="161bc-131">応答</span><span class="sxs-lookup"><span data-stu-id="161bc-131">Response</span></span>
<span data-ttu-id="161bc-132">かどうかは成功すると、このメソッドが返されます、 `200 OK` 、応答の本体で応答コードと[windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)のオブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="161bc-132">If successful, this method returns a `200 OK` response code and [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="161bc-133">例</span><span class="sxs-lookup"><span data-stu-id="161bc-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="161bc-134">要求</span><span class="sxs-lookup"><span data-stu-id="161bc-134">Request</span></span>
<span data-ttu-id="161bc-135">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="161bc-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate
```

### <a name="response"></a><span data-ttu-id="161bc-136">応答</span><span class="sxs-lookup"><span data-stu-id="161bc-136">Response</span></span>
<span data-ttu-id="161bc-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="161bc-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 968

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsPhone81CertificateProfileBase",
    "id": "336e97ac-97ac-336e-ac97-6e33ac976e33",
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
    "certificateValidityPeriodScale": "months",
    "extendedKeyUsages": [
      {
        "@odata.type": "microsoft.graph.extendedKeyUsage",
        "name": "Name value",
        "objectIdentifier": "Object Identifier value"
      }
    ]
  }
}
```




