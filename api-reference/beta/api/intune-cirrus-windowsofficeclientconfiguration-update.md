---
title: WindowsOfficeClientConfiguration を更新します。
description: セキュリティ以外の特定のポリシーのペイロードにパッチを適用します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: cb9078e630ab20c38bcf9cb41a08d6e94f370311
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29401363"
---
# <a name="update-windowsofficeclientconfiguration"></a><span data-ttu-id="47717-103">WindowsOfficeClientConfiguration を更新します。</span><span class="sxs-lookup"><span data-stu-id="47717-103">Update windowsOfficeClientConfiguration</span></span>

> <span data-ttu-id="47717-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="47717-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="47717-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="47717-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="47717-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="47717-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="47717-107">セキュリティ以外の特定のポリシーのペイロードにパッチを適用します。</span><span class="sxs-lookup"><span data-stu-id="47717-107">Patch a specific non-security policy payload.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="47717-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="47717-108">Prerequisites</span></span>
<span data-ttu-id="47717-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="47717-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="47717-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="47717-111">Permission type</span></span>|<span data-ttu-id="47717-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="47717-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="47717-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="47717-113">Delegated (work or school account)</span></span>|<span data-ttu-id="47717-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="47717-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="47717-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="47717-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="47717-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="47717-116">Not supported.</span></span>|
|<span data-ttu-id="47717-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="47717-117">Application</span></span>|<span data-ttu-id="47717-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="47717-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="47717-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="47717-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /officeConfiguration/clientConfigurations/{key}
```

## <a name="request-headers"></a><span data-ttu-id="47717-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="47717-120">Request headers</span></span>
|<span data-ttu-id="47717-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="47717-121">Header</span></span>|<span data-ttu-id="47717-122">値</span><span class="sxs-lookup"><span data-stu-id="47717-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="47717-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="47717-123">Authorization</span></span>|<span data-ttu-id="47717-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="47717-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="47717-125">Accept</span><span class="sxs-lookup"><span data-stu-id="47717-125">Accept</span></span>|<span data-ttu-id="47717-126">application/json</span><span class="sxs-lookup"><span data-stu-id="47717-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="47717-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="47717-127">Request body</span></span>
<span data-ttu-id="47717-128">要求の本文に[windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md)オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="47717-128">In the request body, supply a JSON representation for the [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md) object.</span></span>

<span data-ttu-id="47717-129">[WindowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md)を作成するときに必要なプロパティを次の表に示します。</span><span class="sxs-lookup"><span data-stu-id="47717-129">The following table shows the properties that are required when you create the [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md).</span></span>

|<span data-ttu-id="47717-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="47717-130">Property</span></span>|<span data-ttu-id="47717-131">型</span><span class="sxs-lookup"><span data-stu-id="47717-131">Type</span></span>|<span data-ttu-id="47717-132">説明</span><span class="sxs-lookup"><span data-stu-id="47717-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="47717-133">id</span><span class="sxs-lookup"><span data-stu-id="47717-133">id</span></span>|<span data-ttu-id="47717-134">String</span><span class="sxs-lookup"><span data-stu-id="47717-134">String</span></span>|<span data-ttu-id="47717-135">[OfficeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)から継承を文書化されていません。</span><span class="sxs-lookup"><span data-stu-id="47717-135">Not yet documented Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="47717-136">userPreferencePayload</span><span class="sxs-lookup"><span data-stu-id="47717-136">userPreferencePayload</span></span>|<span data-ttu-id="47717-137">Stream</span><span class="sxs-lookup"><span data-stu-id="47717-137">Stream</span></span>|<span data-ttu-id="47717-138">[OfficeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)から継承を文書化されていません。</span><span class="sxs-lookup"><span data-stu-id="47717-138">Not yet documented Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="47717-139">policyPayload</span><span class="sxs-lookup"><span data-stu-id="47717-139">policyPayload</span></span>|<span data-ttu-id="47717-140">Stream</span><span class="sxs-lookup"><span data-stu-id="47717-140">Stream</span></span>|<span data-ttu-id="47717-141">[OfficeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)から継承を文書化されていません。</span><span class="sxs-lookup"><span data-stu-id="47717-141">Not yet documented Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="47717-142">説明</span><span class="sxs-lookup"><span data-stu-id="47717-142">description</span></span>|<span data-ttu-id="47717-143">String</span><span class="sxs-lookup"><span data-stu-id="47717-143">String</span></span>|<span data-ttu-id="47717-144">[OfficeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)から継承を文書化されていません。</span><span class="sxs-lookup"><span data-stu-id="47717-144">Not yet documented Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="47717-145">displayName</span><span class="sxs-lookup"><span data-stu-id="47717-145">displayName</span></span>|<span data-ttu-id="47717-146">String</span><span class="sxs-lookup"><span data-stu-id="47717-146">String</span></span>|<span data-ttu-id="47717-147">[OfficeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)から継承を文書化されていません。</span><span class="sxs-lookup"><span data-stu-id="47717-147">Not yet documented Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="47717-148">priority</span><span class="sxs-lookup"><span data-stu-id="47717-148">priority</span></span>|<span data-ttu-id="47717-149">Int32</span><span class="sxs-lookup"><span data-stu-id="47717-149">Int32</span></span>|<span data-ttu-id="47717-150">[OfficeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)から継承を文書化されていません。</span><span class="sxs-lookup"><span data-stu-id="47717-150">Not yet documented Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="47717-151">userCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="47717-151">userCheckinSummary</span></span>|[<span data-ttu-id="47717-152">officeUserCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="47717-152">officeUserCheckinSummary</span></span>](../resources/intune-cirrus-officeusercheckinsummary.md)|<span data-ttu-id="47717-153">[OfficeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)から継承を文書化されていません。</span><span class="sxs-lookup"><span data-stu-id="47717-153">Not yet documented Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="47717-154">checkinStatuses</span><span class="sxs-lookup"><span data-stu-id="47717-154">checkinStatuses</span></span>|<span data-ttu-id="47717-155">[officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="47717-155">[officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md) collection</span></span>|<span data-ttu-id="47717-156">[OfficeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)から継承を文書化されていません。</span><span class="sxs-lookup"><span data-stu-id="47717-156">Not yet documented Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="47717-157">応答</span><span class="sxs-lookup"><span data-stu-id="47717-157">Response</span></span>
<span data-ttu-id="47717-158">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に更新された[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="47717-158">If successful, this method returns a `200 OK` response code and an updated [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="47717-159">例</span><span class="sxs-lookup"><span data-stu-id="47717-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="47717-160">要求</span><span class="sxs-lookup"><span data-stu-id="47717-160">Request</span></span>
<span data-ttu-id="47717-161">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="47717-161">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="47717-162">応答</span><span class="sxs-lookup"><span data-stu-id="47717-162">Response</span></span>
<span data-ttu-id="47717-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="47717-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



