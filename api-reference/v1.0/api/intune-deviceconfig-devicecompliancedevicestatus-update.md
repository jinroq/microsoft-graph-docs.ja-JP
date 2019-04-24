---
title: deviceComplianceDeviceStatus の更新
description: deviceComplianceDeviceStatus オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 06c5b6661320d2212579e4788fc29ce7c2861660
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32460521"
---
# <a name="update-devicecompliancedevicestatus"></a><span data-ttu-id="a3ded-103">deviceComplianceDeviceStatus の更新</span><span class="sxs-lookup"><span data-stu-id="a3ded-103">Update deviceComplianceDeviceStatus</span></span>

> <span data-ttu-id="a3ded-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="a3ded-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a3ded-105">[deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="a3ded-105">Update the properties of a [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a3ded-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="a3ded-106">Prerequisites</span></span>
<span data-ttu-id="a3ded-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a3ded-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a3ded-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a3ded-109">Permission type</span></span>|<span data-ttu-id="a3ded-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="a3ded-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a3ded-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a3ded-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a3ded-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a3ded-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a3ded-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a3ded-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a3ded-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a3ded-114">Not supported.</span></span>|
|<span data-ttu-id="a3ded-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a3ded-115">Application</span></span>|<span data-ttu-id="a3ded-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a3ded-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a3ded-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a3ded-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatuses/{deviceComplianceDeviceStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="a3ded-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a3ded-118">Request headers</span></span>
|<span data-ttu-id="a3ded-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a3ded-119">Header</span></span>|<span data-ttu-id="a3ded-120">値</span><span class="sxs-lookup"><span data-stu-id="a3ded-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a3ded-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="a3ded-121">Authorization</span></span>|<span data-ttu-id="a3ded-122">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="a3ded-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a3ded-123">承諾</span><span class="sxs-lookup"><span data-stu-id="a3ded-123">Accept</span></span>|<span data-ttu-id="a3ded-124">application/json</span><span class="sxs-lookup"><span data-stu-id="a3ded-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a3ded-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="a3ded-125">Request body</span></span>
<span data-ttu-id="a3ded-126">要求本文で、[deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="a3ded-126">In the request body, supply a JSON representation for the [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) object.</span></span>

<span data-ttu-id="a3ded-127">次の表に、[deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="a3ded-127">The following table shows the properties that are required when you create the [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md).</span></span>

|<span data-ttu-id="a3ded-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a3ded-128">Property</span></span>|<span data-ttu-id="a3ded-129">型</span><span class="sxs-lookup"><span data-stu-id="a3ded-129">Type</span></span>|<span data-ttu-id="a3ded-130">説明</span><span class="sxs-lookup"><span data-stu-id="a3ded-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a3ded-131">id</span><span class="sxs-lookup"><span data-stu-id="a3ded-131">id</span></span>|<span data-ttu-id="a3ded-132">String</span><span class="sxs-lookup"><span data-stu-id="a3ded-132">String</span></span>|<span data-ttu-id="a3ded-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="a3ded-133">Key of the entity.</span></span>|
|<span data-ttu-id="a3ded-134">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="a3ded-134">deviceDisplayName</span></span>|<span data-ttu-id="a3ded-135">String</span><span class="sxs-lookup"><span data-stu-id="a3ded-135">String</span></span>|<span data-ttu-id="a3ded-136">DevicePolicyStatus のデバイス名。</span><span class="sxs-lookup"><span data-stu-id="a3ded-136">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="a3ded-137">userName</span><span class="sxs-lookup"><span data-stu-id="a3ded-137">userName</span></span>|<span data-ttu-id="a3ded-138">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="a3ded-138">String</span></span>|<span data-ttu-id="a3ded-139">レポートされているユーザー名</span><span class="sxs-lookup"><span data-stu-id="a3ded-139">The User Name that is being reported</span></span>|
|<span data-ttu-id="a3ded-140">deviceModel</span><span class="sxs-lookup"><span data-stu-id="a3ded-140">deviceModel</span></span>|<span data-ttu-id="a3ded-141">String</span><span class="sxs-lookup"><span data-stu-id="a3ded-141">String</span></span>|<span data-ttu-id="a3ded-142">レポートされているデバイス モデル</span><span class="sxs-lookup"><span data-stu-id="a3ded-142">The device model that is being reported</span></span>|
|<span data-ttu-id="a3ded-143">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="a3ded-143">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="a3ded-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a3ded-144">DateTimeOffset</span></span>|<span data-ttu-id="a3ded-145">デバイス コンプライアンスの猶予期間が過ぎる DateTime</span><span class="sxs-lookup"><span data-stu-id="a3ded-145">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="a3ded-146">status</span><span class="sxs-lookup"><span data-stu-id="a3ded-146">status</span></span>|[<span data-ttu-id="a3ded-147">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="a3ded-147">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="a3ded-148">ポリシー レポートのコンプライアンスの状態。</span><span class="sxs-lookup"><span data-stu-id="a3ded-148">Compliance status of the policy report.</span></span> <span data-ttu-id="a3ded-149">可能な値は、`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned` です。</span><span class="sxs-lookup"><span data-stu-id="a3ded-149">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="a3ded-150">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="a3ded-150">lastReportedDateTime</span></span>|<span data-ttu-id="a3ded-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a3ded-151">DateTimeOffset</span></span>|<span data-ttu-id="a3ded-152">ポリシー レポートの最終変更日時。</span><span class="sxs-lookup"><span data-stu-id="a3ded-152">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="a3ded-153">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="a3ded-153">userPrincipalName</span></span>|<span data-ttu-id="a3ded-154">String</span><span class="sxs-lookup"><span data-stu-id="a3ded-154">String</span></span>|<span data-ttu-id="a3ded-155">UserPrincipalName。</span><span class="sxs-lookup"><span data-stu-id="a3ded-155">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="a3ded-156">応答</span><span class="sxs-lookup"><span data-stu-id="a3ded-156">Response</span></span>
<span data-ttu-id="a3ded-157">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="a3ded-157">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a3ded-158">例</span><span class="sxs-lookup"><span data-stu-id="a3ded-158">Example</span></span>

### <a name="request"></a><span data-ttu-id="a3ded-159">要求</span><span class="sxs-lookup"><span data-stu-id="a3ded-159">Request</span></span>
<span data-ttu-id="a3ded-160">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="a3ded-160">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatuses/{deviceComplianceDeviceStatusId}
Content-type: application/json
Content-length: 426

{
  "@odata.type": "#microsoft.graph.deviceComplianceDeviceStatus",
  "deviceDisplayName": "Device Display Name value",
  "userName": "User Name value",
  "deviceModel": "Device Model value",
  "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="a3ded-161">応答</span><span class="sxs-lookup"><span data-stu-id="a3ded-161">Response</span></span>
<span data-ttu-id="a3ded-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="a3ded-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 475

{
  "@odata.type": "#microsoft.graph.deviceComplianceDeviceStatus",
  "id": "c6c78124-8124-c6c7-2481-c7c62481c7c6",
  "deviceDisplayName": "Device Display Name value",
  "userName": "User Name value",
  "deviceModel": "Device Model value",
  "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```



