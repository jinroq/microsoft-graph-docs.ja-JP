---
title: WindowsOfficeClientConfiguration を作成します。
description: グループを対象とすると、セキュリティ以外の新しいポリシーを作成します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: a915447ad22438d021bb4577fc856bbe89db1fdc
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29394377"
---
# <a name="create-windowsofficeclientconfiguration"></a><span data-ttu-id="0c809-103">WindowsOfficeClientConfiguration を作成します。</span><span class="sxs-lookup"><span data-stu-id="0c809-103">Create windowsOfficeClientConfiguration</span></span>

> <span data-ttu-id="0c809-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="0c809-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="0c809-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0c809-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0c809-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="0c809-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0c809-107">グループを対象とすると、セキュリティ以外の新しいポリシーを作成します。</span><span class="sxs-lookup"><span data-stu-id="0c809-107">Create a new non-security policy with targeting groups.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0c809-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="0c809-108">Prerequisites</span></span>
<span data-ttu-id="0c809-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0c809-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0c809-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0c809-111">Permission type</span></span>|<span data-ttu-id="0c809-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="0c809-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0c809-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0c809-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0c809-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0c809-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0c809-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0c809-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0c809-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0c809-116">Not supported.</span></span>|
|<span data-ttu-id="0c809-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0c809-117">Application</span></span>|<span data-ttu-id="0c809-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0c809-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0c809-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0c809-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /officeConfiguration/clientConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="0c809-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0c809-120">Request headers</span></span>
|<span data-ttu-id="0c809-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0c809-121">Header</span></span>|<span data-ttu-id="0c809-122">値</span><span class="sxs-lookup"><span data-stu-id="0c809-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0c809-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0c809-123">Authorization</span></span>|<span data-ttu-id="0c809-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="0c809-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0c809-125">Accept</span><span class="sxs-lookup"><span data-stu-id="0c809-125">Accept</span></span>|<span data-ttu-id="0c809-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0c809-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0c809-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="0c809-127">Request body</span></span>
<span data-ttu-id="0c809-128">要求の本文に[windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md)オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="0c809-128">In the request body, supply a JSON representation for the [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md) object.</span></span>

<span data-ttu-id="0c809-129">[WindowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md)を作成するときに必要なプロパティを次の表に示します。</span><span class="sxs-lookup"><span data-stu-id="0c809-129">The following table shows the properties that are required when you create the [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md).</span></span>

|<span data-ttu-id="0c809-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0c809-130">Property</span></span>|<span data-ttu-id="0c809-131">型</span><span class="sxs-lookup"><span data-stu-id="0c809-131">Type</span></span>|<span data-ttu-id="0c809-132">説明</span><span class="sxs-lookup"><span data-stu-id="0c809-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0c809-133">id</span><span class="sxs-lookup"><span data-stu-id="0c809-133">id</span></span>|<span data-ttu-id="0c809-134">String</span><span class="sxs-lookup"><span data-stu-id="0c809-134">String</span></span>|<span data-ttu-id="0c809-135">Office クライアントの構成のポリシーの id。</span><span class="sxs-lookup"><span data-stu-id="0c809-135">Id of the office client configuration policy.</span></span> <span data-ttu-id="0c809-136">[OfficeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="0c809-136">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="0c809-137">userPreferencePayload</span><span class="sxs-lookup"><span data-stu-id="0c809-137">userPreferencePayload</span></span>|<span data-ttu-id="0c809-138">Stream</span><span class="sxs-lookup"><span data-stu-id="0c809-138">Stream</span></span>|<span data-ttu-id="0c809-139">JSON の環境設定は、バイナリ形式の文字列は、ユーザーがこれらの値をオーバーライドすることができます。</span><span class="sxs-lookup"><span data-stu-id="0c809-139">Preference settings JSON string in binary format, these values can be overridden by the user.</span></span> <span data-ttu-id="0c809-140">[OfficeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="0c809-140">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="0c809-141">policyPayload</span><span class="sxs-lookup"><span data-stu-id="0c809-141">policyPayload</span></span>|<span data-ttu-id="0c809-142">Stream</span><span class="sxs-lookup"><span data-stu-id="0c809-142">Stream</span></span>|<span data-ttu-id="0c809-143">JSON のポリシー設定はバイナリ形式の文字列は、ユーザーがこれらの値を変更することはできません。</span><span class="sxs-lookup"><span data-stu-id="0c809-143">Policy settings JSON string in binary format, these values cannot be changed by the user.</span></span> <span data-ttu-id="0c809-144">[OfficeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="0c809-144">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="0c809-145">説明</span><span class="sxs-lookup"><span data-stu-id="0c809-145">description</span></span>|<span data-ttu-id="0c809-146">String</span><span class="sxs-lookup"><span data-stu-id="0c809-146">String</span></span>|<span data-ttu-id="0c809-147">管理者には、office クライアントの説明の構成のポリシーが用意されています。</span><span class="sxs-lookup"><span data-stu-id="0c809-147">Admin provided description of the office client configuration policy.</span></span> <span data-ttu-id="0c809-148">[OfficeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="0c809-148">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="0c809-149">displayName</span><span class="sxs-lookup"><span data-stu-id="0c809-149">displayName</span></span>|<span data-ttu-id="0c809-150">String</span><span class="sxs-lookup"><span data-stu-id="0c809-150">String</span></span>|<span data-ttu-id="0c809-151">管理者は、office クライアントの構成のポリシーの名前を提供します。</span><span class="sxs-lookup"><span data-stu-id="0c809-151">Admin provided name of the office client configuration policy.</span></span> <span data-ttu-id="0c809-152">[OfficeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="0c809-152">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="0c809-153">assignments</span><span class="sxs-lookup"><span data-stu-id="0c809-153">assignments</span></span>|<span data-ttu-id="0c809-154">[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="0c809-154">[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) collection</span></span>|<span data-ttu-id="0c809-155">一連のポリシーの割り当てをグループ化.</span><span class="sxs-lookup"><span data-stu-id="0c809-155">The list of group assignments for the policy..</span></span> <span data-ttu-id="0c809-156">[OfficeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="0c809-156">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="0c809-157">priority</span><span class="sxs-lookup"><span data-stu-id="0c809-157">priority</span></span>|<span data-ttu-id="0c809-158">Int32</span><span class="sxs-lookup"><span data-stu-id="0c809-158">Int32</span></span>|<span data-ttu-id="0c809-159">優先度の値がテナントの下にある各ポリシーの一意の値にする必要があり、競合の解決に使用する、値が低い優先順位が高いことを意味します。</span><span class="sxs-lookup"><span data-stu-id="0c809-159">Priority value should be unique value for each policy under a tenant and will be used for conflict resolution, lower values mean priority is high.</span></span> <span data-ttu-id="0c809-160">[OfficeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="0c809-160">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="0c809-161">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0c809-161">lastModifiedDateTime</span></span>|<span data-ttu-id="0c809-162">DateTime
</span><span class="sxs-lookup"><span data-stu-id="0c809-162">DateTime</span></span>|<span data-ttu-id="0c809-163">ポリシーの最終変更された日付時刻スタンプ。</span><span class="sxs-lookup"><span data-stu-id="0c809-163">Last modified datetime stamp of the policy.</span></span> <span data-ttu-id="0c809-164">[OfficeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="0c809-164">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="0c809-165">userCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="0c809-165">userCheckinSummary</span></span>|[<span data-ttu-id="0c809-166">officeUserCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="0c809-166">officeUserCheckinSummary</span></span>](../resources/intune-cirrus-officeusercheckinsummary.md)|<span data-ttu-id="0c809-167">ポリシーの概要チェックのユーザーです。</span><span class="sxs-lookup"><span data-stu-id="0c809-167">User check-in summary for the policy.</span></span> <span data-ttu-id="0c809-168">[OfficeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="0c809-168">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="0c809-169">checkinStatuses</span><span class="sxs-lookup"><span data-stu-id="0c809-169">checkinStatuses</span></span>|<span data-ttu-id="0c809-170">[officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="0c809-170">[officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md) collection</span></span>|<span data-ttu-id="0c809-171">Office クライアントでは、チェック状態の一覧です。</span><span class="sxs-lookup"><span data-stu-id="0c809-171">List of office Client check-in status.</span></span> <span data-ttu-id="0c809-172">[OfficeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="0c809-172">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="0c809-173">応答</span><span class="sxs-lookup"><span data-stu-id="0c809-173">Response</span></span>
<span data-ttu-id="0c809-174">かどうかは成功すると、このメソッドが返されます、`201 Created`応答コードおよび応答の本文に[windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="0c809-174">If successful, this method returns a `201 Created` response code and a [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0c809-175">例</span><span class="sxs-lookup"><span data-stu-id="0c809-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="0c809-176">要求</span><span class="sxs-lookup"><span data-stu-id="0c809-176">Request</span></span>
<span data-ttu-id="0c809-177">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="0c809-177">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="0c809-178">応答</span><span class="sxs-lookup"><span data-stu-id="0c809-178">Response</span></span>
<span data-ttu-id="0c809-p113">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="0c809-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



