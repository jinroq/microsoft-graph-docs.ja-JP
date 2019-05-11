---
title: WindowsOfficeClientSecurityConfiguration の更新
description: WindowsOfficeClientSecurityConfiguration オブジェクトのプロパティを更新します。
localization_priority: Normal
author: rolyon
ms.prod: Intune
ms.openlocfilehash: 87f6378c8f2febcb01d836dcc82a4cb4f765b984
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33933922"
---
# <a name="update-windowsofficeclientsecurityconfiguration"></a><span data-ttu-id="ce2dd-103">WindowsOfficeClientSecurityConfiguration の更新</span><span class="sxs-lookup"><span data-stu-id="ce2dd-103">Update windowsOfficeClientSecurityConfiguration</span></span>

> <span data-ttu-id="ce2dd-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ce2dd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ce2dd-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="ce2dd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ce2dd-106">[WindowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="ce2dd-106">Update the properties of a [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ce2dd-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="ce2dd-107">Prerequisites</span></span>
<span data-ttu-id="ce2dd-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ce2dd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ce2dd-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ce2dd-110">Permission type</span></span>|<span data-ttu-id="ce2dd-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="ce2dd-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ce2dd-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ce2dd-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ce2dd-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ce2dd-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ce2dd-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ce2dd-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ce2dd-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ce2dd-115">Not supported.</span></span>|
|<span data-ttu-id="ce2dd-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ce2dd-116">Application</span></span>|<span data-ttu-id="ce2dd-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ce2dd-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ce2dd-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ce2dd-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /officeConfiguration/clientConfigurations/{officeClientConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="ce2dd-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ce2dd-119">Request headers</span></span>
|<span data-ttu-id="ce2dd-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ce2dd-120">Header</span></span>|<span data-ttu-id="ce2dd-121">値</span><span class="sxs-lookup"><span data-stu-id="ce2dd-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ce2dd-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ce2dd-122">Authorization</span></span>|<span data-ttu-id="ce2dd-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="ce2dd-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ce2dd-124">承諾</span><span class="sxs-lookup"><span data-stu-id="ce2dd-124">Accept</span></span>|<span data-ttu-id="ce2dd-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ce2dd-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ce2dd-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="ce2dd-126">Request body</span></span>
<span data-ttu-id="ce2dd-127">要求本文で、 [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="ce2dd-127">In the request body, supply a JSON representation for the [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) object.</span></span>

<span data-ttu-id="ce2dd-128">次の表に、 [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="ce2dd-128">The following table shows the properties that are required when you create the [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md).</span></span>

|<span data-ttu-id="ce2dd-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ce2dd-129">Property</span></span>|<span data-ttu-id="ce2dd-130">型</span><span class="sxs-lookup"><span data-stu-id="ce2dd-130">Type</span></span>|<span data-ttu-id="ce2dd-131">説明</span><span class="sxs-lookup"><span data-stu-id="ce2dd-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ce2dd-132">id</span><span class="sxs-lookup"><span data-stu-id="ce2dd-132">id</span></span>|<span data-ttu-id="ce2dd-133">文字列</span><span class="sxs-lookup"><span data-stu-id="ce2dd-133">String</span></span>|<span data-ttu-id="ce2dd-134">Office クライアント構成ポリシーの Id。</span><span class="sxs-lookup"><span data-stu-id="ce2dd-134">Id of the office client configuration policy.</span></span> <span data-ttu-id="ce2dd-135">[OfficeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="ce2dd-135">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="ce2dd-136">userPreferencePayload</span><span class="sxs-lookup"><span data-stu-id="ce2dd-136">userPreferencePayload</span></span>|<span data-ttu-id="ce2dd-137">Stream</span><span class="sxs-lookup"><span data-stu-id="ce2dd-137">Stream</span></span>|<span data-ttu-id="ce2dd-138">プリファレンス設定 JSON 文字列はバイナリ形式です。これらの値はユーザーが上書きできます。</span><span class="sxs-lookup"><span data-stu-id="ce2dd-138">Preference settings JSON string in binary format, these values can be overridden by the user.</span></span> <span data-ttu-id="ce2dd-139">[OfficeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="ce2dd-139">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="ce2dd-140">policyPayload</span><span class="sxs-lookup"><span data-stu-id="ce2dd-140">policyPayload</span></span>|<span data-ttu-id="ce2dd-141">Stream</span><span class="sxs-lookup"><span data-stu-id="ce2dd-141">Stream</span></span>|<span data-ttu-id="ce2dd-142">ポリシー設定 JSON 文字列 (バイナリ形式) では、ユーザーがこれらの値を変更することはできません。</span><span class="sxs-lookup"><span data-stu-id="ce2dd-142">Policy settings JSON string in binary format, these values cannot be changed by the user.</span></span> <span data-ttu-id="ce2dd-143">[OfficeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="ce2dd-143">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="ce2dd-144">description</span><span class="sxs-lookup"><span data-stu-id="ce2dd-144">description</span></span>|<span data-ttu-id="ce2dd-145">String</span><span class="sxs-lookup"><span data-stu-id="ce2dd-145">String</span></span>|<span data-ttu-id="ce2dd-146">管理者が提供する office クライアント構成ポリシーの説明。</span><span class="sxs-lookup"><span data-stu-id="ce2dd-146">Admin provided description of the office client configuration policy.</span></span> <span data-ttu-id="ce2dd-147">[OfficeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="ce2dd-147">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="ce2dd-148">displayName</span><span class="sxs-lookup"><span data-stu-id="ce2dd-148">displayName</span></span>|<span data-ttu-id="ce2dd-149">String</span><span class="sxs-lookup"><span data-stu-id="ce2dd-149">String</span></span>|<span data-ttu-id="ce2dd-150">管理者が指定した office クライアント構成ポリシーの名前。</span><span class="sxs-lookup"><span data-stu-id="ce2dd-150">Admin provided name of the office client configuration policy.</span></span> <span data-ttu-id="ce2dd-151">[OfficeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="ce2dd-151">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="ce2dd-152">assignments</span><span class="sxs-lookup"><span data-stu-id="ce2dd-152">assignments</span></span>|<span data-ttu-id="ce2dd-153">[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="ce2dd-153">[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) collection</span></span>|<span data-ttu-id="ce2dd-154">ポリシーのグループの割り当てのリスト。</span><span class="sxs-lookup"><span data-stu-id="ce2dd-154">The list of group assignments for the policy..</span></span> <span data-ttu-id="ce2dd-155">[OfficeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="ce2dd-155">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="ce2dd-156">priority</span><span class="sxs-lookup"><span data-stu-id="ce2dd-156">priority</span></span>|<span data-ttu-id="ce2dd-157">Int32</span><span class="sxs-lookup"><span data-stu-id="ce2dd-157">Int32</span></span>|<span data-ttu-id="ce2dd-158">優先度の値は、テナントの各ポリシーの一意の値である必要があり、競合の解決に使用されます。低い値は、優先度が高くなります。</span><span class="sxs-lookup"><span data-stu-id="ce2dd-158">Priority value should be unique value for each policy under a tenant and will be used for conflict resolution, lower values mean priority is high.</span></span> <span data-ttu-id="ce2dd-159">[OfficeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="ce2dd-159">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="ce2dd-160">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ce2dd-160">lastModifiedDateTime</span></span>|<span data-ttu-id="ce2dd-161">DateTime</span><span class="sxs-lookup"><span data-stu-id="ce2dd-161">DateTime</span></span>|<span data-ttu-id="ce2dd-162">ポリシーの最終更新日時スタンプ。</span><span class="sxs-lookup"><span data-stu-id="ce2dd-162">Last modified datetime stamp of the policy.</span></span> <span data-ttu-id="ce2dd-163">[OfficeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="ce2dd-163">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="ce2dd-164">userCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="ce2dd-164">userCheckinSummary</span></span>|[<span data-ttu-id="ce2dd-165">officeUserCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="ce2dd-165">officeUserCheckinSummary</span></span>](../resources/intune-cirrus-officeusercheckinsummary.md)|<span data-ttu-id="ce2dd-166">ポリシーのユーザーチェックインの概要。</span><span class="sxs-lookup"><span data-stu-id="ce2dd-166">User check-in summary for the policy.</span></span> <span data-ttu-id="ce2dd-167">[OfficeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="ce2dd-167">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="ce2dd-168">checkinStatuses</span><span class="sxs-lookup"><span data-stu-id="ce2dd-168">checkinStatuses</span></span>|<span data-ttu-id="ce2dd-169">[officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="ce2dd-169">[officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md) collection</span></span>|<span data-ttu-id="ce2dd-170">Office クライアントのチェックイン状態のリスト。</span><span class="sxs-lookup"><span data-stu-id="ce2dd-170">List of office Client check-in status.</span></span> <span data-ttu-id="ce2dd-171">[OfficeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="ce2dd-171">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="ce2dd-172">応答</span><span class="sxs-lookup"><span data-stu-id="ce2dd-172">Response</span></span>
<span data-ttu-id="ce2dd-173">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="ce2dd-173">If successful, this method returns a `200 OK` response code and an updated [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ce2dd-174">例</span><span class="sxs-lookup"><span data-stu-id="ce2dd-174">Example</span></span>

### <a name="request"></a><span data-ttu-id="ce2dd-175">要求</span><span class="sxs-lookup"><span data-stu-id="ce2dd-175">Request</span></span>
<span data-ttu-id="ce2dd-176">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ce2dd-176">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="ce2dd-177">応答</span><span class="sxs-lookup"><span data-stu-id="ce2dd-177">Response</span></span>
<span data-ttu-id="ce2dd-p112">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="ce2dd-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



