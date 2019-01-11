---
title: リスト androidForWorkCertificateProfileBases
description: AndroidForWorkCertificateProfileBase オブジェクトのプロパティと関係を一覧表示します。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 6f5ece38b7e4fe066d9fc81b287c149b5bce47ed
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27882398"
---
# <a name="list-androidforworkcertificateprofilebases"></a><span data-ttu-id="3bd9a-103">リスト androidForWorkCertificateProfileBases</span><span class="sxs-lookup"><span data-stu-id="3bd9a-103">List androidForWorkCertificateProfileBases</span></span>

> <span data-ttu-id="3bd9a-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="3bd9a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3bd9a-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3bd9a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3bd9a-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="3bd9a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3bd9a-107">[AndroidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)オブジェクトのプロパティと関係を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="3bd9a-107">List properties and relationships of the [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3bd9a-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="3bd9a-108">Prerequisites</span></span>
<span data-ttu-id="3bd9a-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3bd9a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3bd9a-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="3bd9a-111">Permission type</span></span>|<span data-ttu-id="3bd9a-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="3bd9a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3bd9a-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="3bd9a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3bd9a-114">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="3bd9a-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="3bd9a-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="3bd9a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3bd9a-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3bd9a-116">Not supported.</span></span>|
|<span data-ttu-id="3bd9a-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="3bd9a-117">Application</span></span>|<span data-ttu-id="3bd9a-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3bd9a-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3bd9a-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="3bd9a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="3bd9a-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3bd9a-120">Request headers</span></span>
|<span data-ttu-id="3bd9a-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3bd9a-121">Header</span></span>|<span data-ttu-id="3bd9a-122">値</span><span class="sxs-lookup"><span data-stu-id="3bd9a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3bd9a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3bd9a-123">Authorization</span></span>|<span data-ttu-id="3bd9a-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="3bd9a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3bd9a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="3bd9a-125">Accept</span></span>|<span data-ttu-id="3bd9a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3bd9a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3bd9a-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="3bd9a-127">Request body</span></span>
<span data-ttu-id="3bd9a-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="3bd9a-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3bd9a-129">応答</span><span class="sxs-lookup"><span data-stu-id="3bd9a-129">Response</span></span>
<span data-ttu-id="3bd9a-130">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に[androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)オブジェクトのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="3bd9a-130">If successful, this method returns a `200 OK` response code and a collection of [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3bd9a-131">例</span><span class="sxs-lookup"><span data-stu-id="3bd9a-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="3bd9a-132">要求</span><span class="sxs-lookup"><span data-stu-id="3bd9a-132">Request</span></span>
<span data-ttu-id="3bd9a-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="3bd9a-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="3bd9a-134">応答</span><span class="sxs-lookup"><span data-stu-id="3bd9a-134">Response</span></span>
<span data-ttu-id="3bd9a-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="3bd9a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 922

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.androidForWorkCertificateProfileBase",
      "id": "87f1d53b-d53b-87f1-3bd5-f1873bd5f187",
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
      "subjectNameFormat": "commonNameIncludingEmail",
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
  ]
}
```





