---
title: importAppleDeviceIdentityList アクション
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 717824e8d0731fe50cb00537e8c8d73647de3778
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31790236"
---
# <a name="importappledeviceidentitylist-action"></a><span data-ttu-id="1a291-103">importAppleDeviceIdentityList アクション</span><span class="sxs-lookup"><span data-stu-id="1a291-103">importAppleDeviceIdentityList action</span></span>

> <span data-ttu-id="1a291-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1a291-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1a291-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="1a291-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1a291-106">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="1a291-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1a291-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="1a291-107">Prerequisites</span></span>
<span data-ttu-id="1a291-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1a291-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1a291-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1a291-110">Permission type</span></span>|<span data-ttu-id="1a291-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="1a291-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1a291-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="1a291-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1a291-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1a291-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="1a291-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1a291-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1a291-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1a291-115">Not supported.</span></span>|
|<span data-ttu-id="1a291-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1a291-116">Application</span></span>|<span data-ttu-id="1a291-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1a291-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1a291-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1a291-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities/importAppleDeviceIdentityList
```

## <a name="request-headers"></a><span data-ttu-id="1a291-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1a291-119">Request headers</span></span>
|<span data-ttu-id="1a291-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1a291-120">Header</span></span>|<span data-ttu-id="1a291-121">値</span><span class="sxs-lookup"><span data-stu-id="1a291-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1a291-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="1a291-122">Authorization</span></span>|<span data-ttu-id="1a291-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="1a291-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1a291-124">承諾</span><span class="sxs-lookup"><span data-stu-id="1a291-124">Accept</span></span>|<span data-ttu-id="1a291-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1a291-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1a291-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="1a291-126">Request body</span></span>
<span data-ttu-id="1a291-127">要求本文で、パラメーターの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="1a291-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="1a291-128">次の表に、このアクションで使用できるパラメーターを示します。</span><span class="sxs-lookup"><span data-stu-id="1a291-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="1a291-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1a291-129">Property</span></span>|<span data-ttu-id="1a291-130">型</span><span class="sxs-lookup"><span data-stu-id="1a291-130">Type</span></span>|<span data-ttu-id="1a291-131">説明</span><span class="sxs-lookup"><span data-stu-id="1a291-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1a291-132">importedAppleDeviceIdentities</span><span class="sxs-lookup"><span data-stu-id="1a291-132">importedAppleDeviceIdentities</span></span>|<span data-ttu-id="1a291-133">[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="1a291-133">[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) collection</span></span>|<span data-ttu-id="1a291-134">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="1a291-134">Not yet documented</span></span>|
|<span data-ttu-id="1a291-135">overwriteImportedDeviceIdentities</span><span class="sxs-lookup"><span data-stu-id="1a291-135">overwriteImportedDeviceIdentities</span></span>|<span data-ttu-id="1a291-136">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="1a291-136">Boolean</span></span>|<span data-ttu-id="1a291-137">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="1a291-137">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="1a291-138">応答</span><span class="sxs-lookup"><span data-stu-id="1a291-138">Response</span></span>
<span data-ttu-id="1a291-139">成功した場合、このアクション`200 OK`は応答コードと、応答本文で[importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md)コレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="1a291-139">If successful, this action returns a `200 OK` response code and a [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1a291-140">例</span><span class="sxs-lookup"><span data-stu-id="1a291-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="1a291-141">要求</span><span class="sxs-lookup"><span data-stu-id="1a291-141">Request</span></span>
<span data-ttu-id="1a291-142">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="1a291-142">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="1a291-143">応答</span><span class="sxs-lookup"><span data-stu-id="1a291-143">Response</span></span>
<span data-ttu-id="1a291-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="1a291-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





