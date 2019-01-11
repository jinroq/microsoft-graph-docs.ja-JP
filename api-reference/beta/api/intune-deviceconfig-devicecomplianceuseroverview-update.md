---
title: deviceComplianceUserOverview の更新
description: deviceComplianceUserOverview オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 05ccf80b957bf52155dfef738c886cf41155fc22
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27891106"
---
# <a name="update-devicecomplianceuseroverview"></a><span data-ttu-id="57e5d-103">deviceComplianceUserOverview の更新</span><span class="sxs-lookup"><span data-stu-id="57e5d-103">Update deviceComplianceUserOverview</span></span>

> <span data-ttu-id="57e5d-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="57e5d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="57e5d-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="57e5d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="57e5d-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="57e5d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="57e5d-107">[deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="57e5d-107">Update the properties of a [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="57e5d-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="57e5d-108">Prerequisites</span></span>
<span data-ttu-id="57e5d-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="57e5d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="57e5d-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="57e5d-111">Permission type</span></span>|<span data-ttu-id="57e5d-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="57e5d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="57e5d-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="57e5d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="57e5d-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="57e5d-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="57e5d-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="57e5d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="57e5d-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="57e5d-116">Not supported.</span></span>|
|<span data-ttu-id="57e5d-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="57e5d-117">Application</span></span>|<span data-ttu-id="57e5d-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="57e5d-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="57e5d-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="57e5d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/userStatusOverview
```

## <a name="request-headers"></a><span data-ttu-id="57e5d-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="57e5d-120">Request headers</span></span>
|<span data-ttu-id="57e5d-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="57e5d-121">Header</span></span>|<span data-ttu-id="57e5d-122">値</span><span class="sxs-lookup"><span data-stu-id="57e5d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="57e5d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="57e5d-123">Authorization</span></span>|<span data-ttu-id="57e5d-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="57e5d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="57e5d-125">Accept</span><span class="sxs-lookup"><span data-stu-id="57e5d-125">Accept</span></span>|<span data-ttu-id="57e5d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="57e5d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="57e5d-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="57e5d-127">Request body</span></span>
<span data-ttu-id="57e5d-128">要求本文で、[deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="57e5d-128">In the request body, supply a JSON representation for the [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) object.</span></span>

<span data-ttu-id="57e5d-129">次の表に、[deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="57e5d-129">The following table shows the properties that are required when you create the [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md).</span></span>

|<span data-ttu-id="57e5d-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="57e5d-130">Property</span></span>|<span data-ttu-id="57e5d-131">種類</span><span class="sxs-lookup"><span data-stu-id="57e5d-131">Type</span></span>|<span data-ttu-id="57e5d-132">説明</span><span class="sxs-lookup"><span data-stu-id="57e5d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="57e5d-133">ID</span><span class="sxs-lookup"><span data-stu-id="57e5d-133">id</span></span>|<span data-ttu-id="57e5d-134">String</span><span class="sxs-lookup"><span data-stu-id="57e5d-134">String</span></span>|<span data-ttu-id="57e5d-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="57e5d-135">Key of the entity.</span></span>|
|<span data-ttu-id="57e5d-136">pendingCount</span><span class="sxs-lookup"><span data-stu-id="57e5d-136">pendingCount</span></span>|<span data-ttu-id="57e5d-137">Int32</span><span class="sxs-lookup"><span data-stu-id="57e5d-137">Int32</span></span>|<span data-ttu-id="57e5d-138">保留中のユーザーの数</span><span class="sxs-lookup"><span data-stu-id="57e5d-138">Number of pending Users</span></span>|
|<span data-ttu-id="57e5d-139">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="57e5d-139">notApplicableCount</span></span>|<span data-ttu-id="57e5d-140">Int32</span><span class="sxs-lookup"><span data-stu-id="57e5d-140">Int32</span></span>|<span data-ttu-id="57e5d-141">適用されないユーザーの数</span><span class="sxs-lookup"><span data-stu-id="57e5d-141">Number of not applicable users</span></span>|
|<span data-ttu-id="57e5d-142">successCount</span><span class="sxs-lookup"><span data-stu-id="57e5d-142">successCount</span></span>|<span data-ttu-id="57e5d-143">Int32</span><span class="sxs-lookup"><span data-stu-id="57e5d-143">Int32</span></span>|<span data-ttu-id="57e5d-144">成功したユーザーの数</span><span class="sxs-lookup"><span data-stu-id="57e5d-144">Number of succeeded Users</span></span>|
|<span data-ttu-id="57e5d-145">errorCount</span><span class="sxs-lookup"><span data-stu-id="57e5d-145">errorCount</span></span>|<span data-ttu-id="57e5d-146">Int32</span><span class="sxs-lookup"><span data-stu-id="57e5d-146">Int32</span></span>|<span data-ttu-id="57e5d-147">エラー ユーザーの数</span><span class="sxs-lookup"><span data-stu-id="57e5d-147">Number of error Users</span></span>|
|<span data-ttu-id="57e5d-148">failedCount</span><span class="sxs-lookup"><span data-stu-id="57e5d-148">failedCount</span></span>|<span data-ttu-id="57e5d-149">Int32</span><span class="sxs-lookup"><span data-stu-id="57e5d-149">Int32</span></span>|<span data-ttu-id="57e5d-150">失敗したユーザーの数</span><span class="sxs-lookup"><span data-stu-id="57e5d-150">Number of failed Users</span></span>|
|<span data-ttu-id="57e5d-151">conflictCount</span><span class="sxs-lookup"><span data-stu-id="57e5d-151">conflictCount</span></span>|<span data-ttu-id="57e5d-152">Int32</span><span class="sxs-lookup"><span data-stu-id="57e5d-152">Int32</span></span>|<span data-ttu-id="57e5d-153">競合しているユーザーの数</span><span class="sxs-lookup"><span data-stu-id="57e5d-153">Number of users in conflict</span></span>|
|<span data-ttu-id="57e5d-154">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="57e5d-154">lastUpdateDateTime</span></span>|<span data-ttu-id="57e5d-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="57e5d-155">DateTimeOffset</span></span>|<span data-ttu-id="57e5d-156">最終更新時刻</span><span class="sxs-lookup"><span data-stu-id="57e5d-156">Last update time</span></span>|
|<span data-ttu-id="57e5d-157">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="57e5d-157">configurationVersion</span></span>|<span data-ttu-id="57e5d-158">Int32</span><span class="sxs-lookup"><span data-stu-id="57e5d-158">Int32</span></span>|<span data-ttu-id="57e5d-159">対象の概要に関するポリシーのバージョン</span><span class="sxs-lookup"><span data-stu-id="57e5d-159">Version of the policy for that overview</span></span>|



## <a name="response"></a><span data-ttu-id="57e5d-160">応答</span><span class="sxs-lookup"><span data-stu-id="57e5d-160">Response</span></span>
<span data-ttu-id="57e5d-161">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="57e5d-161">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="57e5d-162">例</span><span class="sxs-lookup"><span data-stu-id="57e5d-162">Example</span></span>
### <a name="request"></a><span data-ttu-id="57e5d-163">要求</span><span class="sxs-lookup"><span data-stu-id="57e5d-163">Request</span></span>
<span data-ttu-id="57e5d-164">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="57e5d-164">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/userStatusOverview
Content-type: application/json
Content-length: 236

{
  "pendingCount": 12,
  "notApplicableCount": 2,
  "successCount": 12,
  "errorCount": 10,
  "failedCount": 11,
  "conflictCount": 13,
  "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
  "configurationVersion": 4
}
```

### <a name="response"></a><span data-ttu-id="57e5d-165">応答</span><span class="sxs-lookup"><span data-stu-id="57e5d-165">Response</span></span>
<span data-ttu-id="57e5d-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="57e5d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 352

{
  "@odata.type": "#microsoft.graph.deviceComplianceUserOverview",
  "id": "2d4f5bf4-5bf4-2d4f-f45b-4f2df45b4f2d",
  "pendingCount": 12,
  "notApplicableCount": 2,
  "successCount": 12,
  "errorCount": 10,
  "failedCount": 11,
  "conflictCount": 13,
  "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
  "configurationVersion": 4
}
```





