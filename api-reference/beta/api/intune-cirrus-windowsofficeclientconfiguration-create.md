---
title: windowsOfficeClientConfiguration を作成する
description: ターゲットグループを使用して、新しいセキュリティで保護されていないポリシーを作成します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 5a8e11fcf9728a554c8938d3ccf2314bf5e1999c
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30164163"
---
# <a name="create-windowsofficeclientconfiguration"></a><span data-ttu-id="717f6-103">windowsOfficeClientConfiguration を作成する</span><span class="sxs-lookup"><span data-stu-id="717f6-103">Create windowsOfficeClientConfiguration</span></span>

> <span data-ttu-id="717f6-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="717f6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="717f6-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="717f6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="717f6-106">ターゲットグループを使用して、新しいセキュリティで保護されていないポリシーを作成します。</span><span class="sxs-lookup"><span data-stu-id="717f6-106">Create a new non-security policy with targeting groups.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="717f6-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="717f6-107">Prerequisites</span></span>
<span data-ttu-id="717f6-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="717f6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="717f6-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="717f6-110">Permission type</span></span>|<span data-ttu-id="717f6-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="717f6-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="717f6-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="717f6-112">Delegated (work or school account)</span></span>|<span data-ttu-id="717f6-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="717f6-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="717f6-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="717f6-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="717f6-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="717f6-115">Not supported.</span></span>|
|<span data-ttu-id="717f6-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="717f6-116">Application</span></span>|<span data-ttu-id="717f6-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="717f6-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="717f6-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="717f6-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /officeConfiguration/clientConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="717f6-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="717f6-119">Request headers</span></span>
|<span data-ttu-id="717f6-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="717f6-120">Header</span></span>|<span data-ttu-id="717f6-121">値</span><span class="sxs-lookup"><span data-stu-id="717f6-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="717f6-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="717f6-122">Authorization</span></span>|<span data-ttu-id="717f6-123">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="717f6-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="717f6-124">承諾</span><span class="sxs-lookup"><span data-stu-id="717f6-124">Accept</span></span>|<span data-ttu-id="717f6-125">application/json</span><span class="sxs-lookup"><span data-stu-id="717f6-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="717f6-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="717f6-126">Request body</span></span>
<span data-ttu-id="717f6-127">要求本文で、 [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="717f6-127">In the request body, supply a JSON representation for the [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md) object.</span></span>

<span data-ttu-id="717f6-128">次の表に、 [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="717f6-128">The following table shows the properties that are required when you create the [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md).</span></span>

|<span data-ttu-id="717f6-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="717f6-129">Property</span></span>|<span data-ttu-id="717f6-130">型</span><span class="sxs-lookup"><span data-stu-id="717f6-130">Type</span></span>|<span data-ttu-id="717f6-131">説明</span><span class="sxs-lookup"><span data-stu-id="717f6-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="717f6-132">id</span><span class="sxs-lookup"><span data-stu-id="717f6-132">id</span></span>|<span data-ttu-id="717f6-133">文字列</span><span class="sxs-lookup"><span data-stu-id="717f6-133">String</span></span>|<span data-ttu-id="717f6-134">office クライアント構成ポリシーの Id。</span><span class="sxs-lookup"><span data-stu-id="717f6-134">Id of the office client configuration policy.</span></span> <span data-ttu-id="717f6-135">[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="717f6-135">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="717f6-136">userPreferencePayload</span><span class="sxs-lookup"><span data-stu-id="717f6-136">userPreferencePayload</span></span>|<span data-ttu-id="717f6-137">Stream</span><span class="sxs-lookup"><span data-stu-id="717f6-137">Stream</span></span>|<span data-ttu-id="717f6-138">プリファレンス設定 JSON 文字列はバイナリ形式です。これらの値はユーザーが上書きできます。</span><span class="sxs-lookup"><span data-stu-id="717f6-138">Preference settings JSON string in binary format, these values can be overridden by the user.</span></span> <span data-ttu-id="717f6-139">[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="717f6-139">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="717f6-140">policypayload</span><span class="sxs-lookup"><span data-stu-id="717f6-140">policyPayload</span></span>|<span data-ttu-id="717f6-141">Stream</span><span class="sxs-lookup"><span data-stu-id="717f6-141">Stream</span></span>|<span data-ttu-id="717f6-142">ポリシー設定 JSON 文字列 (バイナリ形式) では、ユーザーがこれらの値を変更することはできません。</span><span class="sxs-lookup"><span data-stu-id="717f6-142">Policy settings JSON string in binary format, these values cannot be changed by the user.</span></span> <span data-ttu-id="717f6-143">[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="717f6-143">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="717f6-144">説明</span><span class="sxs-lookup"><span data-stu-id="717f6-144">description</span></span>|<span data-ttu-id="717f6-145">String</span><span class="sxs-lookup"><span data-stu-id="717f6-145">String</span></span>|<span data-ttu-id="717f6-146">管理者が提供する office クライアント構成ポリシーの説明。</span><span class="sxs-lookup"><span data-stu-id="717f6-146">Admin provided description of the office client configuration policy.</span></span> <span data-ttu-id="717f6-147">[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="717f6-147">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="717f6-148">displayName</span><span class="sxs-lookup"><span data-stu-id="717f6-148">displayName</span></span>|<span data-ttu-id="717f6-149">String</span><span class="sxs-lookup"><span data-stu-id="717f6-149">String</span></span>|<span data-ttu-id="717f6-150">管理者が指定した office クライアント構成ポリシーの名前。</span><span class="sxs-lookup"><span data-stu-id="717f6-150">Admin provided name of the office client configuration policy.</span></span> <span data-ttu-id="717f6-151">[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="717f6-151">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="717f6-152">assignments</span><span class="sxs-lookup"><span data-stu-id="717f6-152">assignments</span></span>|<span data-ttu-id="717f6-153">[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="717f6-153">[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) collection</span></span>|<span data-ttu-id="717f6-154">ポリシーのグループの割り当てのリスト。</span><span class="sxs-lookup"><span data-stu-id="717f6-154">The list of group assignments for the policy..</span></span> <span data-ttu-id="717f6-155">[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="717f6-155">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="717f6-156">priority</span><span class="sxs-lookup"><span data-stu-id="717f6-156">priority</span></span>|<span data-ttu-id="717f6-157">Int32</span><span class="sxs-lookup"><span data-stu-id="717f6-157">Int32</span></span>|<span data-ttu-id="717f6-158">優先度の値は、テナントの各ポリシーの一意の値である必要があり、競合の解決に使用されます。低い値は、優先度が高くなります。</span><span class="sxs-lookup"><span data-stu-id="717f6-158">Priority value should be unique value for each policy under a tenant and will be used for conflict resolution, lower values mean priority is high.</span></span> <span data-ttu-id="717f6-159">[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="717f6-159">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="717f6-160">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="717f6-160">lastModifiedDateTime</span></span>|<span data-ttu-id="717f6-161">DateTime
</span><span class="sxs-lookup"><span data-stu-id="717f6-161">DateTime</span></span>|<span data-ttu-id="717f6-162">ポリシーの最終更新日時スタンプ。</span><span class="sxs-lookup"><span data-stu-id="717f6-162">Last modified datetime stamp of the policy.</span></span> <span data-ttu-id="717f6-163">[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="717f6-163">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="717f6-164">userCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="717f6-164">userCheckinSummary</span></span>|[<span data-ttu-id="717f6-165">officeUserCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="717f6-165">officeUserCheckinSummary</span></span>](../resources/intune-cirrus-officeusercheckinsummary.md)|<span data-ttu-id="717f6-166">ポリシーのユーザーチェックインの概要。</span><span class="sxs-lookup"><span data-stu-id="717f6-166">User check-in summary for the policy.</span></span> <span data-ttu-id="717f6-167">[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="717f6-167">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="717f6-168">checkinstatuses</span><span class="sxs-lookup"><span data-stu-id="717f6-168">checkinStatuses</span></span>|<span data-ttu-id="717f6-169">[officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="717f6-169">[officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md) collection</span></span>|<span data-ttu-id="717f6-170">office クライアントのチェックイン状態のリスト。</span><span class="sxs-lookup"><span data-stu-id="717f6-170">List of office Client check-in status.</span></span> <span data-ttu-id="717f6-171">[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="717f6-171">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="717f6-172">応答</span><span class="sxs-lookup"><span data-stu-id="717f6-172">Response</span></span>
<span data-ttu-id="717f6-173">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="717f6-173">If successful, this method returns a `201 Created` response code and a [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="717f6-174">例</span><span class="sxs-lookup"><span data-stu-id="717f6-174">Example</span></span>

### <a name="request"></a><span data-ttu-id="717f6-175">要求</span><span class="sxs-lookup"><span data-stu-id="717f6-175">Request</span></span>
<span data-ttu-id="717f6-176">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="717f6-176">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/officeConfiguration/clientConfigurations
Content-type: application/json
Content-length: 1020

{
  "@odata.type": "#microsoft.graph.windowsOfficeClientConfiguration",
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

### <a name="response"></a><span data-ttu-id="717f6-177">応答</span><span class="sxs-lookup"><span data-stu-id="717f6-177">Response</span></span>
<span data-ttu-id="717f6-p112">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="717f6-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



