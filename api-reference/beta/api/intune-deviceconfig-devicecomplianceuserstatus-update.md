---
title: deviceComplianceUserStatus の更新
description: deviceComplianceUserStatus オブジェクトのプロパティを更新します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 0316f19ae718fbd358868fe7701d7ab833db75af
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29416042"
---
# <a name="update-devicecomplianceuserstatus"></a><span data-ttu-id="547fe-103">deviceComplianceUserStatus の更新</span><span class="sxs-lookup"><span data-stu-id="547fe-103">Update deviceComplianceUserStatus</span></span>

> <span data-ttu-id="547fe-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="547fe-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="547fe-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="547fe-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="547fe-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="547fe-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="547fe-107">[deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="547fe-107">Update the properties of a [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="547fe-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="547fe-108">Prerequisites</span></span>
<span data-ttu-id="547fe-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="547fe-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="547fe-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="547fe-111">Permission type</span></span>|<span data-ttu-id="547fe-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="547fe-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="547fe-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="547fe-113">Delegated (work or school account)</span></span>|<span data-ttu-id="547fe-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="547fe-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="547fe-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="547fe-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="547fe-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="547fe-116">Not supported.</span></span>|
|<span data-ttu-id="547fe-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="547fe-117">Application</span></span>|<span data-ttu-id="547fe-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="547fe-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="547fe-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="547fe-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/userStatuses/{deviceComplianceUserStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="547fe-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="547fe-120">Request headers</span></span>
|<span data-ttu-id="547fe-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="547fe-121">Header</span></span>|<span data-ttu-id="547fe-122">値</span><span class="sxs-lookup"><span data-stu-id="547fe-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="547fe-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="547fe-123">Authorization</span></span>|<span data-ttu-id="547fe-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="547fe-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="547fe-125">Accept</span><span class="sxs-lookup"><span data-stu-id="547fe-125">Accept</span></span>|<span data-ttu-id="547fe-126">application/json</span><span class="sxs-lookup"><span data-stu-id="547fe-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="547fe-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="547fe-127">Request body</span></span>
<span data-ttu-id="547fe-128">要求本文で、[deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="547fe-128">In the request body, supply a JSON representation for the [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) object.</span></span>

<span data-ttu-id="547fe-129">次の表に、[deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="547fe-129">The following table shows the properties that are required when you create the [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md).</span></span>

|<span data-ttu-id="547fe-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="547fe-130">Property</span></span>|<span data-ttu-id="547fe-131">型</span><span class="sxs-lookup"><span data-stu-id="547fe-131">Type</span></span>|<span data-ttu-id="547fe-132">説明</span><span class="sxs-lookup"><span data-stu-id="547fe-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="547fe-133">id</span><span class="sxs-lookup"><span data-stu-id="547fe-133">id</span></span>|<span data-ttu-id="547fe-134">String</span><span class="sxs-lookup"><span data-stu-id="547fe-134">String</span></span>|<span data-ttu-id="547fe-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="547fe-135">Key of the entity.</span></span>|
|<span data-ttu-id="547fe-136">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="547fe-136">userDisplayName</span></span>|<span data-ttu-id="547fe-137">String</span><span class="sxs-lookup"><span data-stu-id="547fe-137">String</span></span>|<span data-ttu-id="547fe-138">DevicePolicyStatus のユーザー名。</span><span class="sxs-lookup"><span data-stu-id="547fe-138">User name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="547fe-139">devicesCount</span><span class="sxs-lookup"><span data-stu-id="547fe-139">devicesCount</span></span>|<span data-ttu-id="547fe-140">Int32</span><span class="sxs-lookup"><span data-stu-id="547fe-140">Int32</span></span>|<span data-ttu-id="547fe-141">そのユーザーのデバイスの数。</span><span class="sxs-lookup"><span data-stu-id="547fe-141">Devices count for that user.</span></span>|
|<span data-ttu-id="547fe-142">status</span><span class="sxs-lookup"><span data-stu-id="547fe-142">status</span></span>|[<span data-ttu-id="547fe-143">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="547fe-143">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="547fe-144">ポリシー レポートのコンプライアンスの状態。</span><span class="sxs-lookup"><span data-stu-id="547fe-144">Compliance status of the policy report.</span></span> <span data-ttu-id="547fe-145">可能な値は、`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned` です。</span><span class="sxs-lookup"><span data-stu-id="547fe-145">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="547fe-146">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="547fe-146">lastReportedDateTime</span></span>|<span data-ttu-id="547fe-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="547fe-147">DateTimeOffset</span></span>|<span data-ttu-id="547fe-148">ポリシー レポートの最終変更日時。</span><span class="sxs-lookup"><span data-stu-id="547fe-148">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="547fe-149">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="547fe-149">userPrincipalName</span></span>|<span data-ttu-id="547fe-150">String</span><span class="sxs-lookup"><span data-stu-id="547fe-150">String</span></span>|<span data-ttu-id="547fe-151">UserPrincipalName。</span><span class="sxs-lookup"><span data-stu-id="547fe-151">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="547fe-152">応答</span><span class="sxs-lookup"><span data-stu-id="547fe-152">Response</span></span>
<span data-ttu-id="547fe-153">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="547fe-153">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="547fe-154">例</span><span class="sxs-lookup"><span data-stu-id="547fe-154">Example</span></span>

### <a name="request"></a><span data-ttu-id="547fe-155">要求</span><span class="sxs-lookup"><span data-stu-id="547fe-155">Request</span></span>
<span data-ttu-id="547fe-156">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="547fe-156">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="547fe-157">応答</span><span class="sxs-lookup"><span data-stu-id="547fe-157">Response</span></span>
<span data-ttu-id="547fe-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="547fe-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




