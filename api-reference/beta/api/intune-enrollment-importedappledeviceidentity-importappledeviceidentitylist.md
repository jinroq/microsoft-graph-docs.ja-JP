---
title: importAppleDeviceIdentityList アクション
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 75a40be8d2ea3ddafadb78f95662dcadf7a9ac01
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27890602"
---
# <a name="importappledeviceidentitylist-action"></a><span data-ttu-id="75b3b-103">importAppleDeviceIdentityList アクション</span><span class="sxs-lookup"><span data-stu-id="75b3b-103">importAppleDeviceIdentityList action</span></span>

> <span data-ttu-id="75b3b-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="75b3b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="75b3b-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="75b3b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="75b3b-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="75b3b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="75b3b-107">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="75b3b-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="75b3b-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="75b3b-108">Prerequisites</span></span>
<span data-ttu-id="75b3b-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="75b3b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="75b3b-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="75b3b-111">Permission type</span></span>|<span data-ttu-id="75b3b-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="75b3b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="75b3b-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="75b3b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="75b3b-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="75b3b-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="75b3b-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="75b3b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="75b3b-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="75b3b-116">Not supported.</span></span>|
|<span data-ttu-id="75b3b-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="75b3b-117">Application</span></span>|<span data-ttu-id="75b3b-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="75b3b-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="75b3b-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="75b3b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities/importAppleDeviceIdentityList
```

## <a name="request-headers"></a><span data-ttu-id="75b3b-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="75b3b-120">Request headers</span></span>
|<span data-ttu-id="75b3b-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="75b3b-121">Header</span></span>|<span data-ttu-id="75b3b-122">値</span><span class="sxs-lookup"><span data-stu-id="75b3b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="75b3b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="75b3b-123">Authorization</span></span>|<span data-ttu-id="75b3b-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="75b3b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="75b3b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="75b3b-125">Accept</span></span>|<span data-ttu-id="75b3b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="75b3b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="75b3b-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="75b3b-127">Request body</span></span>
<span data-ttu-id="75b3b-128">要求本文で、パラメーターの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="75b3b-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="75b3b-129">次の表に、このアクションで使用できるパラメーターを示します。</span><span class="sxs-lookup"><span data-stu-id="75b3b-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="75b3b-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="75b3b-130">Property</span></span>|<span data-ttu-id="75b3b-131">種類</span><span class="sxs-lookup"><span data-stu-id="75b3b-131">Type</span></span>|<span data-ttu-id="75b3b-132">説明</span><span class="sxs-lookup"><span data-stu-id="75b3b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="75b3b-133">importedAppleDeviceIdentities</span><span class="sxs-lookup"><span data-stu-id="75b3b-133">importedAppleDeviceIdentities</span></span>|<span data-ttu-id="75b3b-134">[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="75b3b-134">[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) collection</span></span>|<span data-ttu-id="75b3b-135">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="75b3b-135">Not yet documented</span></span>|
|<span data-ttu-id="75b3b-136">overwriteImportedDeviceIdentities</span><span class="sxs-lookup"><span data-stu-id="75b3b-136">overwriteImportedDeviceIdentities</span></span>|<span data-ttu-id="75b3b-137">ブール値</span><span class="sxs-lookup"><span data-stu-id="75b3b-137">Boolean</span></span>|<span data-ttu-id="75b3b-138">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="75b3b-138">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="75b3b-139">応答</span><span class="sxs-lookup"><span data-stu-id="75b3b-139">Response</span></span>
<span data-ttu-id="75b3b-140">かどうか、成功を返すアクション、`200 OK`応答コードおよび応答の本文に[importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md)のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="75b3b-140">If successful, this action returns a `200 OK` response code and a [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="75b3b-141">例</span><span class="sxs-lookup"><span data-stu-id="75b3b-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="75b3b-142">要求</span><span class="sxs-lookup"><span data-stu-id="75b3b-142">Request</span></span>
<span data-ttu-id="75b3b-143">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="75b3b-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities/importAppleDeviceIdentityList

Content-type: application/json
Content-length: 756

{
  "importedAppleDeviceIdentities": [
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
  ],
  "overwriteImportedDeviceIdentities": true
}
```

### <a name="response"></a><span data-ttu-id="75b3b-144">応答</span><span class="sxs-lookup"><span data-stu-id="75b3b-144">Response</span></span>
<span data-ttu-id="75b3b-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="75b3b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 715

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.importedAppleDeviceIdentityResult",
      "id": "557cfb4a-fb4a-557c-4afb-7c554afb7c55",
      "serialNumber": "Serial Number value",
      "requestedEnrollmentProfileId": "Requested Enrollment Profile Id value",
      "requestedEnrollmentProfileAssignmentDateTime": "2017-01-01T00:02:32.8167841-08:00",
      "isSupervised": true,
      "discoverySource": "adminImport",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastContactedDateTime": "2016-12-31T23:58:44.2908994-08:00",
      "description": "Description value",
      "enrollmentState": "enrolled",
      "platform": "ios",
      "status": true
    }
  ]
}
```





