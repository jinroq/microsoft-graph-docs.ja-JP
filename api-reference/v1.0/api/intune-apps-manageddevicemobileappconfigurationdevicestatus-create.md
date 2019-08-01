---
title: ManagedDeviceMobileAppConfigurationDeviceStatus を作成する
description: 新しい managedDeviceMobileAppConfigurationDeviceStatus オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 3e0db1d11d2d0cd74a7051da030e45940b4d5e62
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36002301"
---
# <a name="create-manageddevicemobileappconfigurationdevicestatus"></a><span data-ttu-id="d4bb2-103">ManagedDeviceMobileAppConfigurationDeviceStatus を作成する</span><span class="sxs-lookup"><span data-stu-id="d4bb2-103">Create managedDeviceMobileAppConfigurationDeviceStatus</span></span>

> <span data-ttu-id="d4bb2-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="d4bb2-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d4bb2-105">新しい[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="d4bb2-105">Create a new [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d4bb2-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="d4bb2-106">Prerequisites</span></span>
<span data-ttu-id="d4bb2-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d4bb2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d4bb2-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d4bb2-109">Permission type</span></span>|<span data-ttu-id="d4bb2-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="d4bb2-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d4bb2-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d4bb2-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d4bb2-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d4bb2-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="d4bb2-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d4bb2-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d4bb2-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d4bb2-114">Not supported.</span></span>|
|<span data-ttu-id="d4bb2-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d4bb2-115">Application</span></span>|<span data-ttu-id="d4bb2-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d4bb2-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d4bb2-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d4bb2-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatuses
```

## <a name="request-headers"></a><span data-ttu-id="d4bb2-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d4bb2-118">Request headers</span></span>
|<span data-ttu-id="d4bb2-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d4bb2-119">Header</span></span>|<span data-ttu-id="d4bb2-120">値</span><span class="sxs-lookup"><span data-stu-id="d4bb2-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d4bb2-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="d4bb2-121">Authorization</span></span>|<span data-ttu-id="d4bb2-122">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="d4bb2-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d4bb2-123">承諾</span><span class="sxs-lookup"><span data-stu-id="d4bb2-123">Accept</span></span>|<span data-ttu-id="d4bb2-124">application/json</span><span class="sxs-lookup"><span data-stu-id="d4bb2-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d4bb2-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="d4bb2-125">Request body</span></span>
<span data-ttu-id="d4bb2-126">要求本文で、managedDeviceMobileAppConfigurationDeviceStatus オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="d4bb2-126">In the request body, supply a JSON representation for the managedDeviceMobileAppConfigurationDeviceStatus object.</span></span>

<span data-ttu-id="d4bb2-127">次の表に、managedDeviceMobileAppConfigurationDeviceStatus の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="d4bb2-127">The following table shows the properties that are required when you create the managedDeviceMobileAppConfigurationDeviceStatus.</span></span>

|<span data-ttu-id="d4bb2-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d4bb2-128">Property</span></span>|<span data-ttu-id="d4bb2-129">型</span><span class="sxs-lookup"><span data-stu-id="d4bb2-129">Type</span></span>|<span data-ttu-id="d4bb2-130">説明</span><span class="sxs-lookup"><span data-stu-id="d4bb2-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d4bb2-131">id</span><span class="sxs-lookup"><span data-stu-id="d4bb2-131">id</span></span>|<span data-ttu-id="d4bb2-132">文字列</span><span class="sxs-lookup"><span data-stu-id="d4bb2-132">String</span></span>|<span data-ttu-id="d4bb2-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="d4bb2-133">Key of the entity.</span></span>|
|<span data-ttu-id="d4bb2-134">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="d4bb2-134">deviceDisplayName</span></span>|<span data-ttu-id="d4bb2-135">String</span><span class="sxs-lookup"><span data-stu-id="d4bb2-135">String</span></span>|<span data-ttu-id="d4bb2-136">DevicePolicyStatus のデバイス名。</span><span class="sxs-lookup"><span data-stu-id="d4bb2-136">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="d4bb2-137">userName</span><span class="sxs-lookup"><span data-stu-id="d4bb2-137">userName</span></span>|<span data-ttu-id="d4bb2-138">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="d4bb2-138">String</span></span>|<span data-ttu-id="d4bb2-139">レポートされているユーザー名</span><span class="sxs-lookup"><span data-stu-id="d4bb2-139">The User Name that is being reported</span></span>|
|<span data-ttu-id="d4bb2-140">deviceModel</span><span class="sxs-lookup"><span data-stu-id="d4bb2-140">deviceModel</span></span>|<span data-ttu-id="d4bb2-141">String</span><span class="sxs-lookup"><span data-stu-id="d4bb2-141">String</span></span>|<span data-ttu-id="d4bb2-142">レポートされているデバイス モデル</span><span class="sxs-lookup"><span data-stu-id="d4bb2-142">The device model that is being reported</span></span>|
|<span data-ttu-id="d4bb2-143">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="d4bb2-143">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="d4bb2-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d4bb2-144">DateTimeOffset</span></span>|<span data-ttu-id="d4bb2-145">デバイス コンプライアンスの猶予期間が過ぎる DateTime</span><span class="sxs-lookup"><span data-stu-id="d4bb2-145">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="d4bb2-146">status</span><span class="sxs-lookup"><span data-stu-id="d4bb2-146">status</span></span>|[<span data-ttu-id="d4bb2-147">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="d4bb2-147">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="d4bb2-148">ポリシー レポートのコンプライアンスの状態。</span><span class="sxs-lookup"><span data-stu-id="d4bb2-148">Compliance status of the policy report.</span></span> <span data-ttu-id="d4bb2-149">可能な値は、`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned` です。</span><span class="sxs-lookup"><span data-stu-id="d4bb2-149">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="d4bb2-150">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="d4bb2-150">lastReportedDateTime</span></span>|<span data-ttu-id="d4bb2-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d4bb2-151">DateTimeOffset</span></span>|<span data-ttu-id="d4bb2-152">ポリシー レポートの最終変更日時。</span><span class="sxs-lookup"><span data-stu-id="d4bb2-152">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="d4bb2-153">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="d4bb2-153">userPrincipalName</span></span>|<span data-ttu-id="d4bb2-154">String</span><span class="sxs-lookup"><span data-stu-id="d4bb2-154">String</span></span>|<span data-ttu-id="d4bb2-155">UserPrincipalName。</span><span class="sxs-lookup"><span data-stu-id="d4bb2-155">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="d4bb2-156">応答</span><span class="sxs-lookup"><span data-stu-id="d4bb2-156">Response</span></span>
<span data-ttu-id="d4bb2-157">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="d4bb2-157">If successful, this method returns a `201 Created` response code and a [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d4bb2-158">例</span><span class="sxs-lookup"><span data-stu-id="d4bb2-158">Example</span></span>

### <a name="request"></a><span data-ttu-id="d4bb2-159">要求</span><span class="sxs-lookup"><span data-stu-id="d4bb2-159">Request</span></span>
<span data-ttu-id="d4bb2-160">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="d4bb2-160">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatuses
Content-type: application/json
Content-length: 445

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationDeviceStatus",
  "deviceDisplayName": "Device Display Name value",
  "userName": "User Name value",
  "deviceModel": "Device Model value",
  "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="d4bb2-161">応答</span><span class="sxs-lookup"><span data-stu-id="d4bb2-161">Response</span></span>
<span data-ttu-id="d4bb2-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="d4bb2-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 494

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationDeviceStatus",
  "id": "477d3651-3651-477d-5136-7d4751367d47",
  "deviceDisplayName": "Device Display Name value",
  "userName": "User Name value",
  "deviceModel": "Device Model value",
  "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```



