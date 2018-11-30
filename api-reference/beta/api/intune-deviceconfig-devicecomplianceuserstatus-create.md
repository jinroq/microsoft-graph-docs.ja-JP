---
title: deviceComplianceUserStatus の作成
description: 新しい deviceComplianceUserStatus オブジェクトを作成します。
ms.openlocfilehash: 03b2b221ba41c2b8812c6cb0d4e6ec9ab711b583
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27073274"
---
# <a name="create-devicecomplianceuserstatus"></a><span data-ttu-id="5f510-103">deviceComplianceUserStatus の作成</span><span class="sxs-lookup"><span data-stu-id="5f510-103">Create deviceComplianceUserStatus</span></span>

> <span data-ttu-id="5f510-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="5f510-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5f510-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5f510-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5f510-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="5f510-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5f510-107">新しい [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="5f510-107">Create a new [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="5f510-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="5f510-108">Prerequisites</span></span>
<span data-ttu-id="5f510-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5f510-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5f510-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="5f510-111">Permission type</span></span>|<span data-ttu-id="5f510-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="5f510-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5f510-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="5f510-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5f510-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5f510-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="5f510-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="5f510-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5f510-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5f510-116">Not supported.</span></span>|
|<span data-ttu-id="5f510-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="5f510-117">Application</span></span>|<span data-ttu-id="5f510-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5f510-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5f510-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="5f510-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/userStatuses
```

## <a name="request-headers"></a><span data-ttu-id="5f510-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5f510-120">Request headers</span></span>
|<span data-ttu-id="5f510-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5f510-121">Header</span></span>|<span data-ttu-id="5f510-122">値</span><span class="sxs-lookup"><span data-stu-id="5f510-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5f510-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5f510-123">Authorization</span></span>|<span data-ttu-id="5f510-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="5f510-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5f510-125">Accept</span><span class="sxs-lookup"><span data-stu-id="5f510-125">Accept</span></span>|<span data-ttu-id="5f510-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5f510-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5f510-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="5f510-127">Request body</span></span>
<span data-ttu-id="5f510-128">要求本文で、deviceComplianceUserStatus オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="5f510-128">In the request body, supply a JSON representation for the deviceComplianceUserStatus object.</span></span>

<span data-ttu-id="5f510-129">次の表に、deviceComplianceUserStatus の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="5f510-129">The following table shows the properties that are required when you create the deviceComplianceUserStatus.</span></span>

|<span data-ttu-id="5f510-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5f510-130">Property</span></span>|<span data-ttu-id="5f510-131">型</span><span class="sxs-lookup"><span data-stu-id="5f510-131">Type</span></span>|<span data-ttu-id="5f510-132">説明</span><span class="sxs-lookup"><span data-stu-id="5f510-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5f510-133">id</span><span class="sxs-lookup"><span data-stu-id="5f510-133">id</span></span>|<span data-ttu-id="5f510-134">String</span><span class="sxs-lookup"><span data-stu-id="5f510-134">String</span></span>|<span data-ttu-id="5f510-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="5f510-135">Key of the entity.</span></span>|
|<span data-ttu-id="5f510-136">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="5f510-136">userDisplayName</span></span>|<span data-ttu-id="5f510-137">String</span><span class="sxs-lookup"><span data-stu-id="5f510-137">String</span></span>|<span data-ttu-id="5f510-138">DevicePolicyStatus のユーザー名。</span><span class="sxs-lookup"><span data-stu-id="5f510-138">User name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="5f510-139">devicesCount</span><span class="sxs-lookup"><span data-stu-id="5f510-139">devicesCount</span></span>|<span data-ttu-id="5f510-140">Int32</span><span class="sxs-lookup"><span data-stu-id="5f510-140">Int32</span></span>|<span data-ttu-id="5f510-141">そのユーザーのデバイスの数。</span><span class="sxs-lookup"><span data-stu-id="5f510-141">Devices count for that user.</span></span>|
|<span data-ttu-id="5f510-142">status</span><span class="sxs-lookup"><span data-stu-id="5f510-142">status</span></span>|[<span data-ttu-id="5f510-143">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="5f510-143">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="5f510-144">ポリシー レポートのコンプライアンスの状態。</span><span class="sxs-lookup"><span data-stu-id="5f510-144">Compliance status of the policy report.</span></span> <span data-ttu-id="5f510-145">可能な値は、`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned` です。</span><span class="sxs-lookup"><span data-stu-id="5f510-145">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="5f510-146">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="5f510-146">lastReportedDateTime</span></span>|<span data-ttu-id="5f510-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5f510-147">DateTimeOffset</span></span>|<span data-ttu-id="5f510-148">ポリシー レポートの最終変更日時。</span><span class="sxs-lookup"><span data-stu-id="5f510-148">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="5f510-149">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="5f510-149">userPrincipalName</span></span>|<span data-ttu-id="5f510-150">String</span><span class="sxs-lookup"><span data-stu-id="5f510-150">String</span></span>|<span data-ttu-id="5f510-151">UserPrincipalName。</span><span class="sxs-lookup"><span data-stu-id="5f510-151">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="5f510-152">応答</span><span class="sxs-lookup"><span data-stu-id="5f510-152">Response</span></span>
<span data-ttu-id="5f510-153">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="5f510-153">If successful, this method returns a `201 Created` response code and a [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5f510-154">例</span><span class="sxs-lookup"><span data-stu-id="5f510-154">Example</span></span>
### <a name="request"></a><span data-ttu-id="5f510-155">要求</span><span class="sxs-lookup"><span data-stu-id="5f510-155">Request</span></span>
<span data-ttu-id="5f510-156">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="5f510-156">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/userStatuses
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

### <a name="response"></a><span data-ttu-id="5f510-157">応答</span><span class="sxs-lookup"><span data-stu-id="5f510-157">Response</span></span>
<span data-ttu-id="5f510-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="5f510-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





