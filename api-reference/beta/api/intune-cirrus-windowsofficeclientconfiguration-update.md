---
title: windowsOfficeClientConfiguration の更新
description: 特定のセキュリティ以外のポリシーペイロードにパッチを適用します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: d116d846b6540ea2b9e2a91f54a5abdfa81e2409
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32483293"
---
# <a name="update-windowsofficeclientconfiguration"></a><span data-ttu-id="fd808-103">windowsOfficeClientConfiguration の更新</span><span class="sxs-lookup"><span data-stu-id="fd808-103">Update windowsOfficeClientConfiguration</span></span>

> <span data-ttu-id="fd808-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fd808-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fd808-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="fd808-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fd808-106">特定のセキュリティ以外のポリシーペイロードにパッチを適用します。</span><span class="sxs-lookup"><span data-stu-id="fd808-106">Patch a specific non-security policy payload.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fd808-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="fd808-107">Prerequisites</span></span>
<span data-ttu-id="fd808-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="fd808-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fd808-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="fd808-110">Permission type</span></span>|<span data-ttu-id="fd808-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="fd808-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fd808-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="fd808-112">Delegated (work or school account)</span></span>|<span data-ttu-id="fd808-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fd808-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="fd808-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="fd808-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fd808-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fd808-115">Not supported.</span></span>|
|<span data-ttu-id="fd808-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="fd808-116">Application</span></span>|<span data-ttu-id="fd808-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fd808-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fd808-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="fd808-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /officeConfiguration/clientConfigurations/{key}
```

## <a name="request-headers"></a><span data-ttu-id="fd808-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="fd808-119">Request headers</span></span>
|<span data-ttu-id="fd808-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="fd808-120">Header</span></span>|<span data-ttu-id="fd808-121">値</span><span class="sxs-lookup"><span data-stu-id="fd808-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fd808-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="fd808-122">Authorization</span></span>|<span data-ttu-id="fd808-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="fd808-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fd808-124">承諾</span><span class="sxs-lookup"><span data-stu-id="fd808-124">Accept</span></span>|<span data-ttu-id="fd808-125">application/json</span><span class="sxs-lookup"><span data-stu-id="fd808-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fd808-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="fd808-126">Request body</span></span>
<span data-ttu-id="fd808-127">要求本文で、 [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="fd808-127">In the request body, supply a JSON representation for the [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md) object.</span></span>

<span data-ttu-id="fd808-128">次の表に、 [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="fd808-128">The following table shows the properties that are required when you create the [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md).</span></span>

|<span data-ttu-id="fd808-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fd808-129">Property</span></span>|<span data-ttu-id="fd808-130">型</span><span class="sxs-lookup"><span data-stu-id="fd808-130">Type</span></span>|<span data-ttu-id="fd808-131">説明</span><span class="sxs-lookup"><span data-stu-id="fd808-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fd808-132">id</span><span class="sxs-lookup"><span data-stu-id="fd808-132">id</span></span>|<span data-ttu-id="fd808-133">String</span><span class="sxs-lookup"><span data-stu-id="fd808-133">String</span></span>|<span data-ttu-id="fd808-134">まだ文書化されていない[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)からの継承</span><span class="sxs-lookup"><span data-stu-id="fd808-134">Not yet documented Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="fd808-135">userPreferencePayload</span><span class="sxs-lookup"><span data-stu-id="fd808-135">userPreferencePayload</span></span>|<span data-ttu-id="fd808-136">Stream</span><span class="sxs-lookup"><span data-stu-id="fd808-136">Stream</span></span>|<span data-ttu-id="fd808-137">まだ文書化されていない[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)からの継承</span><span class="sxs-lookup"><span data-stu-id="fd808-137">Not yet documented Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="fd808-138">policypayload</span><span class="sxs-lookup"><span data-stu-id="fd808-138">policyPayload</span></span>|<span data-ttu-id="fd808-139">Stream</span><span class="sxs-lookup"><span data-stu-id="fd808-139">Stream</span></span>|<span data-ttu-id="fd808-140">まだ文書化されていない[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)からの継承</span><span class="sxs-lookup"><span data-stu-id="fd808-140">Not yet documented Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="fd808-141">説明</span><span class="sxs-lookup"><span data-stu-id="fd808-141">description</span></span>|<span data-ttu-id="fd808-142">String</span><span class="sxs-lookup"><span data-stu-id="fd808-142">String</span></span>|<span data-ttu-id="fd808-143">まだ文書化されていない[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)からの継承</span><span class="sxs-lookup"><span data-stu-id="fd808-143">Not yet documented Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="fd808-144">displayName</span><span class="sxs-lookup"><span data-stu-id="fd808-144">displayName</span></span>|<span data-ttu-id="fd808-145">String</span><span class="sxs-lookup"><span data-stu-id="fd808-145">String</span></span>|<span data-ttu-id="fd808-146">まだ文書化されていない[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)からの継承</span><span class="sxs-lookup"><span data-stu-id="fd808-146">Not yet documented Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="fd808-147">priority</span><span class="sxs-lookup"><span data-stu-id="fd808-147">priority</span></span>|<span data-ttu-id="fd808-148">Int32</span><span class="sxs-lookup"><span data-stu-id="fd808-148">Int32</span></span>|<span data-ttu-id="fd808-149">まだ文書化されていない[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)からの継承</span><span class="sxs-lookup"><span data-stu-id="fd808-149">Not yet documented Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="fd808-150">userCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="fd808-150">userCheckinSummary</span></span>|[<span data-ttu-id="fd808-151">officeUserCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="fd808-151">officeUserCheckinSummary</span></span>](../resources/intune-cirrus-officeusercheckinsummary.md)|<span data-ttu-id="fd808-152">まだ文書化されていない[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)からの継承</span><span class="sxs-lookup"><span data-stu-id="fd808-152">Not yet documented Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="fd808-153">checkinstatuses</span><span class="sxs-lookup"><span data-stu-id="fd808-153">checkinStatuses</span></span>|<span data-ttu-id="fd808-154">[officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="fd808-154">[officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md) collection</span></span>|<span data-ttu-id="fd808-155">まだ文書化されていない[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)からの継承</span><span class="sxs-lookup"><span data-stu-id="fd808-155">Not yet documented Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="fd808-156">応答</span><span class="sxs-lookup"><span data-stu-id="fd808-156">Response</span></span>
<span data-ttu-id="fd808-157">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="fd808-157">If successful, this method returns a `200 OK` response code and an updated [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fd808-158">例</span><span class="sxs-lookup"><span data-stu-id="fd808-158">Example</span></span>

### <a name="request"></a><span data-ttu-id="fd808-159">要求</span><span class="sxs-lookup"><span data-stu-id="fd808-159">Request</span></span>
<span data-ttu-id="fd808-160">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="fd808-160">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/officeConfiguration/clientConfigurations/{officeClientConfigurationId}
Content-type: application/json
Content-length: 949

{
  "userPreferencePayload": "<Unknown Primitive Type Edm.Stream>",
  "policyPayload": "<Unknown Primitive Type Edm.Stream>",
  "description": "Description value",
  "displayName": "Display Name value",
  "priority": 8,
  "userCheckinSummary": {
    "@odata.type": "microsoft.graph.officeUserCheckinSummary",
    "succeededUserCount": 2,
    "failedUserCount": 15
  },
  "checkinStatuses": [
    {
      "@odata.type": "microsoft.graph.officeClientCheckinStatus",
      "userPrincipalName": "User Principal Name value",
      "deviceName": "Device Name value",
      "devicePlatform": "Device Platform value",
      "devicePlatformVersion": "Device Platform Version value",
      "wasSuccessful": true,
      "userId": "User Id value",
      "checkinDateTime": "2016-12-31T23:56:33.9571764-08:00",
      "errorMessage": "Error Message value",
      "appliedPolicies": [
        "Applied Policies value"
      ]
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="fd808-161">応答</span><span class="sxs-lookup"><span data-stu-id="fd808-161">Response</span></span>
<span data-ttu-id="fd808-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="fd808-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1069

{
  "@odata.type": "#microsoft.graph.windowsOfficeClientConfiguration",
  "id": "13a5ac73-ac73-13a5-73ac-a51373aca513",
  "userPreferencePayload": "<Unknown Primitive Type Edm.Stream>",
  "policyPayload": "<Unknown Primitive Type Edm.Stream>",
  "description": "Description value",
  "displayName": "Display Name value",
  "priority": 8,
  "userCheckinSummary": {
    "@odata.type": "microsoft.graph.officeUserCheckinSummary",
    "succeededUserCount": 2,
    "failedUserCount": 15
  },
  "checkinStatuses": [
    {
      "@odata.type": "microsoft.graph.officeClientCheckinStatus",
      "userPrincipalName": "User Principal Name value",
      "deviceName": "Device Name value",
      "devicePlatform": "Device Platform value",
      "devicePlatformVersion": "Device Platform Version value",
      "wasSuccessful": true,
      "userId": "User Id value",
      "checkinDateTime": "2016-12-31T23:56:33.9571764-08:00",
      "errorMessage": "Error Message value",
      "appliedPolicies": [
        "Applied Policies value"
      ]
    }
  ]
}
```



