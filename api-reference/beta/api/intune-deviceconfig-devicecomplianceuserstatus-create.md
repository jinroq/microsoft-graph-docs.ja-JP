---
title: deviceComplianceUserStatus の作成
description: 新しい deviceComplianceUserStatus オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: cd489d69656408d840684c5b1f1f7c17f238cd4e
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30141861"
---
# <a name="create-devicecomplianceuserstatus"></a><span data-ttu-id="b3e55-103">deviceComplianceUserStatus の作成</span><span class="sxs-lookup"><span data-stu-id="b3e55-103">Create deviceComplianceUserStatus</span></span>

> <span data-ttu-id="b3e55-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b3e55-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b3e55-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="b3e55-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b3e55-106">新しい [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="b3e55-106">Create a new [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b3e55-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="b3e55-107">Prerequisites</span></span>
<span data-ttu-id="b3e55-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b3e55-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="b3e55-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b3e55-110">Permission type</span></span>|<span data-ttu-id="b3e55-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="b3e55-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b3e55-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b3e55-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b3e55-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b3e55-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b3e55-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b3e55-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b3e55-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b3e55-115">Not supported.</span></span>|
|<span data-ttu-id="b3e55-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b3e55-116">Application</span></span>|<span data-ttu-id="b3e55-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b3e55-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b3e55-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b3e55-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/userStatuses
```

## <a name="request-headers"></a><span data-ttu-id="b3e55-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b3e55-119">Request headers</span></span>
|<span data-ttu-id="b3e55-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b3e55-120">Header</span></span>|<span data-ttu-id="b3e55-121">値</span><span class="sxs-lookup"><span data-stu-id="b3e55-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b3e55-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b3e55-122">Authorization</span></span>|<span data-ttu-id="b3e55-123">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="b3e55-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b3e55-124">承諾</span><span class="sxs-lookup"><span data-stu-id="b3e55-124">Accept</span></span>|<span data-ttu-id="b3e55-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b3e55-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b3e55-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="b3e55-126">Request body</span></span>
<span data-ttu-id="b3e55-127">要求本文で、deviceComplianceUserStatus オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="b3e55-127">In the request body, supply a JSON representation for the deviceComplianceUserStatus object.</span></span>

<span data-ttu-id="b3e55-128">次の表に、deviceComplianceUserStatus の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="b3e55-128">The following table shows the properties that are required when you create the deviceComplianceUserStatus.</span></span>

|<span data-ttu-id="b3e55-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b3e55-129">Property</span></span>|<span data-ttu-id="b3e55-130">型</span><span class="sxs-lookup"><span data-stu-id="b3e55-130">Type</span></span>|<span data-ttu-id="b3e55-131">説明</span><span class="sxs-lookup"><span data-stu-id="b3e55-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b3e55-132">id</span><span class="sxs-lookup"><span data-stu-id="b3e55-132">id</span></span>|<span data-ttu-id="b3e55-133">String</span><span class="sxs-lookup"><span data-stu-id="b3e55-133">String</span></span>|<span data-ttu-id="b3e55-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="b3e55-134">Key of the entity.</span></span>|
|<span data-ttu-id="b3e55-135">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="b3e55-135">userDisplayName</span></span>|<span data-ttu-id="b3e55-136">String</span><span class="sxs-lookup"><span data-stu-id="b3e55-136">String</span></span>|<span data-ttu-id="b3e55-137">DevicePolicyStatus のユーザー名。</span><span class="sxs-lookup"><span data-stu-id="b3e55-137">User name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="b3e55-138">devicesCount</span><span class="sxs-lookup"><span data-stu-id="b3e55-138">devicesCount</span></span>|<span data-ttu-id="b3e55-139">Int32</span><span class="sxs-lookup"><span data-stu-id="b3e55-139">Int32</span></span>|<span data-ttu-id="b3e55-140">そのユーザーのデバイスの数。</span><span class="sxs-lookup"><span data-stu-id="b3e55-140">Devices count for that user.</span></span>|
|<span data-ttu-id="b3e55-141">status</span><span class="sxs-lookup"><span data-stu-id="b3e55-141">status</span></span>|[<span data-ttu-id="b3e55-142">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="b3e55-142">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="b3e55-143">ポリシー レポートのコンプライアンスの状態。</span><span class="sxs-lookup"><span data-stu-id="b3e55-143">Compliance status of the policy report.</span></span> <span data-ttu-id="b3e55-144">可能な値は、`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned` です。</span><span class="sxs-lookup"><span data-stu-id="b3e55-144">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="b3e55-145">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="b3e55-145">lastReportedDateTime</span></span>|<span data-ttu-id="b3e55-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b3e55-146">DateTimeOffset</span></span>|<span data-ttu-id="b3e55-147">ポリシー レポートの最終変更日時。</span><span class="sxs-lookup"><span data-stu-id="b3e55-147">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="b3e55-148">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="b3e55-148">userPrincipalName</span></span>|<span data-ttu-id="b3e55-149">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="b3e55-149">String</span></span>|<span data-ttu-id="b3e55-150">UserPrincipalName。</span><span class="sxs-lookup"><span data-stu-id="b3e55-150">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="b3e55-151">応答</span><span class="sxs-lookup"><span data-stu-id="b3e55-151">Response</span></span>
<span data-ttu-id="b3e55-152">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="b3e55-152">If successful, this method returns a `201 Created` response code and a [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b3e55-153">例</span><span class="sxs-lookup"><span data-stu-id="b3e55-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="b3e55-154">要求</span><span class="sxs-lookup"><span data-stu-id="b3e55-154">Request</span></span>
<span data-ttu-id="b3e55-155">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="b3e55-155">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b3e55-156">応答</span><span class="sxs-lookup"><span data-stu-id="b3e55-156">Response</span></span>
<span data-ttu-id="b3e55-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="b3e55-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




