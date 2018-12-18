---
title: deviceComplianceUserStatus の更新
description: deviceComplianceUserStatus オブジェクトのプロパティを更新します。
author: tfitzmac
ms.openlocfilehash: ee15016b3055f4b51230cc17638151551c9f8c63
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27353061"
---
# <a name="update-devicecomplianceuserstatus"></a><span data-ttu-id="40ecd-103">deviceComplianceUserStatus の更新</span><span class="sxs-lookup"><span data-stu-id="40ecd-103">Update deviceComplianceUserStatus</span></span>

> <span data-ttu-id="40ecd-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="40ecd-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="40ecd-105">[deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="40ecd-105">Update the properties of a [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="40ecd-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="40ecd-106">Prerequisites</span></span>
<span data-ttu-id="40ecd-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="40ecd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="40ecd-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="40ecd-109">Permission type</span></span>|<span data-ttu-id="40ecd-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="40ecd-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="40ecd-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="40ecd-111">Delegated (work or school account)</span></span>|<span data-ttu-id="40ecd-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="40ecd-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="40ecd-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="40ecd-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="40ecd-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="40ecd-114">Not supported.</span></span>|
|<span data-ttu-id="40ecd-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="40ecd-115">Application</span></span>|<span data-ttu-id="40ecd-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="40ecd-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="40ecd-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="40ecd-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/userStatuses/{deviceComplianceUserStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="40ecd-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="40ecd-118">Request headers</span></span>
|<span data-ttu-id="40ecd-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="40ecd-119">Header</span></span>|<span data-ttu-id="40ecd-120">値</span><span class="sxs-lookup"><span data-stu-id="40ecd-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="40ecd-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="40ecd-121">Authorization</span></span>|<span data-ttu-id="40ecd-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="40ecd-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="40ecd-123">Accept</span><span class="sxs-lookup"><span data-stu-id="40ecd-123">Accept</span></span>|<span data-ttu-id="40ecd-124">application/json</span><span class="sxs-lookup"><span data-stu-id="40ecd-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="40ecd-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="40ecd-125">Request body</span></span>
<span data-ttu-id="40ecd-126">要求本文で、[deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="40ecd-126">In the request body, supply a JSON representation for the [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) object.</span></span>

<span data-ttu-id="40ecd-127">次の表に、[deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="40ecd-127">The following table shows the properties that are required when you create the [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md).</span></span>

|<span data-ttu-id="40ecd-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="40ecd-128">Property</span></span>|<span data-ttu-id="40ecd-129">種類</span><span class="sxs-lookup"><span data-stu-id="40ecd-129">Type</span></span>|<span data-ttu-id="40ecd-130">説明</span><span class="sxs-lookup"><span data-stu-id="40ecd-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="40ecd-131">ID</span><span class="sxs-lookup"><span data-stu-id="40ecd-131">id</span></span>|<span data-ttu-id="40ecd-132">String</span><span class="sxs-lookup"><span data-stu-id="40ecd-132">String</span></span>|<span data-ttu-id="40ecd-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="40ecd-133">Key of the entity.</span></span>|
|<span data-ttu-id="40ecd-134">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="40ecd-134">userDisplayName</span></span>|<span data-ttu-id="40ecd-135">String</span><span class="sxs-lookup"><span data-stu-id="40ecd-135">String</span></span>|<span data-ttu-id="40ecd-136">DevicePolicyStatus のユーザー名。</span><span class="sxs-lookup"><span data-stu-id="40ecd-136">User name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="40ecd-137">devicesCount</span><span class="sxs-lookup"><span data-stu-id="40ecd-137">devicesCount</span></span>|<span data-ttu-id="40ecd-138">Int32</span><span class="sxs-lookup"><span data-stu-id="40ecd-138">Int32</span></span>|<span data-ttu-id="40ecd-139">そのユーザーのデバイスの数。</span><span class="sxs-lookup"><span data-stu-id="40ecd-139">Devices count for that user.</span></span>|
|<span data-ttu-id="40ecd-140">status</span><span class="sxs-lookup"><span data-stu-id="40ecd-140">status</span></span>|[<span data-ttu-id="40ecd-141">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="40ecd-141">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="40ecd-142">ポリシー レポートのコンプライアンスの状態。</span><span class="sxs-lookup"><span data-stu-id="40ecd-142">Compliance status of the policy report.</span></span> <span data-ttu-id="40ecd-143">可能な値は、`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned` です。</span><span class="sxs-lookup"><span data-stu-id="40ecd-143">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="40ecd-144">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="40ecd-144">lastReportedDateTime</span></span>|<span data-ttu-id="40ecd-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="40ecd-145">DateTimeOffset</span></span>|<span data-ttu-id="40ecd-146">ポリシー レポートの最終変更日時。</span><span class="sxs-lookup"><span data-stu-id="40ecd-146">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="40ecd-147">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="40ecd-147">userPrincipalName</span></span>|<span data-ttu-id="40ecd-148">String</span><span class="sxs-lookup"><span data-stu-id="40ecd-148">String</span></span>|<span data-ttu-id="40ecd-149">UserPrincipalName。</span><span class="sxs-lookup"><span data-stu-id="40ecd-149">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="40ecd-150">応答</span><span class="sxs-lookup"><span data-stu-id="40ecd-150">Response</span></span>
<span data-ttu-id="40ecd-151">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="40ecd-151">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="40ecd-152">例</span><span class="sxs-lookup"><span data-stu-id="40ecd-152">Example</span></span>
### <a name="request"></a><span data-ttu-id="40ecd-153">要求</span><span class="sxs-lookup"><span data-stu-id="40ecd-153">Request</span></span>
<span data-ttu-id="40ecd-154">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="40ecd-154">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/userStatuses/{deviceComplianceUserStatusId}
Content-type: application/json
Content-length: 287

{
  "@odata.type": "#microsoft.graph.deviceComplianceUserStatus",
  "userDisplayName": "User Display Name value",
  "devicesCount": 12,
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="40ecd-155">応答</span><span class="sxs-lookup"><span data-stu-id="40ecd-155">Response</span></span>
<span data-ttu-id="40ecd-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="40ecd-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 336

{
  "@odata.type": "#microsoft.graph.deviceComplianceUserStatus",
  "id": "a0b566cd-66cd-a0b5-cd66-b5a0cd66b5a0",
  "userDisplayName": "User Display Name value",
  "devicesCount": 12,
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```



