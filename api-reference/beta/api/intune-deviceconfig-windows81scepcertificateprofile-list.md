---
title: リスト windows81SCEPCertificateProfiles
description: windows81SCEPCertificateProfile オブジェクトのプロパティとリレーションシップをリストします。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7d29d7b29775d007289039ee98c7f05d1c19d298
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/29/2019
ms.locfileid: "30972348"
---
# <a name="list-windows81scepcertificateprofiles"></a><span data-ttu-id="208ee-103">リスト windows81SCEPCertificateProfiles</span><span class="sxs-lookup"><span data-stu-id="208ee-103">List windows81SCEPCertificateProfiles</span></span>

> <span data-ttu-id="208ee-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="208ee-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="208ee-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="208ee-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="208ee-106">[windows81SCEPCertificateProfile](../resources/intune-deviceconfig-windows81scepcertificateprofile.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="208ee-106">List properties and relationships of the [windows81SCEPCertificateProfile](../resources/intune-deviceconfig-windows81scepcertificateprofile.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="208ee-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="208ee-107">Prerequisites</span></span>
<span data-ttu-id="208ee-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="208ee-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="208ee-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="208ee-110">Permission type</span></span>|<span data-ttu-id="208ee-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="208ee-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="208ee-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="208ee-112">Delegated (work or school account)</span></span>|<span data-ttu-id="208ee-113">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="208ee-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="208ee-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="208ee-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="208ee-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="208ee-115">Not supported.</span></span>|
|<span data-ttu-id="208ee-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="208ee-116">Application</span></span>|<span data-ttu-id="208ee-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="208ee-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="208ee-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="208ee-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="208ee-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="208ee-119">Request headers</span></span>
|<span data-ttu-id="208ee-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="208ee-120">Header</span></span>|<span data-ttu-id="208ee-121">値</span><span class="sxs-lookup"><span data-stu-id="208ee-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="208ee-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="208ee-122">Authorization</span></span>|<span data-ttu-id="208ee-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="208ee-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="208ee-124">承諾</span><span class="sxs-lookup"><span data-stu-id="208ee-124">Accept</span></span>|<span data-ttu-id="208ee-125">application/json</span><span class="sxs-lookup"><span data-stu-id="208ee-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="208ee-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="208ee-126">Request body</span></span>
<span data-ttu-id="208ee-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="208ee-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="208ee-128">応答</span><span class="sxs-lookup"><span data-stu-id="208ee-128">Response</span></span>
<span data-ttu-id="208ee-129">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[windows81SCEPCertificateProfile](../resources/intune-deviceconfig-windows81scepcertificateprofile.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="208ee-129">If successful, this method returns a `200 OK` response code and a collection of [windows81SCEPCertificateProfile](../resources/intune-deviceconfig-windows81scepcertificateprofile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="208ee-130">例</span><span class="sxs-lookup"><span data-stu-id="208ee-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="208ee-131">要求</span><span class="sxs-lookup"><span data-stu-id="208ee-131">Request</span></span>
<span data-ttu-id="208ee-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="208ee-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="208ee-133">応答</span><span class="sxs-lookup"><span data-stu-id="208ee-133">Response</span></span>
<span data-ttu-id="208ee-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="208ee-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1616

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windows81SCEPCertificateProfile",
      "id": "2daf8af2-8af2-2daf-f28a-af2df28aaf2d",
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
      ],
      "scepServerUrls": [
        "Scep Server Urls value"
      ],
      "subjectNameFormatString": "Subject Name Format String value",
      "keyUsage": "digitalSignature",
      "keySize": "size2048",
      "hashAlgorithm": "sha2",
      "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value",
      "certificateStore": "machine"
    }
  ]
}
```




