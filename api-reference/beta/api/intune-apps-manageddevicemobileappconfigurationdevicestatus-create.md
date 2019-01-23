---
title: ManagedDeviceMobileAppConfigurationDeviceStatus を作成します。
description: 新しい managedDeviceMobileAppConfigurationDeviceStatus オブジェクトを作成します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 93d6ac158fc1196ce02c8e09ec997bc3827f8e08
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29408923"
---
# <a name="create-manageddevicemobileappconfigurationdevicestatus"></a><span data-ttu-id="2ebf0-103">ManagedDeviceMobileAppConfigurationDeviceStatus を作成します。</span><span class="sxs-lookup"><span data-stu-id="2ebf0-103">Create managedDeviceMobileAppConfigurationDeviceStatus</span></span>

> <span data-ttu-id="2ebf0-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="2ebf0-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="2ebf0-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2ebf0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2ebf0-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="2ebf0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2ebf0-107">新しい[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="2ebf0-107">Create a new [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2ebf0-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="2ebf0-108">Prerequisites</span></span>
<span data-ttu-id="2ebf0-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2ebf0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="2ebf0-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="2ebf0-111">Permission type</span></span>|<span data-ttu-id="2ebf0-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="2ebf0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2ebf0-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="2ebf0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2ebf0-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2ebf0-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="2ebf0-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="2ebf0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2ebf0-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2ebf0-116">Not supported.</span></span>|
|<span data-ttu-id="2ebf0-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="2ebf0-117">Application</span></span>|<span data-ttu-id="2ebf0-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2ebf0-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2ebf0-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="2ebf0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatuses
POST /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/deviceStatuses
```

## <a name="request-headers"></a><span data-ttu-id="2ebf0-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2ebf0-120">Request headers</span></span>
|<span data-ttu-id="2ebf0-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2ebf0-121">Header</span></span>|<span data-ttu-id="2ebf0-122">値</span><span class="sxs-lookup"><span data-stu-id="2ebf0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2ebf0-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2ebf0-123">Authorization</span></span>|<span data-ttu-id="2ebf0-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="2ebf0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2ebf0-125">Accept</span><span class="sxs-lookup"><span data-stu-id="2ebf0-125">Accept</span></span>|<span data-ttu-id="2ebf0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2ebf0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2ebf0-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="2ebf0-127">Request body</span></span>
<span data-ttu-id="2ebf0-128">要求の本文に managedDeviceMobileAppConfigurationDeviceStatus オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="2ebf0-128">In the request body, supply a JSON representation for the managedDeviceMobileAppConfigurationDeviceStatus object.</span></span>

<span data-ttu-id="2ebf0-129">次の表は、managedDeviceMobileAppConfigurationDeviceStatus を作成するときに必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="2ebf0-129">The following table shows the properties that are required when you create the managedDeviceMobileAppConfigurationDeviceStatus.</span></span>

|<span data-ttu-id="2ebf0-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2ebf0-130">Property</span></span>|<span data-ttu-id="2ebf0-131">型</span><span class="sxs-lookup"><span data-stu-id="2ebf0-131">Type</span></span>|<span data-ttu-id="2ebf0-132">説明</span><span class="sxs-lookup"><span data-stu-id="2ebf0-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2ebf0-133">id</span><span class="sxs-lookup"><span data-stu-id="2ebf0-133">id</span></span>|<span data-ttu-id="2ebf0-134">String</span><span class="sxs-lookup"><span data-stu-id="2ebf0-134">String</span></span>|<span data-ttu-id="2ebf0-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="2ebf0-135">Key of the entity.</span></span>|
|<span data-ttu-id="2ebf0-136">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="2ebf0-136">deviceDisplayName</span></span>|<span data-ttu-id="2ebf0-137">String</span><span class="sxs-lookup"><span data-stu-id="2ebf0-137">String</span></span>|<span data-ttu-id="2ebf0-138">DevicePolicyStatus のデバイス名。</span><span class="sxs-lookup"><span data-stu-id="2ebf0-138">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="2ebf0-139">userName</span><span class="sxs-lookup"><span data-stu-id="2ebf0-139">userName</span></span>|<span data-ttu-id="2ebf0-140">String</span><span class="sxs-lookup"><span data-stu-id="2ebf0-140">String</span></span>|<span data-ttu-id="2ebf0-141">レポートされているユーザー名</span><span class="sxs-lookup"><span data-stu-id="2ebf0-141">The User Name that is being reported</span></span>|
|<span data-ttu-id="2ebf0-142">deviceModel</span><span class="sxs-lookup"><span data-stu-id="2ebf0-142">deviceModel</span></span>|<span data-ttu-id="2ebf0-143">String</span><span class="sxs-lookup"><span data-stu-id="2ebf0-143">String</span></span>|<span data-ttu-id="2ebf0-144">レポートされているデバイス モデル</span><span class="sxs-lookup"><span data-stu-id="2ebf0-144">The device model that is being reported</span></span>|
|<span data-ttu-id="2ebf0-145">platform</span><span class="sxs-lookup"><span data-stu-id="2ebf0-145">platform</span></span>|<span data-ttu-id="2ebf0-146">Int32</span><span class="sxs-lookup"><span data-stu-id="2ebf0-146">Int32</span></span>|<span data-ttu-id="2ebf0-147">報告されているデバイスのプラットフォーム</span><span class="sxs-lookup"><span data-stu-id="2ebf0-147">Platform of the device that is being reported</span></span>|
|<span data-ttu-id="2ebf0-148">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="2ebf0-148">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="2ebf0-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2ebf0-149">DateTimeOffset</span></span>|<span data-ttu-id="2ebf0-150">デバイス コンプライアンスの猶予期間が過ぎる DateTime</span><span class="sxs-lookup"><span data-stu-id="2ebf0-150">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="2ebf0-151">status</span><span class="sxs-lookup"><span data-stu-id="2ebf0-151">status</span></span>|[<span data-ttu-id="2ebf0-152">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="2ebf0-152">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="2ebf0-153">ポリシー レポートのコンプライアンスの状態。</span><span class="sxs-lookup"><span data-stu-id="2ebf0-153">Compliance status of the policy report.</span></span> <span data-ttu-id="2ebf0-154">可能な値は、`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned` です。</span><span class="sxs-lookup"><span data-stu-id="2ebf0-154">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="2ebf0-155">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="2ebf0-155">lastReportedDateTime</span></span>|<span data-ttu-id="2ebf0-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2ebf0-156">DateTimeOffset</span></span>|<span data-ttu-id="2ebf0-157">ポリシー レポートの最終変更日時。</span><span class="sxs-lookup"><span data-stu-id="2ebf0-157">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="2ebf0-158">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="2ebf0-158">userPrincipalName</span></span>|<span data-ttu-id="2ebf0-159">String</span><span class="sxs-lookup"><span data-stu-id="2ebf0-159">String</span></span>|<span data-ttu-id="2ebf0-160">UserPrincipalName。</span><span class="sxs-lookup"><span data-stu-id="2ebf0-160">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="2ebf0-161">応答</span><span class="sxs-lookup"><span data-stu-id="2ebf0-161">Response</span></span>
<span data-ttu-id="2ebf0-162">かどうかは成功すると、このメソッドが返されます、`201 Created`応答コードおよび応答の本文に[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="2ebf0-162">If successful, this method returns a `201 Created` response code and a [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2ebf0-163">例</span><span class="sxs-lookup"><span data-stu-id="2ebf0-163">Example</span></span>

### <a name="request"></a><span data-ttu-id="2ebf0-164">要求</span><span class="sxs-lookup"><span data-stu-id="2ebf0-164">Request</span></span>
<span data-ttu-id="2ebf0-165">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="2ebf0-165">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatuses
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

### <a name="response"></a><span data-ttu-id="2ebf0-166">応答</span><span class="sxs-lookup"><span data-stu-id="2ebf0-166">Response</span></span>
<span data-ttu-id="2ebf0-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="2ebf0-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




