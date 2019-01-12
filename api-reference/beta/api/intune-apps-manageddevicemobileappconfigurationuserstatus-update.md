---
title: managedDeviceMobileAppConfigurationUserStatus の更新
description: managedDeviceMobileAppConfigurationUserStatus オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 47c6f6831702cf0b86b0b34574392f18ea1bbe50
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27930223"
---
# <a name="update-manageddevicemobileappconfigurationuserstatus"></a><span data-ttu-id="ffd38-103">managedDeviceMobileAppConfigurationUserStatus の更新</span><span class="sxs-lookup"><span data-stu-id="ffd38-103">Update managedDeviceMobileAppConfigurationUserStatus</span></span>

> <span data-ttu-id="ffd38-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="ffd38-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ffd38-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ffd38-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ffd38-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="ffd38-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ffd38-107">[managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="ffd38-107">Update the properties of a [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ffd38-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="ffd38-108">Prerequisites</span></span>
<span data-ttu-id="ffd38-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ffd38-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ffd38-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ffd38-111">Permission type</span></span>|<span data-ttu-id="ffd38-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="ffd38-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ffd38-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ffd38-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ffd38-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ffd38-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="ffd38-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ffd38-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ffd38-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ffd38-116">Not supported.</span></span>|
|<span data-ttu-id="ffd38-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ffd38-117">Application</span></span>|<span data-ttu-id="ffd38-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ffd38-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ffd38-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ffd38-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/userStatuses/{managedDeviceMobileAppConfigurationUserStatusId}
PATCH /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/userStatuses/{managedDeviceMobileAppConfigurationUserStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="ffd38-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ffd38-120">Request headers</span></span>
|<span data-ttu-id="ffd38-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ffd38-121">Header</span></span>|<span data-ttu-id="ffd38-122">値</span><span class="sxs-lookup"><span data-stu-id="ffd38-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ffd38-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ffd38-123">Authorization</span></span>|<span data-ttu-id="ffd38-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="ffd38-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ffd38-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ffd38-125">Accept</span></span>|<span data-ttu-id="ffd38-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ffd38-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ffd38-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="ffd38-127">Request body</span></span>
<span data-ttu-id="ffd38-128">要求本文で、[managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="ffd38-128">In the request body, supply a JSON representation for the [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) object.</span></span>

<span data-ttu-id="ffd38-129">次の表に、[managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="ffd38-129">The following table shows the properties that are required when you create the [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md).</span></span>

|<span data-ttu-id="ffd38-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ffd38-130">Property</span></span>|<span data-ttu-id="ffd38-131">型</span><span class="sxs-lookup"><span data-stu-id="ffd38-131">Type</span></span>|<span data-ttu-id="ffd38-132">説明</span><span class="sxs-lookup"><span data-stu-id="ffd38-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ffd38-133">ID</span><span class="sxs-lookup"><span data-stu-id="ffd38-133">id</span></span>|<span data-ttu-id="ffd38-134">String</span><span class="sxs-lookup"><span data-stu-id="ffd38-134">String</span></span>|<span data-ttu-id="ffd38-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="ffd38-135">Key of the entity.</span></span>|
|<span data-ttu-id="ffd38-136">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="ffd38-136">userDisplayName</span></span>|<span data-ttu-id="ffd38-137">String</span><span class="sxs-lookup"><span data-stu-id="ffd38-137">String</span></span>|<span data-ttu-id="ffd38-138">DevicePolicyStatus のユーザー名。</span><span class="sxs-lookup"><span data-stu-id="ffd38-138">User name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="ffd38-139">devicesCount</span><span class="sxs-lookup"><span data-stu-id="ffd38-139">devicesCount</span></span>|<span data-ttu-id="ffd38-140">Int32</span><span class="sxs-lookup"><span data-stu-id="ffd38-140">Int32</span></span>|<span data-ttu-id="ffd38-141">そのユーザーのデバイスの数。</span><span class="sxs-lookup"><span data-stu-id="ffd38-141">Devices count for that user.</span></span>|
|<span data-ttu-id="ffd38-142">status</span><span class="sxs-lookup"><span data-stu-id="ffd38-142">status</span></span>|[<span data-ttu-id="ffd38-143">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="ffd38-143">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="ffd38-144">ポリシー レポートのコンプライアンスの状態。</span><span class="sxs-lookup"><span data-stu-id="ffd38-144">Compliance status of the policy report.</span></span> <span data-ttu-id="ffd38-145">可能な値は、`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned` です。</span><span class="sxs-lookup"><span data-stu-id="ffd38-145">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="ffd38-146">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="ffd38-146">lastReportedDateTime</span></span>|<span data-ttu-id="ffd38-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ffd38-147">DateTimeOffset</span></span>|<span data-ttu-id="ffd38-148">ポリシー レポートの最終変更日時。</span><span class="sxs-lookup"><span data-stu-id="ffd38-148">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="ffd38-149">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="ffd38-149">userPrincipalName</span></span>|<span data-ttu-id="ffd38-150">String</span><span class="sxs-lookup"><span data-stu-id="ffd38-150">String</span></span>|<span data-ttu-id="ffd38-151">UserPrincipalName。</span><span class="sxs-lookup"><span data-stu-id="ffd38-151">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="ffd38-152">応答</span><span class="sxs-lookup"><span data-stu-id="ffd38-152">Response</span></span>
<span data-ttu-id="ffd38-153">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="ffd38-153">If successful, this method returns a `200 OK` response code and an updated [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ffd38-154">例</span><span class="sxs-lookup"><span data-stu-id="ffd38-154">Example</span></span>
### <a name="request"></a><span data-ttu-id="ffd38-155">要求</span><span class="sxs-lookup"><span data-stu-id="ffd38-155">Request</span></span>
<span data-ttu-id="ffd38-156">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ffd38-156">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/userStatuses/{managedDeviceMobileAppConfigurationUserStatusId}
Content-type: application/json
Content-length: 222

{
  "userDisplayName": "User Display Name value",
  "devicesCount": 12,
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="ffd38-157">応答</span><span class="sxs-lookup"><span data-stu-id="ffd38-157">Response</span></span>
<span data-ttu-id="ffd38-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="ffd38-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





