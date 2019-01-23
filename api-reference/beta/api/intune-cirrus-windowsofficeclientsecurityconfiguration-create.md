---
title: WindowsOfficeClientSecurityConfiguration を作成します。
description: 新しい windowsOfficeClientSecurityConfiguration オブジェクトを作成します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: fedc5897f5cc3422de3eb83c8e5d94dcfc56f117
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29417323"
---
# <a name="create-windowsofficeclientsecurityconfiguration"></a><span data-ttu-id="d0160-103">WindowsOfficeClientSecurityConfiguration を作成します。</span><span class="sxs-lookup"><span data-stu-id="d0160-103">Create windowsOfficeClientSecurityConfiguration</span></span>

> <span data-ttu-id="d0160-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="d0160-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="d0160-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d0160-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d0160-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="d0160-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d0160-107">新しい[windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="d0160-107">Create a new [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d0160-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="d0160-108">Prerequisites</span></span>
<span data-ttu-id="d0160-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d0160-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d0160-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d0160-111">Permission type</span></span>|<span data-ttu-id="d0160-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="d0160-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d0160-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d0160-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d0160-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d0160-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d0160-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d0160-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d0160-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d0160-116">Not supported.</span></span>|
|<span data-ttu-id="d0160-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d0160-117">Application</span></span>|<span data-ttu-id="d0160-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d0160-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d0160-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d0160-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /officeConfiguration/clientConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="d0160-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d0160-120">Request headers</span></span>
|<span data-ttu-id="d0160-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d0160-121">Header</span></span>|<span data-ttu-id="d0160-122">値</span><span class="sxs-lookup"><span data-stu-id="d0160-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d0160-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d0160-123">Authorization</span></span>|<span data-ttu-id="d0160-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="d0160-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d0160-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d0160-125">Accept</span></span>|<span data-ttu-id="d0160-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d0160-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d0160-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="d0160-127">Request body</span></span>
<span data-ttu-id="d0160-128">要求の本文に[windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md)オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="d0160-128">In the request body, supply a JSON representation for the [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) object.</span></span>

<span data-ttu-id="d0160-129">[WindowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md)を作成するときに必要なプロパティを次の表に示します。</span><span class="sxs-lookup"><span data-stu-id="d0160-129">The following table shows the properties that are required when you create the [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md).</span></span>

|<span data-ttu-id="d0160-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d0160-130">Property</span></span>|<span data-ttu-id="d0160-131">型</span><span class="sxs-lookup"><span data-stu-id="d0160-131">Type</span></span>|<span data-ttu-id="d0160-132">説明</span><span class="sxs-lookup"><span data-stu-id="d0160-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d0160-133">id</span><span class="sxs-lookup"><span data-stu-id="d0160-133">id</span></span>|<span data-ttu-id="d0160-134">String</span><span class="sxs-lookup"><span data-stu-id="d0160-134">String</span></span>|<span data-ttu-id="d0160-135">Office クライアントの構成のポリシーの id。</span><span class="sxs-lookup"><span data-stu-id="d0160-135">Id of the office client configuration policy.</span></span> <span data-ttu-id="d0160-136">[OfficeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="d0160-136">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="d0160-137">userPreferencePayload</span><span class="sxs-lookup"><span data-stu-id="d0160-137">userPreferencePayload</span></span>|<span data-ttu-id="d0160-138">Stream</span><span class="sxs-lookup"><span data-stu-id="d0160-138">Stream</span></span>|<span data-ttu-id="d0160-139">JSON の環境設定は、バイナリ形式の文字列は、ユーザーがこれらの値をオーバーライドすることができます。</span><span class="sxs-lookup"><span data-stu-id="d0160-139">Preference settings JSON string in binary format, these values can be overridden by the user.</span></span> <span data-ttu-id="d0160-140">[OfficeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="d0160-140">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="d0160-141">policyPayload</span><span class="sxs-lookup"><span data-stu-id="d0160-141">policyPayload</span></span>|<span data-ttu-id="d0160-142">Stream</span><span class="sxs-lookup"><span data-stu-id="d0160-142">Stream</span></span>|<span data-ttu-id="d0160-143">JSON のポリシー設定はバイナリ形式の文字列は、ユーザーがこれらの値を変更することはできません。</span><span class="sxs-lookup"><span data-stu-id="d0160-143">Policy settings JSON string in binary format, these values cannot be changed by the user.</span></span> <span data-ttu-id="d0160-144">[OfficeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="d0160-144">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="d0160-145">説明</span><span class="sxs-lookup"><span data-stu-id="d0160-145">description</span></span>|<span data-ttu-id="d0160-146">String</span><span class="sxs-lookup"><span data-stu-id="d0160-146">String</span></span>|<span data-ttu-id="d0160-147">管理者には、office クライアントの説明の構成のポリシーが用意されています。</span><span class="sxs-lookup"><span data-stu-id="d0160-147">Admin provided description of the office client configuration policy.</span></span> <span data-ttu-id="d0160-148">[OfficeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="d0160-148">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="d0160-149">displayName</span><span class="sxs-lookup"><span data-stu-id="d0160-149">displayName</span></span>|<span data-ttu-id="d0160-150">String</span><span class="sxs-lookup"><span data-stu-id="d0160-150">String</span></span>|<span data-ttu-id="d0160-151">管理者は、office クライアントの構成のポリシーの名前を提供します。</span><span class="sxs-lookup"><span data-stu-id="d0160-151">Admin provided name of the office client configuration policy.</span></span> <span data-ttu-id="d0160-152">[OfficeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="d0160-152">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="d0160-153">assignments</span><span class="sxs-lookup"><span data-stu-id="d0160-153">assignments</span></span>|<span data-ttu-id="d0160-154">[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="d0160-154">[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) collection</span></span>|<span data-ttu-id="d0160-155">一連のポリシーの割り当てをグループ化.</span><span class="sxs-lookup"><span data-stu-id="d0160-155">The list of group assignments for the policy..</span></span> <span data-ttu-id="d0160-156">[OfficeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="d0160-156">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="d0160-157">priority</span><span class="sxs-lookup"><span data-stu-id="d0160-157">priority</span></span>|<span data-ttu-id="d0160-158">Int32</span><span class="sxs-lookup"><span data-stu-id="d0160-158">Int32</span></span>|<span data-ttu-id="d0160-159">優先度の値がテナントの下にある各ポリシーの一意の値にする必要があり、競合の解決に使用する、値が低い優先順位が高いことを意味します。</span><span class="sxs-lookup"><span data-stu-id="d0160-159">Priority value should be unique value for each policy under a tenant and will be used for conflict resolution, lower values mean priority is high.</span></span> <span data-ttu-id="d0160-160">[OfficeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="d0160-160">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="d0160-161">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d0160-161">lastModifiedDateTime</span></span>|<span data-ttu-id="d0160-162">DateTime
</span><span class="sxs-lookup"><span data-stu-id="d0160-162">DateTime</span></span>|<span data-ttu-id="d0160-163">ポリシーの最終変更された日付時刻スタンプ。</span><span class="sxs-lookup"><span data-stu-id="d0160-163">Last modified datetime stamp of the policy.</span></span> <span data-ttu-id="d0160-164">[OfficeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="d0160-164">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="d0160-165">userCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="d0160-165">userCheckinSummary</span></span>|[<span data-ttu-id="d0160-166">officeUserCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="d0160-166">officeUserCheckinSummary</span></span>](../resources/intune-cirrus-officeusercheckinsummary.md)|<span data-ttu-id="d0160-167">ポリシーの概要チェックのユーザーです。</span><span class="sxs-lookup"><span data-stu-id="d0160-167">User check-in summary for the policy.</span></span> <span data-ttu-id="d0160-168">[OfficeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="d0160-168">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="d0160-169">checkinStatuses</span><span class="sxs-lookup"><span data-stu-id="d0160-169">checkinStatuses</span></span>|<span data-ttu-id="d0160-170">[officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="d0160-170">[officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md) collection</span></span>|<span data-ttu-id="d0160-171">Office クライアントでは、チェック状態の一覧です。</span><span class="sxs-lookup"><span data-stu-id="d0160-171">List of office Client check-in status.</span></span> <span data-ttu-id="d0160-172">[OfficeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="d0160-172">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|




## <a name="response"></a><span data-ttu-id="d0160-173">応答</span><span class="sxs-lookup"><span data-stu-id="d0160-173">Response</span></span>
<span data-ttu-id="d0160-174">かどうかは成功すると、このメソッドが返されます、`201 Created`応答コードおよび応答の本文に[windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="d0160-174">If successful, this method returns a `201 Created` response code and a [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d0160-175">例</span><span class="sxs-lookup"><span data-stu-id="d0160-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="d0160-176">要求</span><span class="sxs-lookup"><span data-stu-id="d0160-176">Request</span></span>
<span data-ttu-id="d0160-177">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="d0160-177">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/officeConfiguration/clientConfigurations
Content-type: application/json
Content-length: 1028

{
  "@odata.type": "#microsoft.graph.windowsOfficeClientSecurityConfiguration",
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

### <a name="response"></a><span data-ttu-id="d0160-178">応答</span><span class="sxs-lookup"><span data-stu-id="d0160-178">Response</span></span>
<span data-ttu-id="d0160-p113">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="d0160-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1077

{
  "@odata.type": "#microsoft.graph.windowsOfficeClientSecurityConfiguration",
  "id": "f90ca1a5-a1a5-f90c-a5a1-0cf9a5a10cf9",
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



