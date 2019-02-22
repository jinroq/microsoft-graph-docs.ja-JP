---
title: managedDeviceMobileAppConfigurationUserStatus の更新
description: managedDeviceMobileAppConfigurationUserStatus オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 41eb2658d5bc20728a34587b258581a7a7693ea9
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30156869"
---
# <a name="update-manageddevicemobileappconfigurationuserstatus"></a><span data-ttu-id="abd07-103">managedDeviceMobileAppConfigurationUserStatus の更新</span><span class="sxs-lookup"><span data-stu-id="abd07-103">Update managedDeviceMobileAppConfigurationUserStatus</span></span>

> <span data-ttu-id="abd07-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="abd07-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="abd07-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="abd07-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="abd07-106">[managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="abd07-106">Update the properties of a [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="abd07-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="abd07-107">Prerequisites</span></span>
<span data-ttu-id="abd07-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="abd07-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="abd07-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="abd07-110">Permission type</span></span>|<span data-ttu-id="abd07-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="abd07-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="abd07-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="abd07-112">Delegated (work or school account)</span></span>|<span data-ttu-id="abd07-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="abd07-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="abd07-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="abd07-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="abd07-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="abd07-115">Not supported.</span></span>|
|<span data-ttu-id="abd07-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="abd07-116">Application</span></span>|<span data-ttu-id="abd07-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="abd07-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="abd07-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="abd07-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/userStatuses/{managedDeviceMobileAppConfigurationUserStatusId}
PATCH /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/userStatuses/{managedDeviceMobileAppConfigurationUserStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="abd07-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="abd07-119">Request headers</span></span>
|<span data-ttu-id="abd07-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="abd07-120">Header</span></span>|<span data-ttu-id="abd07-121">値</span><span class="sxs-lookup"><span data-stu-id="abd07-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="abd07-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="abd07-122">Authorization</span></span>|<span data-ttu-id="abd07-123">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="abd07-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="abd07-124">承諾</span><span class="sxs-lookup"><span data-stu-id="abd07-124">Accept</span></span>|<span data-ttu-id="abd07-125">application/json</span><span class="sxs-lookup"><span data-stu-id="abd07-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="abd07-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="abd07-126">Request body</span></span>
<span data-ttu-id="abd07-127">要求本文で、[managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="abd07-127">In the request body, supply a JSON representation for the [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) object.</span></span>

<span data-ttu-id="abd07-128">次の表に、[managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="abd07-128">The following table shows the properties that are required when you create the [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md).</span></span>

|<span data-ttu-id="abd07-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="abd07-129">Property</span></span>|<span data-ttu-id="abd07-130">型</span><span class="sxs-lookup"><span data-stu-id="abd07-130">Type</span></span>|<span data-ttu-id="abd07-131">説明</span><span class="sxs-lookup"><span data-stu-id="abd07-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="abd07-132">id</span><span class="sxs-lookup"><span data-stu-id="abd07-132">id</span></span>|<span data-ttu-id="abd07-133">String</span><span class="sxs-lookup"><span data-stu-id="abd07-133">String</span></span>|<span data-ttu-id="abd07-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="abd07-134">Key of the entity.</span></span>|
|<span data-ttu-id="abd07-135">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="abd07-135">userDisplayName</span></span>|<span data-ttu-id="abd07-136">String</span><span class="sxs-lookup"><span data-stu-id="abd07-136">String</span></span>|<span data-ttu-id="abd07-137">DevicePolicyStatus のユーザー名。</span><span class="sxs-lookup"><span data-stu-id="abd07-137">User name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="abd07-138">devicesCount</span><span class="sxs-lookup"><span data-stu-id="abd07-138">devicesCount</span></span>|<span data-ttu-id="abd07-139">Int32</span><span class="sxs-lookup"><span data-stu-id="abd07-139">Int32</span></span>|<span data-ttu-id="abd07-140">そのユーザーのデバイスの数。</span><span class="sxs-lookup"><span data-stu-id="abd07-140">Devices count for that user.</span></span>|
|<span data-ttu-id="abd07-141">status</span><span class="sxs-lookup"><span data-stu-id="abd07-141">status</span></span>|[<span data-ttu-id="abd07-142">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="abd07-142">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="abd07-143">ポリシー レポートのコンプライアンスの状態。</span><span class="sxs-lookup"><span data-stu-id="abd07-143">Compliance status of the policy report.</span></span> <span data-ttu-id="abd07-144">可能な値は、`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned` です。</span><span class="sxs-lookup"><span data-stu-id="abd07-144">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="abd07-145">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="abd07-145">lastReportedDateTime</span></span>|<span data-ttu-id="abd07-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="abd07-146">DateTimeOffset</span></span>|<span data-ttu-id="abd07-147">ポリシー レポートの最終変更日時。</span><span class="sxs-lookup"><span data-stu-id="abd07-147">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="abd07-148">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="abd07-148">userPrincipalName</span></span>|<span data-ttu-id="abd07-149">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="abd07-149">String</span></span>|<span data-ttu-id="abd07-150">UserPrincipalName。</span><span class="sxs-lookup"><span data-stu-id="abd07-150">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="abd07-151">応答</span><span class="sxs-lookup"><span data-stu-id="abd07-151">Response</span></span>
<span data-ttu-id="abd07-152">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="abd07-152">If successful, this method returns a `200 OK` response code and an updated [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="abd07-153">例</span><span class="sxs-lookup"><span data-stu-id="abd07-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="abd07-154">要求</span><span class="sxs-lookup"><span data-stu-id="abd07-154">Request</span></span>
<span data-ttu-id="abd07-155">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="abd07-155">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/userStatuses/{managedDeviceMobileAppConfigurationUserStatusId}
Content-type: application/json
Content-length: 306

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationUserStatus",
  "userDisplayName": "User Display Name value",
  "devicesCount": 12,
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="abd07-156">応答</span><span class="sxs-lookup"><span data-stu-id="abd07-156">Response</span></span>
<span data-ttu-id="abd07-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="abd07-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 355

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationUserStatus",
  "id": "44960944-0944-4496-4409-964444099644",
  "userDisplayName": "User Display Name value",
  "devicesCount": 12,
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```




