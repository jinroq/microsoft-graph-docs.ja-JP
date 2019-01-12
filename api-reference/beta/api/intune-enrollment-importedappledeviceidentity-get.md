---
title: ImportedAppleDeviceIdentity を取得します。
description: ImportedAppleDeviceIdentity オブジェクトのプロパティと関係を参照してください。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 084bfcf690296cc0f9328fd06d8be0f40f14402b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27913024"
---
# <a name="get-importedappledeviceidentity"></a><span data-ttu-id="821b6-103">ImportedAppleDeviceIdentity を取得します。</span><span class="sxs-lookup"><span data-stu-id="821b6-103">Get importedAppleDeviceIdentity</span></span>

> <span data-ttu-id="821b6-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="821b6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="821b6-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="821b6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="821b6-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="821b6-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="821b6-107">[ImportedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="821b6-107">Read properties and relationships of the [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="821b6-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="821b6-108">Prerequisites</span></span>
<span data-ttu-id="821b6-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="821b6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="821b6-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="821b6-111">Permission type</span></span>|<span data-ttu-id="821b6-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="821b6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="821b6-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="821b6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="821b6-114">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="821b6-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="821b6-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="821b6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="821b6-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="821b6-116">Not supported.</span></span>|
|<span data-ttu-id="821b6-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="821b6-117">Application</span></span>|<span data-ttu-id="821b6-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="821b6-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="821b6-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="821b6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities/{importedAppleDeviceIdentityId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="821b6-120">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="821b6-120">Optional query parameters</span></span>
<span data-ttu-id="821b6-121">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="821b6-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="821b6-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="821b6-122">Request headers</span></span>
|<span data-ttu-id="821b6-123">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="821b6-123">Header</span></span>|<span data-ttu-id="821b6-124">値</span><span class="sxs-lookup"><span data-stu-id="821b6-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="821b6-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="821b6-125">Authorization</span></span>|<span data-ttu-id="821b6-126">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="821b6-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="821b6-127">Accept</span><span class="sxs-lookup"><span data-stu-id="821b6-127">Accept</span></span>|<span data-ttu-id="821b6-128">application/json</span><span class="sxs-lookup"><span data-stu-id="821b6-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="821b6-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="821b6-129">Request body</span></span>
<span data-ttu-id="821b6-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="821b6-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="821b6-131">応答</span><span class="sxs-lookup"><span data-stu-id="821b6-131">Response</span></span>
<span data-ttu-id="821b6-132">かどうかは成功すると、このメソッドが返されます、 `200 OK` 、応答の本体で応答コードと[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)のオブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="821b6-132">If successful, this method returns a `200 OK` response code and [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="821b6-133">例</span><span class="sxs-lookup"><span data-stu-id="821b6-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="821b6-134">要求</span><span class="sxs-lookup"><span data-stu-id="821b6-134">Request</span></span>
<span data-ttu-id="821b6-135">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="821b6-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities/{importedAppleDeviceIdentityId}
```

### <a name="response"></a><span data-ttu-id="821b6-136">応答</span><span class="sxs-lookup"><span data-stu-id="821b6-136">Response</span></span>
<span data-ttu-id="821b6-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="821b6-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 648

{
  "value": {
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
}
```





