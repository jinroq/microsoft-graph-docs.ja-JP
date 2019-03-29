---
title: deviceComplianceDeviceStatus の作成
description: 新しい deviceComplianceDeviceStatus オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a3f88b97de4d14405b53a4ee36bd22168c4e2798
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/29/2019
ms.locfileid: "30971379"
---
# <a name="create-devicecompliancedevicestatus"></a><span data-ttu-id="ee8df-103">deviceComplianceDeviceStatus の作成</span><span class="sxs-lookup"><span data-stu-id="ee8df-103">Create deviceComplianceDeviceStatus</span></span>

> <span data-ttu-id="ee8df-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ee8df-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ee8df-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="ee8df-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ee8df-106">新しい [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="ee8df-106">Create a new [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ee8df-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="ee8df-107">Prerequisites</span></span>
<span data-ttu-id="ee8df-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ee8df-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ee8df-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ee8df-110">Permission type</span></span>|<span data-ttu-id="ee8df-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="ee8df-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ee8df-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ee8df-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ee8df-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ee8df-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ee8df-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ee8df-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ee8df-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ee8df-115">Not supported.</span></span>|
|<span data-ttu-id="ee8df-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ee8df-116">Application</span></span>|<span data-ttu-id="ee8df-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ee8df-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ee8df-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ee8df-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatuses
```

## <a name="request-headers"></a><span data-ttu-id="ee8df-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ee8df-119">Request headers</span></span>
|<span data-ttu-id="ee8df-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ee8df-120">Header</span></span>|<span data-ttu-id="ee8df-121">値</span><span class="sxs-lookup"><span data-stu-id="ee8df-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ee8df-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ee8df-122">Authorization</span></span>|<span data-ttu-id="ee8df-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="ee8df-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ee8df-124">承諾</span><span class="sxs-lookup"><span data-stu-id="ee8df-124">Accept</span></span>|<span data-ttu-id="ee8df-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ee8df-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ee8df-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="ee8df-126">Request body</span></span>
<span data-ttu-id="ee8df-127">要求本文で、deviceComplianceDeviceStatus オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="ee8df-127">In the request body, supply a JSON representation for the deviceComplianceDeviceStatus object.</span></span>

<span data-ttu-id="ee8df-128">次の表に、deviceComplianceDeviceStatus の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="ee8df-128">The following table shows the properties that are required when you create the deviceComplianceDeviceStatus.</span></span>

|<span data-ttu-id="ee8df-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ee8df-129">Property</span></span>|<span data-ttu-id="ee8df-130">型</span><span class="sxs-lookup"><span data-stu-id="ee8df-130">Type</span></span>|<span data-ttu-id="ee8df-131">説明</span><span class="sxs-lookup"><span data-stu-id="ee8df-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ee8df-132">id</span><span class="sxs-lookup"><span data-stu-id="ee8df-132">id</span></span>|<span data-ttu-id="ee8df-133">String</span><span class="sxs-lookup"><span data-stu-id="ee8df-133">String</span></span>|<span data-ttu-id="ee8df-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="ee8df-134">Key of the entity.</span></span>|
|<span data-ttu-id="ee8df-135">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="ee8df-135">deviceDisplayName</span></span>|<span data-ttu-id="ee8df-136">String</span><span class="sxs-lookup"><span data-stu-id="ee8df-136">String</span></span>|<span data-ttu-id="ee8df-137">DevicePolicyStatus のデバイス名。</span><span class="sxs-lookup"><span data-stu-id="ee8df-137">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="ee8df-138">userName</span><span class="sxs-lookup"><span data-stu-id="ee8df-138">userName</span></span>|<span data-ttu-id="ee8df-139">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="ee8df-139">String</span></span>|<span data-ttu-id="ee8df-140">レポートされているユーザー名</span><span class="sxs-lookup"><span data-stu-id="ee8df-140">The User Name that is being reported</span></span>|
|<span data-ttu-id="ee8df-141">deviceModel</span><span class="sxs-lookup"><span data-stu-id="ee8df-141">deviceModel</span></span>|<span data-ttu-id="ee8df-142">String</span><span class="sxs-lookup"><span data-stu-id="ee8df-142">String</span></span>|<span data-ttu-id="ee8df-143">レポートされているデバイス モデル</span><span class="sxs-lookup"><span data-stu-id="ee8df-143">The device model that is being reported</span></span>|
|<span data-ttu-id="ee8df-144">platform</span><span class="sxs-lookup"><span data-stu-id="ee8df-144">platform</span></span>|<span data-ttu-id="ee8df-145">Int32</span><span class="sxs-lookup"><span data-stu-id="ee8df-145">Int32</span></span>|<span data-ttu-id="ee8df-146">レポートされているデバイスのプラットフォーム</span><span class="sxs-lookup"><span data-stu-id="ee8df-146">Platform of the device that is being reported</span></span>|
|<span data-ttu-id="ee8df-147">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="ee8df-147">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="ee8df-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ee8df-148">DateTimeOffset</span></span>|<span data-ttu-id="ee8df-149">デバイス コンプライアンスの猶予期間が過ぎる DateTime</span><span class="sxs-lookup"><span data-stu-id="ee8df-149">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="ee8df-150">status</span><span class="sxs-lookup"><span data-stu-id="ee8df-150">status</span></span>|[<span data-ttu-id="ee8df-151">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="ee8df-151">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="ee8df-152">ポリシー レポートのコンプライアンスの状態。</span><span class="sxs-lookup"><span data-stu-id="ee8df-152">Compliance status of the policy report.</span></span> <span data-ttu-id="ee8df-153">可能な値は、`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned` です。</span><span class="sxs-lookup"><span data-stu-id="ee8df-153">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="ee8df-154">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="ee8df-154">lastReportedDateTime</span></span>|<span data-ttu-id="ee8df-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ee8df-155">DateTimeOffset</span></span>|<span data-ttu-id="ee8df-156">ポリシー レポートの最終変更日時。</span><span class="sxs-lookup"><span data-stu-id="ee8df-156">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="ee8df-157">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="ee8df-157">userPrincipalName</span></span>|<span data-ttu-id="ee8df-158">String</span><span class="sxs-lookup"><span data-stu-id="ee8df-158">String</span></span>|<span data-ttu-id="ee8df-159">UserPrincipalName。</span><span class="sxs-lookup"><span data-stu-id="ee8df-159">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="ee8df-160">応答</span><span class="sxs-lookup"><span data-stu-id="ee8df-160">Response</span></span>
<span data-ttu-id="ee8df-161">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="ee8df-161">If successful, this method returns a `201 Created` response code and a [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ee8df-162">例</span><span class="sxs-lookup"><span data-stu-id="ee8df-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="ee8df-163">要求</span><span class="sxs-lookup"><span data-stu-id="ee8df-163">Request</span></span>
<span data-ttu-id="ee8df-164">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ee8df-164">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatuses
Content-type: application/json
Content-length: 444

{
  "@odata.type": "#microsoft.graph.deviceComplianceDeviceStatus",
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

### <a name="response"></a><span data-ttu-id="ee8df-165">応答</span><span class="sxs-lookup"><span data-stu-id="ee8df-165">Response</span></span>
<span data-ttu-id="ee8df-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="ee8df-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 493

{
  "@odata.type": "#microsoft.graph.deviceComplianceDeviceStatus",
  "id": "c6c78124-8124-c6c7-2481-c7c62481c7c6",
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




