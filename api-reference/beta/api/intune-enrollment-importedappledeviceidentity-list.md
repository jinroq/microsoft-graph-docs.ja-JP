---
title: リスト importedAppleDeviceIdentities
description: ImportedAppleDeviceIdentity オブジェクトのプロパティと関係を一覧表示します。
ms.openlocfilehash: b0b490f6c3de9166bbbd497a819cd3799eef6cff
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27069400"
---
# <a name="list-importedappledeviceidentities"></a><span data-ttu-id="4b3d7-103">リスト importedAppleDeviceIdentities</span><span class="sxs-lookup"><span data-stu-id="4b3d7-103">List importedAppleDeviceIdentities</span></span>

> <span data-ttu-id="4b3d7-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="4b3d7-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4b3d7-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4b3d7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4b3d7-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="4b3d7-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4b3d7-107">[ImportedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)オブジェクトのプロパティと関係を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="4b3d7-107">List properties and relationships of the [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4b3d7-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="4b3d7-108">Prerequisites</span></span>
<span data-ttu-id="4b3d7-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4b3d7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4b3d7-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="4b3d7-111">Permission type</span></span>|<span data-ttu-id="4b3d7-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="4b3d7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4b3d7-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="4b3d7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4b3d7-114">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="4b3d7-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="4b3d7-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="4b3d7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4b3d7-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4b3d7-116">Not supported.</span></span>|
|<span data-ttu-id="4b3d7-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="4b3d7-117">Application</span></span>|<span data-ttu-id="4b3d7-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4b3d7-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4b3d7-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="4b3d7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities
```

## <a name="request-headers"></a><span data-ttu-id="4b3d7-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4b3d7-120">Request headers</span></span>
|<span data-ttu-id="4b3d7-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4b3d7-121">Header</span></span>|<span data-ttu-id="4b3d7-122">値</span><span class="sxs-lookup"><span data-stu-id="4b3d7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4b3d7-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4b3d7-123">Authorization</span></span>|<span data-ttu-id="4b3d7-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="4b3d7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4b3d7-125">Accept</span><span class="sxs-lookup"><span data-stu-id="4b3d7-125">Accept</span></span>|<span data-ttu-id="4b3d7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4b3d7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4b3d7-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="4b3d7-127">Request body</span></span>
<span data-ttu-id="4b3d7-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="4b3d7-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4b3d7-129">応答</span><span class="sxs-lookup"><span data-stu-id="4b3d7-129">Response</span></span>
<span data-ttu-id="4b3d7-130">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)オブジェクトのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="4b3d7-130">If successful, this method returns a `200 OK` response code and a collection of [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4b3d7-131">例</span><span class="sxs-lookup"><span data-stu-id="4b3d7-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="4b3d7-132">要求</span><span class="sxs-lookup"><span data-stu-id="4b3d7-132">Request</span></span>
<span data-ttu-id="4b3d7-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="4b3d7-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities
```

### <a name="response"></a><span data-ttu-id="4b3d7-134">応答</span><span class="sxs-lookup"><span data-stu-id="4b3d7-134">Response</span></span>
<span data-ttu-id="4b3d7-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="4b3d7-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 686

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.importedAppleDeviceIdentity",
      "id": "352e3c2f-3c2f-352e-2f3c-2e352f3c2e35",
      "serialNumber": "Serial Number value",
      "requestedEnrollmentProfileId": "Requested Enrollment Profile Id value",
      "requestedEnrollmentProfileAssignmentDateTime": "2017-01-01T00:02:32.8167841-08:00",
      "isSupervised": true,
      "discoverySource": "adminImport",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastContactedDateTime": "2016-12-31T23:58:44.2908994-08:00",
      "description": "Description value",
      "enrollmentState": "enrolled",
      "platform": "ios"
    }
  ]
}
```





