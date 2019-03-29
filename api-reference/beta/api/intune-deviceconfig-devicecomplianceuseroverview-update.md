---
title: deviceComplianceUserOverview の更新
description: deviceComplianceUserOverview オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 43c519f7bae33891fc5429dcf6d83280234aebc9
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/29/2019
ms.locfileid: "30958586"
---
# <a name="update-devicecomplianceuseroverview"></a><span data-ttu-id="9b1d1-103">deviceComplianceUserOverview の更新</span><span class="sxs-lookup"><span data-stu-id="9b1d1-103">Update deviceComplianceUserOverview</span></span>

> <span data-ttu-id="9b1d1-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9b1d1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9b1d1-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="9b1d1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9b1d1-106">[deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="9b1d1-106">Update the properties of a [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9b1d1-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="9b1d1-107">Prerequisites</span></span>
<span data-ttu-id="9b1d1-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9b1d1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9b1d1-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="9b1d1-110">Permission type</span></span>|<span data-ttu-id="9b1d1-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="9b1d1-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9b1d1-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="9b1d1-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9b1d1-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9b1d1-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9b1d1-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="9b1d1-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9b1d1-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9b1d1-115">Not supported.</span></span>|
|<span data-ttu-id="9b1d1-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="9b1d1-116">Application</span></span>|<span data-ttu-id="9b1d1-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9b1d1-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9b1d1-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="9b1d1-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/userStatusOverview
```

## <a name="request-headers"></a><span data-ttu-id="9b1d1-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9b1d1-119">Request headers</span></span>
|<span data-ttu-id="9b1d1-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9b1d1-120">Header</span></span>|<span data-ttu-id="9b1d1-121">値</span><span class="sxs-lookup"><span data-stu-id="9b1d1-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9b1d1-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="9b1d1-122">Authorization</span></span>|<span data-ttu-id="9b1d1-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="9b1d1-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9b1d1-124">承諾</span><span class="sxs-lookup"><span data-stu-id="9b1d1-124">Accept</span></span>|<span data-ttu-id="9b1d1-125">application/json</span><span class="sxs-lookup"><span data-stu-id="9b1d1-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9b1d1-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="9b1d1-126">Request body</span></span>
<span data-ttu-id="9b1d1-127">要求本文で、[deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="9b1d1-127">In the request body, supply a JSON representation for the [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) object.</span></span>

<span data-ttu-id="9b1d1-128">次の表に、[deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="9b1d1-128">The following table shows the properties that are required when you create the [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md).</span></span>

|<span data-ttu-id="9b1d1-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9b1d1-129">Property</span></span>|<span data-ttu-id="9b1d1-130">型</span><span class="sxs-lookup"><span data-stu-id="9b1d1-130">Type</span></span>|<span data-ttu-id="9b1d1-131">説明</span><span class="sxs-lookup"><span data-stu-id="9b1d1-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9b1d1-132">id</span><span class="sxs-lookup"><span data-stu-id="9b1d1-132">id</span></span>|<span data-ttu-id="9b1d1-133">String</span><span class="sxs-lookup"><span data-stu-id="9b1d1-133">String</span></span>|<span data-ttu-id="9b1d1-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="9b1d1-134">Key of the entity.</span></span>|
|<span data-ttu-id="9b1d1-135">pendingCount</span><span class="sxs-lookup"><span data-stu-id="9b1d1-135">pendingCount</span></span>|<span data-ttu-id="9b1d1-136">Int32</span><span class="sxs-lookup"><span data-stu-id="9b1d1-136">Int32</span></span>|<span data-ttu-id="9b1d1-137">保留中のユーザーの数</span><span class="sxs-lookup"><span data-stu-id="9b1d1-137">Number of pending Users</span></span>|
|<span data-ttu-id="9b1d1-138">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="9b1d1-138">notApplicableCount</span></span>|<span data-ttu-id="9b1d1-139">Int32</span><span class="sxs-lookup"><span data-stu-id="9b1d1-139">Int32</span></span>|<span data-ttu-id="9b1d1-140">該当しないユーザーの数</span><span class="sxs-lookup"><span data-stu-id="9b1d1-140">Number of not applicable users</span></span>|
|<span data-ttu-id="9b1d1-141">successCount</span><span class="sxs-lookup"><span data-stu-id="9b1d1-141">successCount</span></span>|<span data-ttu-id="9b1d1-142">Int32</span><span class="sxs-lookup"><span data-stu-id="9b1d1-142">Int32</span></span>|<span data-ttu-id="9b1d1-143">成功したユーザーの数</span><span class="sxs-lookup"><span data-stu-id="9b1d1-143">Number of succeeded Users</span></span>|
|<span data-ttu-id="9b1d1-144">errorCount</span><span class="sxs-lookup"><span data-stu-id="9b1d1-144">errorCount</span></span>|<span data-ttu-id="9b1d1-145">Int32</span><span class="sxs-lookup"><span data-stu-id="9b1d1-145">Int32</span></span>|<span data-ttu-id="9b1d1-146">エラー ユーザーの数</span><span class="sxs-lookup"><span data-stu-id="9b1d1-146">Number of error Users</span></span>|
|<span data-ttu-id="9b1d1-147">failedCount</span><span class="sxs-lookup"><span data-stu-id="9b1d1-147">failedCount</span></span>|<span data-ttu-id="9b1d1-148">Int32</span><span class="sxs-lookup"><span data-stu-id="9b1d1-148">Int32</span></span>|<span data-ttu-id="9b1d1-149">失敗したユーザーの数</span><span class="sxs-lookup"><span data-stu-id="9b1d1-149">Number of failed Users</span></span>|
|<span data-ttu-id="9b1d1-150">conflictCount</span><span class="sxs-lookup"><span data-stu-id="9b1d1-150">conflictCount</span></span>|<span data-ttu-id="9b1d1-151">Int32</span><span class="sxs-lookup"><span data-stu-id="9b1d1-151">Int32</span></span>|<span data-ttu-id="9b1d1-152">競合しているユーザーの数</span><span class="sxs-lookup"><span data-stu-id="9b1d1-152">Number of users in conflict</span></span>|
|<span data-ttu-id="9b1d1-153">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="9b1d1-153">lastUpdateDateTime</span></span>|<span data-ttu-id="9b1d1-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9b1d1-154">DateTimeOffset</span></span>|<span data-ttu-id="9b1d1-155">最終更新時刻</span><span class="sxs-lookup"><span data-stu-id="9b1d1-155">Last update time</span></span>|
|<span data-ttu-id="9b1d1-156">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="9b1d1-156">configurationVersion</span></span>|<span data-ttu-id="9b1d1-157">Int32</span><span class="sxs-lookup"><span data-stu-id="9b1d1-157">Int32</span></span>|<span data-ttu-id="9b1d1-158">対象の概要に関するポリシーのバージョン</span><span class="sxs-lookup"><span data-stu-id="9b1d1-158">Version of the policy for that overview</span></span>|



## <a name="response"></a><span data-ttu-id="9b1d1-159">応答</span><span class="sxs-lookup"><span data-stu-id="9b1d1-159">Response</span></span>
<span data-ttu-id="9b1d1-160">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="9b1d1-160">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9b1d1-161">例</span><span class="sxs-lookup"><span data-stu-id="9b1d1-161">Example</span></span>

### <a name="request"></a><span data-ttu-id="9b1d1-162">要求</span><span class="sxs-lookup"><span data-stu-id="9b1d1-162">Request</span></span>
<span data-ttu-id="9b1d1-163">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="9b1d1-163">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/userStatusOverview
Content-type: application/json
Content-length: 303

{
  "@odata.type": "#microsoft.graph.deviceComplianceUserOverview",
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

### <a name="response"></a><span data-ttu-id="9b1d1-164">応答</span><span class="sxs-lookup"><span data-stu-id="9b1d1-164">Response</span></span>
<span data-ttu-id="9b1d1-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="9b1d1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




