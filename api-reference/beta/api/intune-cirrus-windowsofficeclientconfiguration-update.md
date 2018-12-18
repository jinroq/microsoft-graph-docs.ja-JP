---
title: WindowsOfficeClientConfiguration を更新します。
description: セキュリティ以外の特定のポリシーのペイロードにパッチを適用します。
author: tfitzmac
ms.openlocfilehash: 728fe7b6ffdb4b964488317551fdbaef139d2803
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27310753"
---
# <a name="update-windowsofficeclientconfiguration"></a><span data-ttu-id="51300-103">WindowsOfficeClientConfiguration を更新します。</span><span class="sxs-lookup"><span data-stu-id="51300-103">Update windowsOfficeClientConfiguration</span></span>

> <span data-ttu-id="51300-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="51300-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="51300-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="51300-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="51300-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="51300-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="51300-107">セキュリティ以外の特定のポリシーのペイロードにパッチを適用します。</span><span class="sxs-lookup"><span data-stu-id="51300-107">Patch a specific non-security policy payload.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="51300-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="51300-108">Prerequisites</span></span>
<span data-ttu-id="51300-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="51300-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="51300-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="51300-111">Permission type</span></span>|<span data-ttu-id="51300-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="51300-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="51300-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="51300-113">Delegated (work or school account)</span></span>|<span data-ttu-id="51300-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="51300-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="51300-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="51300-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="51300-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="51300-116">Not supported.</span></span>|
|<span data-ttu-id="51300-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="51300-117">Application</span></span>|<span data-ttu-id="51300-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="51300-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="51300-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="51300-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /officeConfiguration/clientConfigurations/{key}
```

## <a name="request-headers"></a><span data-ttu-id="51300-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="51300-120">Request headers</span></span>
|<span data-ttu-id="51300-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="51300-121">Header</span></span>|<span data-ttu-id="51300-122">値</span><span class="sxs-lookup"><span data-stu-id="51300-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="51300-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="51300-123">Authorization</span></span>|<span data-ttu-id="51300-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="51300-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="51300-125">Accept</span><span class="sxs-lookup"><span data-stu-id="51300-125">Accept</span></span>|<span data-ttu-id="51300-126">application/json</span><span class="sxs-lookup"><span data-stu-id="51300-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="51300-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="51300-127">Request body</span></span>
<span data-ttu-id="51300-128">要求の本文に[windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md)オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="51300-128">In the request body, supply a JSON representation for the [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md) object.</span></span>

<span data-ttu-id="51300-129">[WindowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md)を作成するときに必要なプロパティを次の表に示します。</span><span class="sxs-lookup"><span data-stu-id="51300-129">The following table shows the properties that are required when you create the [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md).</span></span>

|<span data-ttu-id="51300-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="51300-130">Property</span></span>|<span data-ttu-id="51300-131">種類</span><span class="sxs-lookup"><span data-stu-id="51300-131">Type</span></span>|<span data-ttu-id="51300-132">説明</span><span class="sxs-lookup"><span data-stu-id="51300-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="51300-133">ID</span><span class="sxs-lookup"><span data-stu-id="51300-133">id</span></span>|<span data-ttu-id="51300-134">String</span><span class="sxs-lookup"><span data-stu-id="51300-134">String</span></span>|<span data-ttu-id="51300-135">[OfficeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)から継承を文書化されていません。</span><span class="sxs-lookup"><span data-stu-id="51300-135">Not yet documented Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="51300-136">userPreferencePayload</span><span class="sxs-lookup"><span data-stu-id="51300-136">userPreferencePayload</span></span>|<span data-ttu-id="51300-137">Stream</span><span class="sxs-lookup"><span data-stu-id="51300-137">Stream</span></span>|<span data-ttu-id="51300-138">[OfficeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)から継承を文書化されていません。</span><span class="sxs-lookup"><span data-stu-id="51300-138">Not yet documented Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="51300-139">policyPayload</span><span class="sxs-lookup"><span data-stu-id="51300-139">policyPayload</span></span>|<span data-ttu-id="51300-140">Stream</span><span class="sxs-lookup"><span data-stu-id="51300-140">Stream</span></span>|<span data-ttu-id="51300-141">[OfficeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)から継承を文書化されていません。</span><span class="sxs-lookup"><span data-stu-id="51300-141">Not yet documented Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="51300-142">説明</span><span class="sxs-lookup"><span data-stu-id="51300-142">description</span></span>|<span data-ttu-id="51300-143">String</span><span class="sxs-lookup"><span data-stu-id="51300-143">String</span></span>|<span data-ttu-id="51300-144">[OfficeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)から継承を文書化されていません。</span><span class="sxs-lookup"><span data-stu-id="51300-144">Not yet documented Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="51300-145">displayName</span><span class="sxs-lookup"><span data-stu-id="51300-145">displayName</span></span>|<span data-ttu-id="51300-146">String</span><span class="sxs-lookup"><span data-stu-id="51300-146">String</span></span>|<span data-ttu-id="51300-147">[OfficeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)から継承を文書化されていません。</span><span class="sxs-lookup"><span data-stu-id="51300-147">Not yet documented Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="51300-148">priority</span><span class="sxs-lookup"><span data-stu-id="51300-148">priority</span></span>|<span data-ttu-id="51300-149">Int32</span><span class="sxs-lookup"><span data-stu-id="51300-149">Int32</span></span>|<span data-ttu-id="51300-150">[OfficeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)から継承を文書化されていません。</span><span class="sxs-lookup"><span data-stu-id="51300-150">Not yet documented Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="51300-151">userCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="51300-151">userCheckinSummary</span></span>|[<span data-ttu-id="51300-152">officeUserCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="51300-152">officeUserCheckinSummary</span></span>](../resources/intune-cirrus-officeusercheckinsummary.md)|<span data-ttu-id="51300-153">[OfficeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)から継承を文書化されていません。</span><span class="sxs-lookup"><span data-stu-id="51300-153">Not yet documented Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="51300-154">checkinStatuses</span><span class="sxs-lookup"><span data-stu-id="51300-154">checkinStatuses</span></span>|<span data-ttu-id="51300-155">[officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="51300-155">[officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md) collection</span></span>|<span data-ttu-id="51300-156">[OfficeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)から継承を文書化されていません。</span><span class="sxs-lookup"><span data-stu-id="51300-156">Not yet documented Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="51300-157">応答</span><span class="sxs-lookup"><span data-stu-id="51300-157">Response</span></span>
<span data-ttu-id="51300-158">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に更新された[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="51300-158">If successful, this method returns a `200 OK` response code and an updated [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="51300-159">例</span><span class="sxs-lookup"><span data-stu-id="51300-159">Example</span></span>
### <a name="request"></a><span data-ttu-id="51300-160">要求</span><span class="sxs-lookup"><span data-stu-id="51300-160">Request</span></span>
<span data-ttu-id="51300-161">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="51300-161">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="51300-162">応答</span><span class="sxs-lookup"><span data-stu-id="51300-162">Response</span></span>
<span data-ttu-id="51300-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="51300-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



