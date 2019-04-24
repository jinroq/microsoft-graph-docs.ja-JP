---
title: リスト windows81CertificateProfileBases
description: windows81CertificateProfileBase オブジェクトのプロパティとリレーションシップをリストします。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b3becbc01cd0e9804bde108536ce5e7b0c1c485e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32515359"
---
# <a name="list-windows81certificateprofilebases"></a><span data-ttu-id="2379f-103">リスト windows81CertificateProfileBases</span><span class="sxs-lookup"><span data-stu-id="2379f-103">List windows81CertificateProfileBases</span></span>

> <span data-ttu-id="2379f-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2379f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2379f-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="2379f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2379f-106">[windows81CertificateProfileBase](../resources/intune-deviceconfig-windows81certificateprofilebase.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="2379f-106">List properties and relationships of the [windows81CertificateProfileBase](../resources/intune-deviceconfig-windows81certificateprofilebase.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2379f-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="2379f-107">Prerequisites</span></span>
<span data-ttu-id="2379f-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2379f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2379f-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="2379f-110">Permission type</span></span>|<span data-ttu-id="2379f-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="2379f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2379f-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="2379f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2379f-113">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="2379f-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="2379f-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="2379f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2379f-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2379f-115">Not supported.</span></span>|
|<span data-ttu-id="2379f-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="2379f-116">Application</span></span>|<span data-ttu-id="2379f-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2379f-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2379f-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="2379f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="2379f-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2379f-119">Request headers</span></span>
|<span data-ttu-id="2379f-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2379f-120">Header</span></span>|<span data-ttu-id="2379f-121">値</span><span class="sxs-lookup"><span data-stu-id="2379f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2379f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="2379f-122">Authorization</span></span>|<span data-ttu-id="2379f-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="2379f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2379f-124">承諾</span><span class="sxs-lookup"><span data-stu-id="2379f-124">Accept</span></span>|<span data-ttu-id="2379f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2379f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2379f-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="2379f-126">Request body</span></span>
<span data-ttu-id="2379f-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="2379f-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2379f-128">応答</span><span class="sxs-lookup"><span data-stu-id="2379f-128">Response</span></span>
<span data-ttu-id="2379f-129">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[windows81CertificateProfileBase](../resources/intune-deviceconfig-windows81certificateprofilebase.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="2379f-129">If successful, this method returns a `200 OK` response code and a collection of [windows81CertificateProfileBase](../resources/intune-deviceconfig-windows81certificateprofilebase.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2379f-130">例</span><span class="sxs-lookup"><span data-stu-id="2379f-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="2379f-131">要求</span><span class="sxs-lookup"><span data-stu-id="2379f-131">Request</span></span>
<span data-ttu-id="2379f-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="2379f-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="2379f-133">応答</span><span class="sxs-lookup"><span data-stu-id="2379f-133">Response</span></span>
<span data-ttu-id="2379f-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="2379f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1243

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windows81CertificateProfileBase",
      "id": "61cae8b8-e8b8-61ca-b8e8-ca61b8e8ca61",
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
      ],
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





