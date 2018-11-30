---
title: deviceConfigurationUserStatus の更新
description: deviceConfigurationUserStatus オブジェクトのプロパティを更新します。
ms.openlocfilehash: c8d34042be1e5166880c0a23ab9ec7fd0126df01
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27070580"
---
# <a name="update-deviceconfigurationuserstatus"></a><span data-ttu-id="7d590-103">deviceConfigurationUserStatus の更新</span><span class="sxs-lookup"><span data-stu-id="7d590-103">Update deviceConfigurationUserStatus</span></span>

> <span data-ttu-id="7d590-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="7d590-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7d590-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7d590-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7d590-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="7d590-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7d590-107">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="7d590-107">Update the properties of a [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7d590-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="7d590-108">Prerequisites</span></span>
<span data-ttu-id="7d590-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7d590-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7d590-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7d590-111">Permission type</span></span>|<span data-ttu-id="7d590-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="7d590-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7d590-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7d590-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7d590-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7d590-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7d590-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7d590-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7d590-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7d590-116">Not supported.</span></span>|
|<span data-ttu-id="7d590-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7d590-117">Application</span></span>|<span data-ttu-id="7d590-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7d590-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7d590-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7d590-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/userStatuses/{deviceConfigurationUserStatusId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/rootCertificate/userStatuses/{deviceConfigurationUserStatusId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/userStatuses/{deviceConfigurationUserStatusId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/rootCertificate/userStatuses/{deviceConfigurationUserStatusId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/rootCertificate/userStatuses/{deviceConfigurationUserStatusId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSScepCertificateProfile/rootCertificate/userStatuses/{deviceConfigurationUserStatusId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/userStatuses/{deviceConfigurationUserStatusId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/userStatuses/{deviceConfigurationUserStatusId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/userStatuses/{deviceConfigurationUserStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="7d590-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7d590-120">Request headers</span></span>
|<span data-ttu-id="7d590-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7d590-121">Header</span></span>|<span data-ttu-id="7d590-122">値</span><span class="sxs-lookup"><span data-stu-id="7d590-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7d590-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7d590-123">Authorization</span></span>|<span data-ttu-id="7d590-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="7d590-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7d590-125">Accept</span><span class="sxs-lookup"><span data-stu-id="7d590-125">Accept</span></span>|<span data-ttu-id="7d590-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7d590-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7d590-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="7d590-127">Request body</span></span>
<span data-ttu-id="7d590-128">要求本文で、[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="7d590-128">In the request body, supply a JSON representation for the [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) object.</span></span>

<span data-ttu-id="7d590-129">次の表に、[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="7d590-129">The following table shows the properties that are required when you create the [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md).</span></span>

|<span data-ttu-id="7d590-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7d590-130">Property</span></span>|<span data-ttu-id="7d590-131">型</span><span class="sxs-lookup"><span data-stu-id="7d590-131">Type</span></span>|<span data-ttu-id="7d590-132">説明</span><span class="sxs-lookup"><span data-stu-id="7d590-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7d590-133">id</span><span class="sxs-lookup"><span data-stu-id="7d590-133">id</span></span>|<span data-ttu-id="7d590-134">String</span><span class="sxs-lookup"><span data-stu-id="7d590-134">String</span></span>|<span data-ttu-id="7d590-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="7d590-135">Key of the entity.</span></span>|
|<span data-ttu-id="7d590-136">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="7d590-136">userDisplayName</span></span>|<span data-ttu-id="7d590-137">String</span><span class="sxs-lookup"><span data-stu-id="7d590-137">String</span></span>|<span data-ttu-id="7d590-138">DevicePolicyStatus のユーザー名。</span><span class="sxs-lookup"><span data-stu-id="7d590-138">User name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="7d590-139">devicesCount</span><span class="sxs-lookup"><span data-stu-id="7d590-139">devicesCount</span></span>|<span data-ttu-id="7d590-140">Int32</span><span class="sxs-lookup"><span data-stu-id="7d590-140">Int32</span></span>|<span data-ttu-id="7d590-141">そのユーザーのデバイスの数。</span><span class="sxs-lookup"><span data-stu-id="7d590-141">Devices count for that user.</span></span>|
|<span data-ttu-id="7d590-142">status</span><span class="sxs-lookup"><span data-stu-id="7d590-142">status</span></span>|[<span data-ttu-id="7d590-143">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="7d590-143">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="7d590-144">ポリシー レポートのコンプライアンスの状態。</span><span class="sxs-lookup"><span data-stu-id="7d590-144">Compliance status of the policy report.</span></span> <span data-ttu-id="7d590-145">可能な値は、`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned` です。</span><span class="sxs-lookup"><span data-stu-id="7d590-145">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="7d590-146">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="7d590-146">lastReportedDateTime</span></span>|<span data-ttu-id="7d590-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7d590-147">DateTimeOffset</span></span>|<span data-ttu-id="7d590-148">ポリシー レポートの最終変更日時。</span><span class="sxs-lookup"><span data-stu-id="7d590-148">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="7d590-149">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="7d590-149">userPrincipalName</span></span>|<span data-ttu-id="7d590-150">String</span><span class="sxs-lookup"><span data-stu-id="7d590-150">String</span></span>|<span data-ttu-id="7d590-151">UserPrincipalName。</span><span class="sxs-lookup"><span data-stu-id="7d590-151">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="7d590-152">応答</span><span class="sxs-lookup"><span data-stu-id="7d590-152">Response</span></span>
<span data-ttu-id="7d590-153">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="7d590-153">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7d590-154">例</span><span class="sxs-lookup"><span data-stu-id="7d590-154">Example</span></span>
### <a name="request"></a><span data-ttu-id="7d590-155">要求</span><span class="sxs-lookup"><span data-stu-id="7d590-155">Request</span></span>
<span data-ttu-id="7d590-156">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="7d590-156">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/userStatuses/{deviceConfigurationUserStatusId}
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

### <a name="response"></a><span data-ttu-id="7d590-157">応答</span><span class="sxs-lookup"><span data-stu-id="7d590-157">Response</span></span>
<span data-ttu-id="7d590-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="7d590-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 339

{
  "@odata.type": "#microsoft.graph.deviceConfigurationUserStatus",
  "id": "7e323db2-3db2-7e32-b23d-327eb23d327e",
  "userDisplayName": "User Display Name value",
  "devicesCount": 12,
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```





