---
title: ManagedDeviceMobileAppConfigurationDeviceStatus を更新します。
description: ManagedDeviceMobileAppConfigurationDeviceStatus オブジェクトのプロパティを更新します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 56394f7825d180391723ffc722d58200dba9069d
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29397793"
---
# <a name="update-manageddevicemobileappconfigurationdevicestatus"></a><span data-ttu-id="f5ed8-103">ManagedDeviceMobileAppConfigurationDeviceStatus を更新します。</span><span class="sxs-lookup"><span data-stu-id="f5ed8-103">Update managedDeviceMobileAppConfigurationDeviceStatus</span></span>

> <span data-ttu-id="f5ed8-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="f5ed8-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="f5ed8-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f5ed8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f5ed8-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="f5ed8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f5ed8-107">[ManagedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="f5ed8-107">Update the properties of a [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f5ed8-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="f5ed8-108">Prerequisites</span></span>
<span data-ttu-id="f5ed8-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f5ed8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="f5ed8-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f5ed8-111">Permission type</span></span>|<span data-ttu-id="f5ed8-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="f5ed8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f5ed8-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f5ed8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f5ed8-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f5ed8-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="f5ed8-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f5ed8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f5ed8-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f5ed8-116">Not supported.</span></span>|
|<span data-ttu-id="f5ed8-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f5ed8-117">Application</span></span>|<span data-ttu-id="f5ed8-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f5ed8-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f5ed8-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f5ed8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatuses/{managedDeviceMobileAppConfigurationDeviceStatusId}
PATCH /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/deviceStatuses/{managedDeviceMobileAppConfigurationDeviceStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="f5ed8-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f5ed8-120">Request headers</span></span>
|<span data-ttu-id="f5ed8-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f5ed8-121">Header</span></span>|<span data-ttu-id="f5ed8-122">値</span><span class="sxs-lookup"><span data-stu-id="f5ed8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f5ed8-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f5ed8-123">Authorization</span></span>|<span data-ttu-id="f5ed8-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="f5ed8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f5ed8-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f5ed8-125">Accept</span></span>|<span data-ttu-id="f5ed8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f5ed8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f5ed8-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="f5ed8-127">Request body</span></span>
<span data-ttu-id="f5ed8-128">要求の本文に[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md)オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="f5ed8-128">In the request body, supply a JSON representation for the [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) object.</span></span>

<span data-ttu-id="f5ed8-129">[ManagedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md)を作成するときに必要なプロパティを次の表に示します。</span><span class="sxs-lookup"><span data-stu-id="f5ed8-129">The following table shows the properties that are required when you create the [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md).</span></span>

|<span data-ttu-id="f5ed8-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f5ed8-130">Property</span></span>|<span data-ttu-id="f5ed8-131">型</span><span class="sxs-lookup"><span data-stu-id="f5ed8-131">Type</span></span>|<span data-ttu-id="f5ed8-132">説明</span><span class="sxs-lookup"><span data-stu-id="f5ed8-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f5ed8-133">id</span><span class="sxs-lookup"><span data-stu-id="f5ed8-133">id</span></span>|<span data-ttu-id="f5ed8-134">String</span><span class="sxs-lookup"><span data-stu-id="f5ed8-134">String</span></span>|<span data-ttu-id="f5ed8-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="f5ed8-135">Key of the entity.</span></span>|
|<span data-ttu-id="f5ed8-136">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="f5ed8-136">deviceDisplayName</span></span>|<span data-ttu-id="f5ed8-137">String</span><span class="sxs-lookup"><span data-stu-id="f5ed8-137">String</span></span>|<span data-ttu-id="f5ed8-138">DevicePolicyStatus のデバイス名。</span><span class="sxs-lookup"><span data-stu-id="f5ed8-138">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="f5ed8-139">userName</span><span class="sxs-lookup"><span data-stu-id="f5ed8-139">userName</span></span>|<span data-ttu-id="f5ed8-140">String</span><span class="sxs-lookup"><span data-stu-id="f5ed8-140">String</span></span>|<span data-ttu-id="f5ed8-141">レポートされているユーザー名</span><span class="sxs-lookup"><span data-stu-id="f5ed8-141">The User Name that is being reported</span></span>|
|<span data-ttu-id="f5ed8-142">deviceModel</span><span class="sxs-lookup"><span data-stu-id="f5ed8-142">deviceModel</span></span>|<span data-ttu-id="f5ed8-143">String</span><span class="sxs-lookup"><span data-stu-id="f5ed8-143">String</span></span>|<span data-ttu-id="f5ed8-144">レポートされているデバイス モデル</span><span class="sxs-lookup"><span data-stu-id="f5ed8-144">The device model that is being reported</span></span>|
|<span data-ttu-id="f5ed8-145">platform</span><span class="sxs-lookup"><span data-stu-id="f5ed8-145">platform</span></span>|<span data-ttu-id="f5ed8-146">Int32</span><span class="sxs-lookup"><span data-stu-id="f5ed8-146">Int32</span></span>|<span data-ttu-id="f5ed8-147">報告されているデバイスのプラットフォーム</span><span class="sxs-lookup"><span data-stu-id="f5ed8-147">Platform of the device that is being reported</span></span>|
|<span data-ttu-id="f5ed8-148">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="f5ed8-148">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="f5ed8-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f5ed8-149">DateTimeOffset</span></span>|<span data-ttu-id="f5ed8-150">デバイス コンプライアンスの猶予期間が過ぎる DateTime</span><span class="sxs-lookup"><span data-stu-id="f5ed8-150">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="f5ed8-151">status</span><span class="sxs-lookup"><span data-stu-id="f5ed8-151">status</span></span>|[<span data-ttu-id="f5ed8-152">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="f5ed8-152">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="f5ed8-153">ポリシー レポートのコンプライアンスの状態。</span><span class="sxs-lookup"><span data-stu-id="f5ed8-153">Compliance status of the policy report.</span></span> <span data-ttu-id="f5ed8-154">可能な値は、`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned` です。</span><span class="sxs-lookup"><span data-stu-id="f5ed8-154">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="f5ed8-155">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="f5ed8-155">lastReportedDateTime</span></span>|<span data-ttu-id="f5ed8-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f5ed8-156">DateTimeOffset</span></span>|<span data-ttu-id="f5ed8-157">ポリシー レポートの最終変更日時。</span><span class="sxs-lookup"><span data-stu-id="f5ed8-157">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="f5ed8-158">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="f5ed8-158">userPrincipalName</span></span>|<span data-ttu-id="f5ed8-159">String</span><span class="sxs-lookup"><span data-stu-id="f5ed8-159">String</span></span>|<span data-ttu-id="f5ed8-160">UserPrincipalName。</span><span class="sxs-lookup"><span data-stu-id="f5ed8-160">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="f5ed8-161">応答</span><span class="sxs-lookup"><span data-stu-id="f5ed8-161">Response</span></span>
<span data-ttu-id="f5ed8-162">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に更新された[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="f5ed8-162">If successful, this method returns a `200 OK` response code and an updated [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f5ed8-163">例</span><span class="sxs-lookup"><span data-stu-id="f5ed8-163">Example</span></span>

### <a name="request"></a><span data-ttu-id="f5ed8-164">要求</span><span class="sxs-lookup"><span data-stu-id="f5ed8-164">Request</span></span>
<span data-ttu-id="f5ed8-165">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="f5ed8-165">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f5ed8-166">応答</span><span class="sxs-lookup"><span data-stu-id="f5ed8-166">Response</span></span>
<span data-ttu-id="f5ed8-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="f5ed8-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




