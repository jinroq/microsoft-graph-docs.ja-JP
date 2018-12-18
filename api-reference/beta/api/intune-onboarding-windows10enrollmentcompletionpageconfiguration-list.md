---
title: リスト windows10EnrollmentCompletionPageConfigurations
description: Windows10EnrollmentCompletionPageConfiguration オブジェクトのプロパティと関係を一覧表示します。
author: tfitzmac
ms.openlocfilehash: 0a58303efbf97e8f447d0fdd0345d46d559b3c77
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27338725"
---
# <a name="list-windows10enrollmentcompletionpageconfigurations"></a><span data-ttu-id="5507b-103">リスト windows10EnrollmentCompletionPageConfigurations</span><span class="sxs-lookup"><span data-stu-id="5507b-103">List windows10EnrollmentCompletionPageConfigurations</span></span>

> <span data-ttu-id="5507b-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="5507b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5507b-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5507b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5507b-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="5507b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5507b-107">[Windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md)オブジェクトのプロパティと関係を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="5507b-107">List properties and relationships of the [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="5507b-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="5507b-108">Prerequisites</span></span>
<span data-ttu-id="5507b-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5507b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5507b-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="5507b-111">Permission type</span></span>|<span data-ttu-id="5507b-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="5507b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5507b-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="5507b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5507b-114">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="5507b-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="5507b-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="5507b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5507b-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5507b-116">Not supported.</span></span>|
|<span data-ttu-id="5507b-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="5507b-117">Application</span></span>|<span data-ttu-id="5507b-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5507b-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5507b-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="5507b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="5507b-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5507b-120">Request headers</span></span>
|<span data-ttu-id="5507b-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5507b-121">Header</span></span>|<span data-ttu-id="5507b-122">値</span><span class="sxs-lookup"><span data-stu-id="5507b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5507b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5507b-123">Authorization</span></span>|<span data-ttu-id="5507b-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="5507b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5507b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="5507b-125">Accept</span></span>|<span data-ttu-id="5507b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5507b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5507b-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="5507b-127">Request body</span></span>
<span data-ttu-id="5507b-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="5507b-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5507b-129">応答</span><span class="sxs-lookup"><span data-stu-id="5507b-129">Response</span></span>
<span data-ttu-id="5507b-130">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に[windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md)オブジェクトのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="5507b-130">If successful, this method returns a `200 OK` response code and a collection of [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5507b-131">例</span><span class="sxs-lookup"><span data-stu-id="5507b-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="5507b-132">要求</span><span class="sxs-lookup"><span data-stu-id="5507b-132">Request</span></span>
<span data-ttu-id="5507b-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="5507b-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations
```

### <a name="response"></a><span data-ttu-id="5507b-134">応答</span><span class="sxs-lookup"><span data-stu-id="5507b-134">Response</span></span>
<span data-ttu-id="5507b-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="5507b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 860

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windows10EnrollmentCompletionPageConfiguration",
      "id": "77bf8248-8248-77bf-4882-bf774882bf77",
      "displayName": "Display Name value",
      "description": "Description value",
      "priority": 8,
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "version": 7,
      "showInstallationProgress": true,
      "blockDeviceSetupRetryByUser": true,
      "allowDeviceResetOnInstallFailure": true,
      "allowLogCollectionOnInstallFailure": true,
      "customErrorMessage": "Custom Error Message value",
      "installProgressTimeoutInMinutes": 15,
      "allowDeviceUseOnInstallFailure": true,
      "selectedMobileAppIds": [
        "Selected Mobile App Ids value"
      ]
    }
  ]
}
```





