---
title: deviceComplianceUserStatus の更新
description: deviceComplianceUserStatus オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 40d58158ca3a0e17f7f92b15a35f1b730d2511c4
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27852802"
---
# <a name="update-devicecomplianceuserstatus"></a><span data-ttu-id="b8c20-103">deviceComplianceUserStatus の更新</span><span class="sxs-lookup"><span data-stu-id="b8c20-103">Update deviceComplianceUserStatus</span></span>

> <span data-ttu-id="b8c20-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="b8c20-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b8c20-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b8c20-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b8c20-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="b8c20-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b8c20-107">[deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="b8c20-107">Update the properties of a [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b8c20-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="b8c20-108">Prerequisites</span></span>
<span data-ttu-id="b8c20-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b8c20-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b8c20-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b8c20-111">Permission type</span></span>|<span data-ttu-id="b8c20-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="b8c20-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b8c20-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b8c20-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b8c20-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b8c20-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b8c20-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b8c20-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b8c20-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b8c20-116">Not supported.</span></span>|
|<span data-ttu-id="b8c20-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b8c20-117">Application</span></span>|<span data-ttu-id="b8c20-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b8c20-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b8c20-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b8c20-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/userStatuses/{deviceComplianceUserStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="b8c20-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b8c20-120">Request headers</span></span>
|<span data-ttu-id="b8c20-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b8c20-121">Header</span></span>|<span data-ttu-id="b8c20-122">値</span><span class="sxs-lookup"><span data-stu-id="b8c20-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b8c20-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b8c20-123">Authorization</span></span>|<span data-ttu-id="b8c20-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="b8c20-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b8c20-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b8c20-125">Accept</span></span>|<span data-ttu-id="b8c20-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b8c20-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b8c20-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="b8c20-127">Request body</span></span>
<span data-ttu-id="b8c20-128">要求本文で、[deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="b8c20-128">In the request body, supply a JSON representation for the [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) object.</span></span>

<span data-ttu-id="b8c20-129">次の表に、[deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="b8c20-129">The following table shows the properties that are required when you create the [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md).</span></span>

|<span data-ttu-id="b8c20-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b8c20-130">Property</span></span>|<span data-ttu-id="b8c20-131">種類</span><span class="sxs-lookup"><span data-stu-id="b8c20-131">Type</span></span>|<span data-ttu-id="b8c20-132">説明</span><span class="sxs-lookup"><span data-stu-id="b8c20-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b8c20-133">ID</span><span class="sxs-lookup"><span data-stu-id="b8c20-133">id</span></span>|<span data-ttu-id="b8c20-134">String</span><span class="sxs-lookup"><span data-stu-id="b8c20-134">String</span></span>|<span data-ttu-id="b8c20-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="b8c20-135">Key of the entity.</span></span>|
|<span data-ttu-id="b8c20-136">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="b8c20-136">userDisplayName</span></span>|<span data-ttu-id="b8c20-137">String</span><span class="sxs-lookup"><span data-stu-id="b8c20-137">String</span></span>|<span data-ttu-id="b8c20-138">DevicePolicyStatus のユーザー名。</span><span class="sxs-lookup"><span data-stu-id="b8c20-138">User name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="b8c20-139">devicesCount</span><span class="sxs-lookup"><span data-stu-id="b8c20-139">devicesCount</span></span>|<span data-ttu-id="b8c20-140">Int32</span><span class="sxs-lookup"><span data-stu-id="b8c20-140">Int32</span></span>|<span data-ttu-id="b8c20-141">そのユーザーのデバイスの数。</span><span class="sxs-lookup"><span data-stu-id="b8c20-141">Devices count for that user.</span></span>|
|<span data-ttu-id="b8c20-142">status</span><span class="sxs-lookup"><span data-stu-id="b8c20-142">status</span></span>|[<span data-ttu-id="b8c20-143">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="b8c20-143">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="b8c20-144">ポリシー レポートのコンプライアンスの状態。</span><span class="sxs-lookup"><span data-stu-id="b8c20-144">Compliance status of the policy report.</span></span> <span data-ttu-id="b8c20-145">可能な値は、`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned` です。</span><span class="sxs-lookup"><span data-stu-id="b8c20-145">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="b8c20-146">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="b8c20-146">lastReportedDateTime</span></span>|<span data-ttu-id="b8c20-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b8c20-147">DateTimeOffset</span></span>|<span data-ttu-id="b8c20-148">ポリシー レポートの最終変更日時。</span><span class="sxs-lookup"><span data-stu-id="b8c20-148">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="b8c20-149">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="b8c20-149">userPrincipalName</span></span>|<span data-ttu-id="b8c20-150">String</span><span class="sxs-lookup"><span data-stu-id="b8c20-150">String</span></span>|<span data-ttu-id="b8c20-151">UserPrincipalName。</span><span class="sxs-lookup"><span data-stu-id="b8c20-151">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="b8c20-152">応答</span><span class="sxs-lookup"><span data-stu-id="b8c20-152">Response</span></span>
<span data-ttu-id="b8c20-153">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="b8c20-153">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b8c20-154">例</span><span class="sxs-lookup"><span data-stu-id="b8c20-154">Example</span></span>
### <a name="request"></a><span data-ttu-id="b8c20-155">要求</span><span class="sxs-lookup"><span data-stu-id="b8c20-155">Request</span></span>
<span data-ttu-id="b8c20-156">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="b8c20-156">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/userStatuses/{deviceComplianceUserStatusId}
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

### <a name="response"></a><span data-ttu-id="b8c20-157">応答</span><span class="sxs-lookup"><span data-stu-id="b8c20-157">Response</span></span>
<span data-ttu-id="b8c20-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="b8c20-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





