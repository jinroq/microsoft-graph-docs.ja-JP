---
title: deviceComplianceUserStatus の作成
description: 新しい deviceComplianceUserStatus オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b855f9515e2c0bda21817ac00c0a3948904dabe1
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32574583"
---
# <a name="create-devicecomplianceuserstatus"></a><span data-ttu-id="a2535-103">deviceComplianceUserStatus の作成</span><span class="sxs-lookup"><span data-stu-id="a2535-103">Create deviceComplianceUserStatus</span></span>

> <span data-ttu-id="a2535-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="a2535-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a2535-105">新しい [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="a2535-105">Create a new [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a2535-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="a2535-106">Prerequisites</span></span>
<span data-ttu-id="a2535-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a2535-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a2535-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a2535-109">Permission type</span></span>|<span data-ttu-id="a2535-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="a2535-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a2535-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a2535-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a2535-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a2535-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a2535-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a2535-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a2535-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a2535-114">Not supported.</span></span>|
|<span data-ttu-id="a2535-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a2535-115">Application</span></span>|<span data-ttu-id="a2535-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a2535-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a2535-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a2535-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/userStatuses
```

## <a name="request-headers"></a><span data-ttu-id="a2535-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a2535-118">Request headers</span></span>
|<span data-ttu-id="a2535-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a2535-119">Header</span></span>|<span data-ttu-id="a2535-120">値</span><span class="sxs-lookup"><span data-stu-id="a2535-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a2535-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="a2535-121">Authorization</span></span>|<span data-ttu-id="a2535-122">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="a2535-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a2535-123">承諾</span><span class="sxs-lookup"><span data-stu-id="a2535-123">Accept</span></span>|<span data-ttu-id="a2535-124">application/json</span><span class="sxs-lookup"><span data-stu-id="a2535-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a2535-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="a2535-125">Request body</span></span>
<span data-ttu-id="a2535-126">要求本文で、deviceComplianceUserStatus オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="a2535-126">In the request body, supply a JSON representation for the deviceComplianceUserStatus object.</span></span>

<span data-ttu-id="a2535-127">次の表に、deviceComplianceUserStatus の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="a2535-127">The following table shows the properties that are required when you create the deviceComplianceUserStatus.</span></span>

|<span data-ttu-id="a2535-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a2535-128">Property</span></span>|<span data-ttu-id="a2535-129">型</span><span class="sxs-lookup"><span data-stu-id="a2535-129">Type</span></span>|<span data-ttu-id="a2535-130">説明</span><span class="sxs-lookup"><span data-stu-id="a2535-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a2535-131">id</span><span class="sxs-lookup"><span data-stu-id="a2535-131">id</span></span>|<span data-ttu-id="a2535-132">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="a2535-132">String</span></span>|<span data-ttu-id="a2535-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="a2535-133">Key of the entity.</span></span>|
|<span data-ttu-id="a2535-134">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="a2535-134">userDisplayName</span></span>|<span data-ttu-id="a2535-135">String</span><span class="sxs-lookup"><span data-stu-id="a2535-135">String</span></span>|<span data-ttu-id="a2535-136">DevicePolicyStatus のユーザー名。</span><span class="sxs-lookup"><span data-stu-id="a2535-136">User name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="a2535-137">devicesCount</span><span class="sxs-lookup"><span data-stu-id="a2535-137">devicesCount</span></span>|<span data-ttu-id="a2535-138">Int32</span><span class="sxs-lookup"><span data-stu-id="a2535-138">Int32</span></span>|<span data-ttu-id="a2535-139">そのユーザーのデバイスの数。</span><span class="sxs-lookup"><span data-stu-id="a2535-139">Devices count for that user.</span></span>|
|<span data-ttu-id="a2535-140">status</span><span class="sxs-lookup"><span data-stu-id="a2535-140">status</span></span>|[<span data-ttu-id="a2535-141">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="a2535-141">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="a2535-142">ポリシー レポートのコンプライアンスの状態。</span><span class="sxs-lookup"><span data-stu-id="a2535-142">Compliance status of the policy report.</span></span> <span data-ttu-id="a2535-143">可能な値は、`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned` です。</span><span class="sxs-lookup"><span data-stu-id="a2535-143">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="a2535-144">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="a2535-144">lastReportedDateTime</span></span>|<span data-ttu-id="a2535-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a2535-145">DateTimeOffset</span></span>|<span data-ttu-id="a2535-146">ポリシー レポートの最終変更日時。</span><span class="sxs-lookup"><span data-stu-id="a2535-146">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="a2535-147">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="a2535-147">userPrincipalName</span></span>|<span data-ttu-id="a2535-148">String</span><span class="sxs-lookup"><span data-stu-id="a2535-148">String</span></span>|<span data-ttu-id="a2535-149">UserPrincipalName。</span><span class="sxs-lookup"><span data-stu-id="a2535-149">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="a2535-150">応答</span><span class="sxs-lookup"><span data-stu-id="a2535-150">Response</span></span>
<span data-ttu-id="a2535-151">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="a2535-151">If successful, this method returns a `201 Created` response code and a [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a2535-152">例</span><span class="sxs-lookup"><span data-stu-id="a2535-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="a2535-153">要求</span><span class="sxs-lookup"><span data-stu-id="a2535-153">Request</span></span>
<span data-ttu-id="a2535-154">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="a2535-154">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/userStatuses
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

### <a name="response"></a><span data-ttu-id="a2535-155">応答</span><span class="sxs-lookup"><span data-stu-id="a2535-155">Response</span></span>
<span data-ttu-id="a2535-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="a2535-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



