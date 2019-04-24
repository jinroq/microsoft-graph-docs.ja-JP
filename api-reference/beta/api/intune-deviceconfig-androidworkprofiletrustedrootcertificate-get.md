---
title: androidwork profiletrustedrootcertificate の取得
description: androidwork profiletrustedrootcertificate オブジェクトのプロパティとリレーションシップを読み取ります。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f5aeb5b16e5cb58f7d2820df1af7960a26b7154d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32472765"
---
# <a name="get-androidworkprofiletrustedrootcertificate"></a><span data-ttu-id="7549c-103">androidwork profiletrustedrootcertificate の取得</span><span class="sxs-lookup"><span data-stu-id="7549c-103">Get androidWorkProfileTrustedRootCertificate</span></span>

> <span data-ttu-id="7549c-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7549c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7549c-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="7549c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7549c-106">[androidwork profiletrustedrootcertificate](../resources/intune-deviceconfig-androidworkprofiletrustedrootcertificate.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="7549c-106">Read properties and relationships of the [androidWorkProfileTrustedRootCertificate](../resources/intune-deviceconfig-androidworkprofiletrustedrootcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7549c-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="7549c-107">Prerequisites</span></span>
<span data-ttu-id="7549c-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7549c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7549c-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7549c-110">Permission type</span></span>|<span data-ttu-id="7549c-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="7549c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7549c-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7549c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7549c-113">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="7549c-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="7549c-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7549c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7549c-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7549c-115">Not supported.</span></span>|
|<span data-ttu-id="7549c-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7549c-116">Application</span></span>|<span data-ttu-id="7549c-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7549c-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7549c-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7549c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/rootCertificate
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidWorkProfileCertificateProfileBase/rootCertificate
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidWorkProfileEnterpriseWiFiConfiguration/rootCertificateForServerValidation
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7549c-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="7549c-119">Optional query parameters</span></span>
<span data-ttu-id="7549c-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://docs.microsoft.com/en-us/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="7549c-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7549c-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7549c-121">Request headers</span></span>
|<span data-ttu-id="7549c-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7549c-122">Header</span></span>|<span data-ttu-id="7549c-123">値</span><span class="sxs-lookup"><span data-stu-id="7549c-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7549c-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="7549c-124">Authorization</span></span>|<span data-ttu-id="7549c-125">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="7549c-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7549c-126">承諾</span><span class="sxs-lookup"><span data-stu-id="7549c-126">Accept</span></span>|<span data-ttu-id="7549c-127">application/json</span><span class="sxs-lookup"><span data-stu-id="7549c-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7549c-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="7549c-128">Request body</span></span>
<span data-ttu-id="7549c-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="7549c-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7549c-130">応答</span><span class="sxs-lookup"><span data-stu-id="7549c-130">Response</span></span>
<span data-ttu-id="7549c-131">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[androidwork profiletrustedrootcertificate](../resources/intune-deviceconfig-androidworkprofiletrustedrootcertificate.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="7549c-131">If successful, this method returns a `200 OK` response code and [androidWorkProfileTrustedRootCertificate](../resources/intune-deviceconfig-androidworkprofiletrustedrootcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7549c-132">例</span><span class="sxs-lookup"><span data-stu-id="7549c-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="7549c-133">要求</span><span class="sxs-lookup"><span data-stu-id="7549c-133">Request</span></span>
<span data-ttu-id="7549c-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="7549c-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/rootCertificate
```

### <a name="response"></a><span data-ttu-id="7549c-135">応答</span><span class="sxs-lookup"><span data-stu-id="7549c-135">Response</span></span>
<span data-ttu-id="7549c-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="7549c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 595

{
  "value": {
    "@odata.type": "#microsoft.graph.androidWorkProfileTrustedRootCertificate",
    "id": "37cc7454-7454-37cc-5474-cc375474cc37",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "supportsScopeTags": true,
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "displayName": "Display Name value",
    "version": 7,
    "trustedRootCertificate": "dHJ1c3RlZFJvb3RDZXJ0aWZpY2F0ZQ==",
    "certFileName": "Cert File Name value"
  }
}
```





