---
title: deviceConfigurationUserStatus の更新
description: deviceConfigurationUserStatus オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 120f7ff6a50318e938fcf2a8e2d0664d72d4151f
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31798622"
---
# <a name="update-deviceconfigurationuserstatus"></a><span data-ttu-id="4937b-103">deviceConfigurationUserStatus の更新</span><span class="sxs-lookup"><span data-stu-id="4937b-103">Update deviceConfigurationUserStatus</span></span>

> <span data-ttu-id="4937b-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4937b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4937b-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="4937b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4937b-106">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="4937b-106">Update the properties of a [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4937b-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="4937b-107">Prerequisites</span></span>
<span data-ttu-id="4937b-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4937b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4937b-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="4937b-110">Permission type</span></span>|<span data-ttu-id="4937b-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="4937b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4937b-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="4937b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4937b-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4937b-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4937b-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="4937b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4937b-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4937b-115">Not supported.</span></span>|
|<span data-ttu-id="4937b-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="4937b-116">Application</span></span>|<span data-ttu-id="4937b-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4937b-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4937b-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="4937b-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="4937b-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4937b-119">Request headers</span></span>
|<span data-ttu-id="4937b-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4937b-120">Header</span></span>|<span data-ttu-id="4937b-121">値</span><span class="sxs-lookup"><span data-stu-id="4937b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4937b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="4937b-122">Authorization</span></span>|<span data-ttu-id="4937b-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="4937b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4937b-124">承諾</span><span class="sxs-lookup"><span data-stu-id="4937b-124">Accept</span></span>|<span data-ttu-id="4937b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4937b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4937b-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="4937b-126">Request body</span></span>
<span data-ttu-id="4937b-127">要求本文で、[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="4937b-127">In the request body, supply a JSON representation for the [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) object.</span></span>

<span data-ttu-id="4937b-128">次の表に、[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="4937b-128">The following table shows the properties that are required when you create the [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md).</span></span>

|<span data-ttu-id="4937b-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4937b-129">Property</span></span>|<span data-ttu-id="4937b-130">型</span><span class="sxs-lookup"><span data-stu-id="4937b-130">Type</span></span>|<span data-ttu-id="4937b-131">説明</span><span class="sxs-lookup"><span data-stu-id="4937b-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4937b-132">id</span><span class="sxs-lookup"><span data-stu-id="4937b-132">id</span></span>|<span data-ttu-id="4937b-133">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="4937b-133">String</span></span>|<span data-ttu-id="4937b-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="4937b-134">Key of the entity.</span></span>|
|<span data-ttu-id="4937b-135">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="4937b-135">userDisplayName</span></span>|<span data-ttu-id="4937b-136">String</span><span class="sxs-lookup"><span data-stu-id="4937b-136">String</span></span>|<span data-ttu-id="4937b-137">DevicePolicyStatus のユーザー名。</span><span class="sxs-lookup"><span data-stu-id="4937b-137">User name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="4937b-138">devicesCount</span><span class="sxs-lookup"><span data-stu-id="4937b-138">devicesCount</span></span>|<span data-ttu-id="4937b-139">Int32</span><span class="sxs-lookup"><span data-stu-id="4937b-139">Int32</span></span>|<span data-ttu-id="4937b-140">そのユーザーのデバイスの数。</span><span class="sxs-lookup"><span data-stu-id="4937b-140">Devices count for that user.</span></span>|
|<span data-ttu-id="4937b-141">status</span><span class="sxs-lookup"><span data-stu-id="4937b-141">status</span></span>|[<span data-ttu-id="4937b-142">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="4937b-142">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="4937b-143">ポリシー レポートのコンプライアンスの状態。</span><span class="sxs-lookup"><span data-stu-id="4937b-143">Compliance status of the policy report.</span></span> <span data-ttu-id="4937b-144">可能な値は、`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned` です。</span><span class="sxs-lookup"><span data-stu-id="4937b-144">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="4937b-145">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="4937b-145">lastReportedDateTime</span></span>|<span data-ttu-id="4937b-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4937b-146">DateTimeOffset</span></span>|<span data-ttu-id="4937b-147">ポリシー レポートの最終変更日時。</span><span class="sxs-lookup"><span data-stu-id="4937b-147">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="4937b-148">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="4937b-148">userPrincipalName</span></span>|<span data-ttu-id="4937b-149">String</span><span class="sxs-lookup"><span data-stu-id="4937b-149">String</span></span>|<span data-ttu-id="4937b-150">UserPrincipalName。</span><span class="sxs-lookup"><span data-stu-id="4937b-150">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="4937b-151">応答</span><span class="sxs-lookup"><span data-stu-id="4937b-151">Response</span></span>
<span data-ttu-id="4937b-152">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="4937b-152">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4937b-153">例</span><span class="sxs-lookup"><span data-stu-id="4937b-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="4937b-154">要求</span><span class="sxs-lookup"><span data-stu-id="4937b-154">Request</span></span>
<span data-ttu-id="4937b-155">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="4937b-155">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/userStatuses/{deviceConfigurationUserStatusId}
Content-type: application/json
Content-length: 290

{
  "@odata.type": "#microsoft.graph.deviceConfigurationUserStatus",
  "userDisplayName": "User Display Name value",
  "devicesCount": 12,
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="4937b-156">応答</span><span class="sxs-lookup"><span data-stu-id="4937b-156">Response</span></span>
<span data-ttu-id="4937b-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="4937b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





