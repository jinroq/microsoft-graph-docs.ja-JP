---
title: deviceComplianceUserOverview の更新
description: deviceComplianceUserOverview オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f5e14d46cf3d61da172a139f598c9a726458fff2
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/29/2019
ms.locfileid: "30960434"
---
# <a name="update-devicecomplianceuseroverview"></a><span data-ttu-id="ed96f-103">deviceComplianceUserOverview の更新</span><span class="sxs-lookup"><span data-stu-id="ed96f-103">Update deviceComplianceUserOverview</span></span>

> <span data-ttu-id="ed96f-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="ed96f-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ed96f-105">[deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="ed96f-105">Update the properties of a [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ed96f-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="ed96f-106">Prerequisites</span></span>
<span data-ttu-id="ed96f-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ed96f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ed96f-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ed96f-109">Permission type</span></span>|<span data-ttu-id="ed96f-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="ed96f-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ed96f-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ed96f-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ed96f-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ed96f-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ed96f-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ed96f-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ed96f-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ed96f-114">Not supported.</span></span>|
|<span data-ttu-id="ed96f-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ed96f-115">Application</span></span>|<span data-ttu-id="ed96f-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ed96f-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ed96f-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ed96f-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/userStatusOverview
```

## <a name="request-headers"></a><span data-ttu-id="ed96f-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ed96f-118">Request headers</span></span>
|<span data-ttu-id="ed96f-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ed96f-119">Header</span></span>|<span data-ttu-id="ed96f-120">値</span><span class="sxs-lookup"><span data-stu-id="ed96f-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ed96f-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="ed96f-121">Authorization</span></span>|<span data-ttu-id="ed96f-122">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="ed96f-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ed96f-123">承諾</span><span class="sxs-lookup"><span data-stu-id="ed96f-123">Accept</span></span>|<span data-ttu-id="ed96f-124">application/json</span><span class="sxs-lookup"><span data-stu-id="ed96f-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ed96f-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="ed96f-125">Request body</span></span>
<span data-ttu-id="ed96f-126">要求本文で、[deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="ed96f-126">In the request body, supply a JSON representation for the [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) object.</span></span>

<span data-ttu-id="ed96f-127">次の表に、[deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="ed96f-127">The following table shows the properties that are required when you create the [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md).</span></span>

|<span data-ttu-id="ed96f-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ed96f-128">Property</span></span>|<span data-ttu-id="ed96f-129">型</span><span class="sxs-lookup"><span data-stu-id="ed96f-129">Type</span></span>|<span data-ttu-id="ed96f-130">説明</span><span class="sxs-lookup"><span data-stu-id="ed96f-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ed96f-131">id</span><span class="sxs-lookup"><span data-stu-id="ed96f-131">id</span></span>|<span data-ttu-id="ed96f-132">String</span><span class="sxs-lookup"><span data-stu-id="ed96f-132">String</span></span>|<span data-ttu-id="ed96f-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="ed96f-133">Key of the entity.</span></span>|
|<span data-ttu-id="ed96f-134">pendingCount</span><span class="sxs-lookup"><span data-stu-id="ed96f-134">pendingCount</span></span>|<span data-ttu-id="ed96f-135">Int32</span><span class="sxs-lookup"><span data-stu-id="ed96f-135">Int32</span></span>|<span data-ttu-id="ed96f-136">保留中のユーザーの数</span><span class="sxs-lookup"><span data-stu-id="ed96f-136">Number of pending Users</span></span>|
|<span data-ttu-id="ed96f-137">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="ed96f-137">notApplicableCount</span></span>|<span data-ttu-id="ed96f-138">Int32</span><span class="sxs-lookup"><span data-stu-id="ed96f-138">Int32</span></span>|<span data-ttu-id="ed96f-139">該当しないユーザーの数</span><span class="sxs-lookup"><span data-stu-id="ed96f-139">Number of not applicable users</span></span>|
|<span data-ttu-id="ed96f-140">successCount</span><span class="sxs-lookup"><span data-stu-id="ed96f-140">successCount</span></span>|<span data-ttu-id="ed96f-141">Int32</span><span class="sxs-lookup"><span data-stu-id="ed96f-141">Int32</span></span>|<span data-ttu-id="ed96f-142">成功したユーザーの数</span><span class="sxs-lookup"><span data-stu-id="ed96f-142">Number of succeeded Users</span></span>|
|<span data-ttu-id="ed96f-143">errorCount</span><span class="sxs-lookup"><span data-stu-id="ed96f-143">errorCount</span></span>|<span data-ttu-id="ed96f-144">Int32</span><span class="sxs-lookup"><span data-stu-id="ed96f-144">Int32</span></span>|<span data-ttu-id="ed96f-145">エラー ユーザーの数</span><span class="sxs-lookup"><span data-stu-id="ed96f-145">Number of error Users</span></span>|
|<span data-ttu-id="ed96f-146">failedCount</span><span class="sxs-lookup"><span data-stu-id="ed96f-146">failedCount</span></span>|<span data-ttu-id="ed96f-147">Int32</span><span class="sxs-lookup"><span data-stu-id="ed96f-147">Int32</span></span>|<span data-ttu-id="ed96f-148">失敗したユーザーの数</span><span class="sxs-lookup"><span data-stu-id="ed96f-148">Number of failed Users</span></span>|
|<span data-ttu-id="ed96f-149">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="ed96f-149">lastUpdateDateTime</span></span>|<span data-ttu-id="ed96f-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ed96f-150">DateTimeOffset</span></span>|<span data-ttu-id="ed96f-151">最終更新時刻</span><span class="sxs-lookup"><span data-stu-id="ed96f-151">Last update time</span></span>|
|<span data-ttu-id="ed96f-152">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="ed96f-152">configurationVersion</span></span>|<span data-ttu-id="ed96f-153">Int32</span><span class="sxs-lookup"><span data-stu-id="ed96f-153">Int32</span></span>|<span data-ttu-id="ed96f-154">対象の概要に関するポリシーのバージョン</span><span class="sxs-lookup"><span data-stu-id="ed96f-154">Version of the policy for that overview</span></span>|



## <a name="response"></a><span data-ttu-id="ed96f-155">応答</span><span class="sxs-lookup"><span data-stu-id="ed96f-155">Response</span></span>
<span data-ttu-id="ed96f-156">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="ed96f-156">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ed96f-157">例</span><span class="sxs-lookup"><span data-stu-id="ed96f-157">Example</span></span>

### <a name="request"></a><span data-ttu-id="ed96f-158">要求</span><span class="sxs-lookup"><span data-stu-id="ed96f-158">Request</span></span>
<span data-ttu-id="ed96f-159">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ed96f-159">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/userStatusOverview
Content-type: application/json
Content-length: 279

{
  "@odata.type": "#microsoft.graph.deviceComplianceUserOverview",
  "pendingCount": 12,
  "notApplicableCount": 2,
  "successCount": 12,
  "errorCount": 10,
  "failedCount": 11,
  "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
  "configurationVersion": 4
}
```

### <a name="response"></a><span data-ttu-id="ed96f-160">応答</span><span class="sxs-lookup"><span data-stu-id="ed96f-160">Response</span></span>
<span data-ttu-id="ed96f-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="ed96f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 328

{
  "@odata.type": "#microsoft.graph.deviceComplianceUserOverview",
  "id": "2d4f5bf4-5bf4-2d4f-f45b-4f2df45b4f2d",
  "pendingCount": 12,
  "notApplicableCount": 2,
  "successCount": 12,
  "errorCount": 10,
  "failedCount": 11,
  "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
  "configurationVersion": 4
}
```



