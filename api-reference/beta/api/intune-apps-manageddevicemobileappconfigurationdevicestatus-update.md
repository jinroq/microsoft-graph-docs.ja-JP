---
title: managedDeviceMobileAppConfigurationDeviceStatus の更新
description: managedDeviceMobileAppConfigurationDeviceStatus オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 48afdece32d82d0112ebc77cf13fa71ff1b175d1
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/29/2019
ms.locfileid: "30961946"
---
# <a name="update-manageddevicemobileappconfigurationdevicestatus"></a><span data-ttu-id="457f0-103">managedDeviceMobileAppConfigurationDeviceStatus の更新</span><span class="sxs-lookup"><span data-stu-id="457f0-103">Update managedDeviceMobileAppConfigurationDeviceStatus</span></span>

> <span data-ttu-id="457f0-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="457f0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="457f0-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="457f0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="457f0-106">[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="457f0-106">Update the properties of a [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="457f0-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="457f0-107">Prerequisites</span></span>
<span data-ttu-id="457f0-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="457f0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="457f0-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="457f0-110">Permission type</span></span>|<span data-ttu-id="457f0-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="457f0-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="457f0-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="457f0-112">Delegated (work or school account)</span></span>|<span data-ttu-id="457f0-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="457f0-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="457f0-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="457f0-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="457f0-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="457f0-115">Not supported.</span></span>|
|<span data-ttu-id="457f0-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="457f0-116">Application</span></span>|<span data-ttu-id="457f0-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="457f0-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="457f0-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="457f0-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatuses/{managedDeviceMobileAppConfigurationDeviceStatusId}
PATCH /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/deviceStatuses/{managedDeviceMobileAppConfigurationDeviceStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="457f0-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="457f0-119">Request headers</span></span>
|<span data-ttu-id="457f0-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="457f0-120">Header</span></span>|<span data-ttu-id="457f0-121">値</span><span class="sxs-lookup"><span data-stu-id="457f0-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="457f0-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="457f0-122">Authorization</span></span>|<span data-ttu-id="457f0-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="457f0-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="457f0-124">承諾</span><span class="sxs-lookup"><span data-stu-id="457f0-124">Accept</span></span>|<span data-ttu-id="457f0-125">application/json</span><span class="sxs-lookup"><span data-stu-id="457f0-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="457f0-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="457f0-126">Request body</span></span>
<span data-ttu-id="457f0-127">要求本文で、 [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="457f0-127">In the request body, supply a JSON representation for the [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) object.</span></span>

<span data-ttu-id="457f0-128">次の表に、 [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="457f0-128">The following table shows the properties that are required when you create the [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md).</span></span>

|<span data-ttu-id="457f0-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="457f0-129">Property</span></span>|<span data-ttu-id="457f0-130">型</span><span class="sxs-lookup"><span data-stu-id="457f0-130">Type</span></span>|<span data-ttu-id="457f0-131">説明</span><span class="sxs-lookup"><span data-stu-id="457f0-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="457f0-132">id</span><span class="sxs-lookup"><span data-stu-id="457f0-132">id</span></span>|<span data-ttu-id="457f0-133">String</span><span class="sxs-lookup"><span data-stu-id="457f0-133">String</span></span>|<span data-ttu-id="457f0-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="457f0-134">Key of the entity.</span></span>|
|<span data-ttu-id="457f0-135">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="457f0-135">deviceDisplayName</span></span>|<span data-ttu-id="457f0-136">String</span><span class="sxs-lookup"><span data-stu-id="457f0-136">String</span></span>|<span data-ttu-id="457f0-137">DevicePolicyStatus のデバイス名。</span><span class="sxs-lookup"><span data-stu-id="457f0-137">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="457f0-138">userName</span><span class="sxs-lookup"><span data-stu-id="457f0-138">userName</span></span>|<span data-ttu-id="457f0-139">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="457f0-139">String</span></span>|<span data-ttu-id="457f0-140">レポートされているユーザー名</span><span class="sxs-lookup"><span data-stu-id="457f0-140">The User Name that is being reported</span></span>|
|<span data-ttu-id="457f0-141">deviceModel</span><span class="sxs-lookup"><span data-stu-id="457f0-141">deviceModel</span></span>|<span data-ttu-id="457f0-142">String</span><span class="sxs-lookup"><span data-stu-id="457f0-142">String</span></span>|<span data-ttu-id="457f0-143">レポートされているデバイス モデル</span><span class="sxs-lookup"><span data-stu-id="457f0-143">The device model that is being reported</span></span>|
|<span data-ttu-id="457f0-144">platform</span><span class="sxs-lookup"><span data-stu-id="457f0-144">platform</span></span>|<span data-ttu-id="457f0-145">Int32</span><span class="sxs-lookup"><span data-stu-id="457f0-145">Int32</span></span>|<span data-ttu-id="457f0-146">レポートされているデバイスのプラットフォーム</span><span class="sxs-lookup"><span data-stu-id="457f0-146">Platform of the device that is being reported</span></span>|
|<span data-ttu-id="457f0-147">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="457f0-147">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="457f0-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="457f0-148">DateTimeOffset</span></span>|<span data-ttu-id="457f0-149">デバイス コンプライアンスの猶予期間が過ぎる DateTime</span><span class="sxs-lookup"><span data-stu-id="457f0-149">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="457f0-150">status</span><span class="sxs-lookup"><span data-stu-id="457f0-150">status</span></span>|[<span data-ttu-id="457f0-151">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="457f0-151">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="457f0-152">ポリシー レポートのコンプライアンスの状態。</span><span class="sxs-lookup"><span data-stu-id="457f0-152">Compliance status of the policy report.</span></span> <span data-ttu-id="457f0-153">可能な値は、`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned` です。</span><span class="sxs-lookup"><span data-stu-id="457f0-153">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="457f0-154">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="457f0-154">lastReportedDateTime</span></span>|<span data-ttu-id="457f0-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="457f0-155">DateTimeOffset</span></span>|<span data-ttu-id="457f0-156">ポリシー レポートの最終変更日時。</span><span class="sxs-lookup"><span data-stu-id="457f0-156">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="457f0-157">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="457f0-157">userPrincipalName</span></span>|<span data-ttu-id="457f0-158">String</span><span class="sxs-lookup"><span data-stu-id="457f0-158">String</span></span>|<span data-ttu-id="457f0-159">UserPrincipalName。</span><span class="sxs-lookup"><span data-stu-id="457f0-159">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="457f0-160">応答</span><span class="sxs-lookup"><span data-stu-id="457f0-160">Response</span></span>
<span data-ttu-id="457f0-161">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="457f0-161">If successful, this method returns a `200 OK` response code and an updated [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="457f0-162">例</span><span class="sxs-lookup"><span data-stu-id="457f0-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="457f0-163">要求</span><span class="sxs-lookup"><span data-stu-id="457f0-163">Request</span></span>
<span data-ttu-id="457f0-164">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="457f0-164">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatuses/{managedDeviceMobileAppConfigurationDeviceStatusId}
Content-type: application/json
Content-length: 463

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationDeviceStatus",
  "deviceDisplayName": "Device Display Name value",
  "userName": "User Name value",
  "deviceModel": "Device Model value",
  "platform": 8,
  "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="457f0-165">応答</span><span class="sxs-lookup"><span data-stu-id="457f0-165">Response</span></span>
<span data-ttu-id="457f0-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="457f0-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 512

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationDeviceStatus",
  "id": "477d3651-3651-477d-5136-7d4751367d47",
  "deviceDisplayName": "Device Display Name value",
  "userName": "User Name value",
  "deviceModel": "Device Model value",
  "platform": 8,
  "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```




