---
title: deviceComplianceDeviceStatus の作成
description: 新しい deviceComplianceDeviceStatus オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b33cb80c584df64eb7130d24c706b5bb0c16b413
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35997758"
---
# <a name="create-devicecompliancedevicestatus"></a><span data-ttu-id="23729-103">deviceComplianceDeviceStatus の作成</span><span class="sxs-lookup"><span data-stu-id="23729-103">Create deviceComplianceDeviceStatus</span></span>

> <span data-ttu-id="23729-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="23729-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="23729-105">新しい [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="23729-105">Create a new [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="23729-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="23729-106">Prerequisites</span></span>
<span data-ttu-id="23729-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="23729-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="23729-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="23729-109">Permission type</span></span>|<span data-ttu-id="23729-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="23729-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="23729-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="23729-111">Delegated (work or school account)</span></span>|<span data-ttu-id="23729-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="23729-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="23729-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="23729-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="23729-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="23729-114">Not supported.</span></span>|
|<span data-ttu-id="23729-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="23729-115">Application</span></span>|<span data-ttu-id="23729-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="23729-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="23729-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="23729-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatuses
```

## <a name="request-headers"></a><span data-ttu-id="23729-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="23729-118">Request headers</span></span>
|<span data-ttu-id="23729-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="23729-119">Header</span></span>|<span data-ttu-id="23729-120">値</span><span class="sxs-lookup"><span data-stu-id="23729-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="23729-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="23729-121">Authorization</span></span>|<span data-ttu-id="23729-122">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="23729-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="23729-123">承諾</span><span class="sxs-lookup"><span data-stu-id="23729-123">Accept</span></span>|<span data-ttu-id="23729-124">application/json</span><span class="sxs-lookup"><span data-stu-id="23729-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="23729-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="23729-125">Request body</span></span>
<span data-ttu-id="23729-126">要求本文で、deviceComplianceDeviceStatus オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="23729-126">In the request body, supply a JSON representation for the deviceComplianceDeviceStatus object.</span></span>

<span data-ttu-id="23729-127">次の表に、deviceComplianceDeviceStatus の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="23729-127">The following table shows the properties that are required when you create the deviceComplianceDeviceStatus.</span></span>

|<span data-ttu-id="23729-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="23729-128">Property</span></span>|<span data-ttu-id="23729-129">型</span><span class="sxs-lookup"><span data-stu-id="23729-129">Type</span></span>|<span data-ttu-id="23729-130">説明</span><span class="sxs-lookup"><span data-stu-id="23729-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="23729-131">id</span><span class="sxs-lookup"><span data-stu-id="23729-131">id</span></span>|<span data-ttu-id="23729-132">文字列</span><span class="sxs-lookup"><span data-stu-id="23729-132">String</span></span>|<span data-ttu-id="23729-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="23729-133">Key of the entity.</span></span>|
|<span data-ttu-id="23729-134">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="23729-134">deviceDisplayName</span></span>|<span data-ttu-id="23729-135">String</span><span class="sxs-lookup"><span data-stu-id="23729-135">String</span></span>|<span data-ttu-id="23729-136">DevicePolicyStatus のデバイス名。</span><span class="sxs-lookup"><span data-stu-id="23729-136">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="23729-137">userName</span><span class="sxs-lookup"><span data-stu-id="23729-137">userName</span></span>|<span data-ttu-id="23729-138">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="23729-138">String</span></span>|<span data-ttu-id="23729-139">レポートされているユーザー名</span><span class="sxs-lookup"><span data-stu-id="23729-139">The User Name that is being reported</span></span>|
|<span data-ttu-id="23729-140">deviceModel</span><span class="sxs-lookup"><span data-stu-id="23729-140">deviceModel</span></span>|<span data-ttu-id="23729-141">String</span><span class="sxs-lookup"><span data-stu-id="23729-141">String</span></span>|<span data-ttu-id="23729-142">レポートされているデバイス モデル</span><span class="sxs-lookup"><span data-stu-id="23729-142">The device model that is being reported</span></span>|
|<span data-ttu-id="23729-143">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="23729-143">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="23729-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="23729-144">DateTimeOffset</span></span>|<span data-ttu-id="23729-145">デバイス コンプライアンスの猶予期間が過ぎる DateTime</span><span class="sxs-lookup"><span data-stu-id="23729-145">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="23729-146">status</span><span class="sxs-lookup"><span data-stu-id="23729-146">status</span></span>|[<span data-ttu-id="23729-147">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="23729-147">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="23729-148">ポリシー レポートのコンプライアンスの状態。</span><span class="sxs-lookup"><span data-stu-id="23729-148">Compliance status of the policy report.</span></span> <span data-ttu-id="23729-149">可能な値は、`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned` です。</span><span class="sxs-lookup"><span data-stu-id="23729-149">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="23729-150">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="23729-150">lastReportedDateTime</span></span>|<span data-ttu-id="23729-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="23729-151">DateTimeOffset</span></span>|<span data-ttu-id="23729-152">ポリシー レポートの最終変更日時。</span><span class="sxs-lookup"><span data-stu-id="23729-152">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="23729-153">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="23729-153">userPrincipalName</span></span>|<span data-ttu-id="23729-154">String</span><span class="sxs-lookup"><span data-stu-id="23729-154">String</span></span>|<span data-ttu-id="23729-155">UserPrincipalName。</span><span class="sxs-lookup"><span data-stu-id="23729-155">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="23729-156">応答</span><span class="sxs-lookup"><span data-stu-id="23729-156">Response</span></span>
<span data-ttu-id="23729-157">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="23729-157">If successful, this method returns a `201 Created` response code and a [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="23729-158">例</span><span class="sxs-lookup"><span data-stu-id="23729-158">Example</span></span>

### <a name="request"></a><span data-ttu-id="23729-159">要求</span><span class="sxs-lookup"><span data-stu-id="23729-159">Request</span></span>
<span data-ttu-id="23729-160">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="23729-160">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatuses
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

### <a name="response"></a><span data-ttu-id="23729-161">応答</span><span class="sxs-lookup"><span data-stu-id="23729-161">Response</span></span>
<span data-ttu-id="23729-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="23729-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



