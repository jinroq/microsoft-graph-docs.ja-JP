---
title: managedDeviceMobileAppConfigurationUserSummary の更新
description: managedDeviceMobileAppConfigurationUserSummary オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b5789ce7e4daca6719fa106159f03157a6a0469a
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30260950"
---
# <a name="update-manageddevicemobileappconfigurationusersummary"></a><span data-ttu-id="a32cd-103">managedDeviceMobileAppConfigurationUserSummary の更新</span><span class="sxs-lookup"><span data-stu-id="a32cd-103">Update managedDeviceMobileAppConfigurationUserSummary</span></span>

> <span data-ttu-id="a32cd-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="a32cd-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a32cd-105">[managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="a32cd-105">Update the properties of a [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a32cd-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="a32cd-106">Prerequisites</span></span>
<span data-ttu-id="a32cd-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a32cd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="a32cd-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a32cd-109">Permission type</span></span>|<span data-ttu-id="a32cd-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="a32cd-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a32cd-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a32cd-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a32cd-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a32cd-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="a32cd-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a32cd-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a32cd-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a32cd-114">Not supported.</span></span>|
|<span data-ttu-id="a32cd-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a32cd-115">Application</span></span>|<span data-ttu-id="a32cd-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a32cd-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a32cd-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a32cd-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/userStatusSummary
```

## <a name="request-headers"></a><span data-ttu-id="a32cd-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a32cd-118">Request headers</span></span>
|<span data-ttu-id="a32cd-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a32cd-119">Header</span></span>|<span data-ttu-id="a32cd-120">値</span><span class="sxs-lookup"><span data-stu-id="a32cd-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a32cd-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="a32cd-121">Authorization</span></span>|<span data-ttu-id="a32cd-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="a32cd-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a32cd-123">承諾</span><span class="sxs-lookup"><span data-stu-id="a32cd-123">Accept</span></span>|<span data-ttu-id="a32cd-124">application/json</span><span class="sxs-lookup"><span data-stu-id="a32cd-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a32cd-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="a32cd-125">Request body</span></span>
<span data-ttu-id="a32cd-126">要求本文で、[managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="a32cd-126">In the request body, supply a JSON representation for the [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) object.</span></span>

<span data-ttu-id="a32cd-127">次の表に、[managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="a32cd-127">The following table shows the properties that are required when you create the [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md).</span></span>

|<span data-ttu-id="a32cd-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a32cd-128">Property</span></span>|<span data-ttu-id="a32cd-129">型</span><span class="sxs-lookup"><span data-stu-id="a32cd-129">Type</span></span>|<span data-ttu-id="a32cd-130">説明</span><span class="sxs-lookup"><span data-stu-id="a32cd-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a32cd-131">id</span><span class="sxs-lookup"><span data-stu-id="a32cd-131">id</span></span>|<span data-ttu-id="a32cd-132">String</span><span class="sxs-lookup"><span data-stu-id="a32cd-132">String</span></span>|<span data-ttu-id="a32cd-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="a32cd-133">Key of the entity.</span></span>|
|<span data-ttu-id="a32cd-134">pendingCount</span><span class="sxs-lookup"><span data-stu-id="a32cd-134">pendingCount</span></span>|<span data-ttu-id="a32cd-135">Int32</span><span class="sxs-lookup"><span data-stu-id="a32cd-135">Int32</span></span>|<span data-ttu-id="a32cd-136">保留中のユーザーの数</span><span class="sxs-lookup"><span data-stu-id="a32cd-136">Number of pending Users</span></span>|
|<span data-ttu-id="a32cd-137">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="a32cd-137">notApplicableCount</span></span>|<span data-ttu-id="a32cd-138">Int32</span><span class="sxs-lookup"><span data-stu-id="a32cd-138">Int32</span></span>|<span data-ttu-id="a32cd-139">該当しないユーザーの数</span><span class="sxs-lookup"><span data-stu-id="a32cd-139">Number of not applicable users</span></span>|
|<span data-ttu-id="a32cd-140">successCount</span><span class="sxs-lookup"><span data-stu-id="a32cd-140">successCount</span></span>|<span data-ttu-id="a32cd-141">Int32</span><span class="sxs-lookup"><span data-stu-id="a32cd-141">Int32</span></span>|<span data-ttu-id="a32cd-142">成功したユーザーの数</span><span class="sxs-lookup"><span data-stu-id="a32cd-142">Number of succeeded Users</span></span>|
|<span data-ttu-id="a32cd-143">errorCount</span><span class="sxs-lookup"><span data-stu-id="a32cd-143">errorCount</span></span>|<span data-ttu-id="a32cd-144">Int32</span><span class="sxs-lookup"><span data-stu-id="a32cd-144">Int32</span></span>|<span data-ttu-id="a32cd-145">エラー ユーザーの数</span><span class="sxs-lookup"><span data-stu-id="a32cd-145">Number of error Users</span></span>|
|<span data-ttu-id="a32cd-146">failedCount</span><span class="sxs-lookup"><span data-stu-id="a32cd-146">failedCount</span></span>|<span data-ttu-id="a32cd-147">Int32</span><span class="sxs-lookup"><span data-stu-id="a32cd-147">Int32</span></span>|<span data-ttu-id="a32cd-148">失敗したユーザーの数</span><span class="sxs-lookup"><span data-stu-id="a32cd-148">Number of failed Users</span></span>|
|<span data-ttu-id="a32cd-149">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="a32cd-149">lastUpdateDateTime</span></span>|<span data-ttu-id="a32cd-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a32cd-150">DateTimeOffset</span></span>|<span data-ttu-id="a32cd-151">最終更新時刻</span><span class="sxs-lookup"><span data-stu-id="a32cd-151">Last update time</span></span>|
|<span data-ttu-id="a32cd-152">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="a32cd-152">configurationVersion</span></span>|<span data-ttu-id="a32cd-153">Int32</span><span class="sxs-lookup"><span data-stu-id="a32cd-153">Int32</span></span>|<span data-ttu-id="a32cd-154">対象の概要に関するポリシーのバージョン</span><span class="sxs-lookup"><span data-stu-id="a32cd-154">Version of the policy for that overview</span></span>|



## <a name="response"></a><span data-ttu-id="a32cd-155">応答</span><span class="sxs-lookup"><span data-stu-id="a32cd-155">Response</span></span>
<span data-ttu-id="a32cd-156">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="a32cd-156">If successful, this method returns a `200 OK` response code and an updated [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a32cd-157">例</span><span class="sxs-lookup"><span data-stu-id="a32cd-157">Example</span></span>

### <a name="request"></a><span data-ttu-id="a32cd-158">要求</span><span class="sxs-lookup"><span data-stu-id="a32cd-158">Request</span></span>
<span data-ttu-id="a32cd-159">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="a32cd-159">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/userStatusSummary
Content-type: application/json
Content-length: 297

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationUserSummary",
  "pendingCount": 12,
  "notApplicableCount": 2,
  "successCount": 12,
  "errorCount": 10,
  "failedCount": 11,
  "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
  "configurationVersion": 4
}
```

### <a name="response"></a><span data-ttu-id="a32cd-160">応答</span><span class="sxs-lookup"><span data-stu-id="a32cd-160">Response</span></span>
<span data-ttu-id="a32cd-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="a32cd-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 346

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationUserSummary",
  "id": "7b953742-3742-7b95-4237-957b4237957b",
  "pendingCount": 12,
  "notApplicableCount": 2,
  "successCount": 12,
  "errorCount": 10,
  "failedCount": 11,
  "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
  "configurationVersion": 4
}
```



