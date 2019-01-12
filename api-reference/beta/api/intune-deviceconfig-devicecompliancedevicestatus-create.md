---
title: deviceComplianceDeviceStatus の作成
description: 新しい deviceComplianceDeviceStatus オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 2ad91ad1e7ccd75821ae64440e88344f7f8b9c3d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27948339"
---
# <a name="create-devicecompliancedevicestatus"></a><span data-ttu-id="54dce-103">deviceComplianceDeviceStatus の作成</span><span class="sxs-lookup"><span data-stu-id="54dce-103">Create deviceComplianceDeviceStatus</span></span>

> <span data-ttu-id="54dce-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="54dce-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="54dce-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="54dce-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="54dce-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="54dce-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="54dce-107">新しい [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="54dce-107">Create a new [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="54dce-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="54dce-108">Prerequisites</span></span>
<span data-ttu-id="54dce-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="54dce-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="54dce-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="54dce-111">Permission type</span></span>|<span data-ttu-id="54dce-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="54dce-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="54dce-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="54dce-113">Delegated (work or school account)</span></span>|<span data-ttu-id="54dce-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="54dce-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="54dce-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="54dce-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="54dce-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="54dce-116">Not supported.</span></span>|
|<span data-ttu-id="54dce-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="54dce-117">Application</span></span>|<span data-ttu-id="54dce-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="54dce-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="54dce-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="54dce-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatuses
```

## <a name="request-headers"></a><span data-ttu-id="54dce-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="54dce-120">Request headers</span></span>
|<span data-ttu-id="54dce-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="54dce-121">Header</span></span>|<span data-ttu-id="54dce-122">値</span><span class="sxs-lookup"><span data-stu-id="54dce-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="54dce-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="54dce-123">Authorization</span></span>|<span data-ttu-id="54dce-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="54dce-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="54dce-125">Accept</span><span class="sxs-lookup"><span data-stu-id="54dce-125">Accept</span></span>|<span data-ttu-id="54dce-126">application/json</span><span class="sxs-lookup"><span data-stu-id="54dce-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="54dce-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="54dce-127">Request body</span></span>
<span data-ttu-id="54dce-128">要求本文で、deviceComplianceDeviceStatus オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="54dce-128">In the request body, supply a JSON representation for the deviceComplianceDeviceStatus object.</span></span>

<span data-ttu-id="54dce-129">次の表に、deviceComplianceDeviceStatus の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="54dce-129">The following table shows the properties that are required when you create the deviceComplianceDeviceStatus.</span></span>

|<span data-ttu-id="54dce-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="54dce-130">Property</span></span>|<span data-ttu-id="54dce-131">種類</span><span class="sxs-lookup"><span data-stu-id="54dce-131">Type</span></span>|<span data-ttu-id="54dce-132">説明</span><span class="sxs-lookup"><span data-stu-id="54dce-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="54dce-133">ID</span><span class="sxs-lookup"><span data-stu-id="54dce-133">id</span></span>|<span data-ttu-id="54dce-134">String</span><span class="sxs-lookup"><span data-stu-id="54dce-134">String</span></span>|<span data-ttu-id="54dce-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="54dce-135">Key of the entity.</span></span>|
|<span data-ttu-id="54dce-136">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="54dce-136">deviceDisplayName</span></span>|<span data-ttu-id="54dce-137">String</span><span class="sxs-lookup"><span data-stu-id="54dce-137">String</span></span>|<span data-ttu-id="54dce-138">DevicePolicyStatus のデバイス名。</span><span class="sxs-lookup"><span data-stu-id="54dce-138">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="54dce-139">userName</span><span class="sxs-lookup"><span data-stu-id="54dce-139">userName</span></span>|<span data-ttu-id="54dce-140">String</span><span class="sxs-lookup"><span data-stu-id="54dce-140">String</span></span>|<span data-ttu-id="54dce-141">レポートされているユーザー名</span><span class="sxs-lookup"><span data-stu-id="54dce-141">The User Name that is being reported</span></span>|
|<span data-ttu-id="54dce-142">deviceModel</span><span class="sxs-lookup"><span data-stu-id="54dce-142">deviceModel</span></span>|<span data-ttu-id="54dce-143">String</span><span class="sxs-lookup"><span data-stu-id="54dce-143">String</span></span>|<span data-ttu-id="54dce-144">レポートされているデバイス モデル</span><span class="sxs-lookup"><span data-stu-id="54dce-144">The device model that is being reported</span></span>|
|<span data-ttu-id="54dce-145">platform</span><span class="sxs-lookup"><span data-stu-id="54dce-145">platform</span></span>|<span data-ttu-id="54dce-146">Int32</span><span class="sxs-lookup"><span data-stu-id="54dce-146">Int32</span></span>|<span data-ttu-id="54dce-147">報告されているデバイスのプラットフォーム</span><span class="sxs-lookup"><span data-stu-id="54dce-147">Platform of the device that is being reported</span></span>|
|<span data-ttu-id="54dce-148">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="54dce-148">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="54dce-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="54dce-149">DateTimeOffset</span></span>|<span data-ttu-id="54dce-150">デバイス コンプライアンスの猶予期間が過ぎる DateTime</span><span class="sxs-lookup"><span data-stu-id="54dce-150">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="54dce-151">status</span><span class="sxs-lookup"><span data-stu-id="54dce-151">status</span></span>|[<span data-ttu-id="54dce-152">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="54dce-152">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="54dce-153">ポリシー レポートのコンプライアンスの状態。</span><span class="sxs-lookup"><span data-stu-id="54dce-153">Compliance status of the policy report.</span></span> <span data-ttu-id="54dce-154">可能な値は、`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned` です。</span><span class="sxs-lookup"><span data-stu-id="54dce-154">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="54dce-155">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="54dce-155">lastReportedDateTime</span></span>|<span data-ttu-id="54dce-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="54dce-156">DateTimeOffset</span></span>|<span data-ttu-id="54dce-157">ポリシー レポートの最終変更日時。</span><span class="sxs-lookup"><span data-stu-id="54dce-157">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="54dce-158">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="54dce-158">userPrincipalName</span></span>|<span data-ttu-id="54dce-159">String</span><span class="sxs-lookup"><span data-stu-id="54dce-159">String</span></span>|<span data-ttu-id="54dce-160">UserPrincipalName。</span><span class="sxs-lookup"><span data-stu-id="54dce-160">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="54dce-161">応答</span><span class="sxs-lookup"><span data-stu-id="54dce-161">Response</span></span>
<span data-ttu-id="54dce-162">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="54dce-162">If successful, this method returns a `201 Created` response code and a [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="54dce-163">例</span><span class="sxs-lookup"><span data-stu-id="54dce-163">Example</span></span>
### <a name="request"></a><span data-ttu-id="54dce-164">要求</span><span class="sxs-lookup"><span data-stu-id="54dce-164">Request</span></span>
<span data-ttu-id="54dce-165">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="54dce-165">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="54dce-166">応答</span><span class="sxs-lookup"><span data-stu-id="54dce-166">Response</span></span>
<span data-ttu-id="54dce-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="54dce-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





