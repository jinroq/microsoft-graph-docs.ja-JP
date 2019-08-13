---
title: deviceComplianceUserStatus の更新
description: deviceComplianceUserStatus オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ac88383e48f3a605f24e0ef23cf32642485cc28b
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36346066"
---
# <a name="update-devicecomplianceuserstatus"></a><span data-ttu-id="205e8-103">deviceComplianceUserStatus の更新</span><span class="sxs-lookup"><span data-stu-id="205e8-103">Update deviceComplianceUserStatus</span></span>

> <span data-ttu-id="205e8-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="205e8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="205e8-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="205e8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="205e8-106">[deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="205e8-106">Update the properties of a [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="205e8-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="205e8-107">Prerequisites</span></span>
<span data-ttu-id="205e8-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="205e8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="205e8-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="205e8-110">Permission type</span></span>|<span data-ttu-id="205e8-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="205e8-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="205e8-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="205e8-112">Delegated (work or school account)</span></span>|<span data-ttu-id="205e8-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="205e8-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="205e8-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="205e8-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="205e8-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="205e8-115">Not supported.</span></span>|
|<span data-ttu-id="205e8-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="205e8-116">Application</span></span>|<span data-ttu-id="205e8-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="205e8-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="205e8-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="205e8-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/userStatuses/{deviceComplianceUserStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="205e8-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="205e8-119">Request headers</span></span>
|<span data-ttu-id="205e8-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="205e8-120">Header</span></span>|<span data-ttu-id="205e8-121">値</span><span class="sxs-lookup"><span data-stu-id="205e8-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="205e8-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="205e8-122">Authorization</span></span>|<span data-ttu-id="205e8-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="205e8-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="205e8-124">承諾</span><span class="sxs-lookup"><span data-stu-id="205e8-124">Accept</span></span>|<span data-ttu-id="205e8-125">application/json</span><span class="sxs-lookup"><span data-stu-id="205e8-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="205e8-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="205e8-126">Request body</span></span>
<span data-ttu-id="205e8-127">要求本文で、[deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="205e8-127">In the request body, supply a JSON representation for the [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) object.</span></span>

<span data-ttu-id="205e8-128">次の表に、[deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="205e8-128">The following table shows the properties that are required when you create the [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md).</span></span>

|<span data-ttu-id="205e8-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="205e8-129">Property</span></span>|<span data-ttu-id="205e8-130">型</span><span class="sxs-lookup"><span data-stu-id="205e8-130">Type</span></span>|<span data-ttu-id="205e8-131">説明</span><span class="sxs-lookup"><span data-stu-id="205e8-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="205e8-132">id</span><span class="sxs-lookup"><span data-stu-id="205e8-132">id</span></span>|<span data-ttu-id="205e8-133">文字列</span><span class="sxs-lookup"><span data-stu-id="205e8-133">String</span></span>|<span data-ttu-id="205e8-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="205e8-134">Key of the entity.</span></span>|
|<span data-ttu-id="205e8-135">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="205e8-135">userDisplayName</span></span>|<span data-ttu-id="205e8-136">String</span><span class="sxs-lookup"><span data-stu-id="205e8-136">String</span></span>|<span data-ttu-id="205e8-137">DevicePolicyStatus のユーザー名。</span><span class="sxs-lookup"><span data-stu-id="205e8-137">User name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="205e8-138">devicesCount</span><span class="sxs-lookup"><span data-stu-id="205e8-138">devicesCount</span></span>|<span data-ttu-id="205e8-139">Int32</span><span class="sxs-lookup"><span data-stu-id="205e8-139">Int32</span></span>|<span data-ttu-id="205e8-140">そのユーザーのデバイスの数。</span><span class="sxs-lookup"><span data-stu-id="205e8-140">Devices count for that user.</span></span>|
|<span data-ttu-id="205e8-141">status</span><span class="sxs-lookup"><span data-stu-id="205e8-141">status</span></span>|[<span data-ttu-id="205e8-142">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="205e8-142">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="205e8-143">ポリシー レポートのコンプライアンスの状態。</span><span class="sxs-lookup"><span data-stu-id="205e8-143">Compliance status of the policy report.</span></span> <span data-ttu-id="205e8-144">可能な値は、`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned` です。</span><span class="sxs-lookup"><span data-stu-id="205e8-144">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="205e8-145">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="205e8-145">lastReportedDateTime</span></span>|<span data-ttu-id="205e8-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="205e8-146">DateTimeOffset</span></span>|<span data-ttu-id="205e8-147">ポリシー レポートの最終変更日時。</span><span class="sxs-lookup"><span data-stu-id="205e8-147">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="205e8-148">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="205e8-148">userPrincipalName</span></span>|<span data-ttu-id="205e8-149">String</span><span class="sxs-lookup"><span data-stu-id="205e8-149">String</span></span>|<span data-ttu-id="205e8-150">UserPrincipalName。</span><span class="sxs-lookup"><span data-stu-id="205e8-150">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="205e8-151">応答</span><span class="sxs-lookup"><span data-stu-id="205e8-151">Response</span></span>
<span data-ttu-id="205e8-152">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="205e8-152">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="205e8-153">例</span><span class="sxs-lookup"><span data-stu-id="205e8-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="205e8-154">要求</span><span class="sxs-lookup"><span data-stu-id="205e8-154">Request</span></span>
<span data-ttu-id="205e8-155">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="205e8-155">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/userStatuses/{deviceComplianceUserStatusId}
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

### <a name="response"></a><span data-ttu-id="205e8-156">応答</span><span class="sxs-lookup"><span data-stu-id="205e8-156">Response</span></span>
<span data-ttu-id="205e8-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="205e8-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






