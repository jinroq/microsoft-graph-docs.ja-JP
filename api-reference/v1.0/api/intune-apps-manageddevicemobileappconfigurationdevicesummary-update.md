---
title: managedDeviceMobileAppConfigurationDeviceSummary の更新
description: managedDeviceMobileAppConfigurationDeviceSummary オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: acdbe717ae96e179432ee49c9eb5fba2f5fde596
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27934388"
---
# <a name="update-manageddevicemobileappconfigurationdevicesummary"></a><span data-ttu-id="f1b7d-103">managedDeviceMobileAppConfigurationDeviceSummary の更新</span><span class="sxs-lookup"><span data-stu-id="f1b7d-103">Update managedDeviceMobileAppConfigurationDeviceSummary</span></span>

> <span data-ttu-id="f1b7d-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="f1b7d-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f1b7d-105">[managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="f1b7d-105">Update the properties of a [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f1b7d-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="f1b7d-106">Prerequisites</span></span>
<span data-ttu-id="f1b7d-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f1b7d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f1b7d-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f1b7d-109">Permission type</span></span>|<span data-ttu-id="f1b7d-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="f1b7d-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f1b7d-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f1b7d-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f1b7d-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f1b7d-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="f1b7d-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f1b7d-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f1b7d-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f1b7d-114">Not supported.</span></span>|
|<span data-ttu-id="f1b7d-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f1b7d-115">Application</span></span>|<span data-ttu-id="f1b7d-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f1b7d-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f1b7d-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f1b7d-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatusSummary
```

## <a name="request-headers"></a><span data-ttu-id="f1b7d-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f1b7d-118">Request headers</span></span>
|<span data-ttu-id="f1b7d-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f1b7d-119">Header</span></span>|<span data-ttu-id="f1b7d-120">値</span><span class="sxs-lookup"><span data-stu-id="f1b7d-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f1b7d-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="f1b7d-121">Authorization</span></span>|<span data-ttu-id="f1b7d-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="f1b7d-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f1b7d-123">Accept</span><span class="sxs-lookup"><span data-stu-id="f1b7d-123">Accept</span></span>|<span data-ttu-id="f1b7d-124">application/json</span><span class="sxs-lookup"><span data-stu-id="f1b7d-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f1b7d-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="f1b7d-125">Request body</span></span>
<span data-ttu-id="f1b7d-126">要求本文で、[managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="f1b7d-126">In the request body, supply a JSON representation for the [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) object.</span></span>

<span data-ttu-id="f1b7d-127">次の表に、[managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="f1b7d-127">The following table shows the properties that are required when you create the [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md).</span></span>

|<span data-ttu-id="f1b7d-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f1b7d-128">Property</span></span>|<span data-ttu-id="f1b7d-129">種類</span><span class="sxs-lookup"><span data-stu-id="f1b7d-129">Type</span></span>|<span data-ttu-id="f1b7d-130">説明</span><span class="sxs-lookup"><span data-stu-id="f1b7d-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f1b7d-131">ID</span><span class="sxs-lookup"><span data-stu-id="f1b7d-131">id</span></span>|<span data-ttu-id="f1b7d-132">String</span><span class="sxs-lookup"><span data-stu-id="f1b7d-132">String</span></span>|<span data-ttu-id="f1b7d-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="f1b7d-133">Key of the entity.</span></span>|
|<span data-ttu-id="f1b7d-134">pendingCount</span><span class="sxs-lookup"><span data-stu-id="f1b7d-134">pendingCount</span></span>|<span data-ttu-id="f1b7d-135">Int32</span><span class="sxs-lookup"><span data-stu-id="f1b7d-135">Int32</span></span>|<span data-ttu-id="f1b7d-136">保留中のデバイスの数</span><span class="sxs-lookup"><span data-stu-id="f1b7d-136">Number of pending devices</span></span>|
|<span data-ttu-id="f1b7d-137">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="f1b7d-137">notApplicableCount</span></span>|<span data-ttu-id="f1b7d-138">Int32</span><span class="sxs-lookup"><span data-stu-id="f1b7d-138">Int32</span></span>|<span data-ttu-id="f1b7d-139">該当しないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="f1b7d-139">Number of not applicable devices</span></span>|
|<span data-ttu-id="f1b7d-140">successCount</span><span class="sxs-lookup"><span data-stu-id="f1b7d-140">successCount</span></span>|<span data-ttu-id="f1b7d-141">Int32</span><span class="sxs-lookup"><span data-stu-id="f1b7d-141">Int32</span></span>|<span data-ttu-id="f1b7d-142">成功したデバイスの数</span><span class="sxs-lookup"><span data-stu-id="f1b7d-142">Number of succeeded devices</span></span>|
|<span data-ttu-id="f1b7d-143">errorCount</span><span class="sxs-lookup"><span data-stu-id="f1b7d-143">errorCount</span></span>|<span data-ttu-id="f1b7d-144">Int32</span><span class="sxs-lookup"><span data-stu-id="f1b7d-144">Int32</span></span>|<span data-ttu-id="f1b7d-145">エラー デバイスの数</span><span class="sxs-lookup"><span data-stu-id="f1b7d-145">Number of error devices</span></span>|
|<span data-ttu-id="f1b7d-146">failedCount</span><span class="sxs-lookup"><span data-stu-id="f1b7d-146">failedCount</span></span>|<span data-ttu-id="f1b7d-147">Int32</span><span class="sxs-lookup"><span data-stu-id="f1b7d-147">Int32</span></span>|<span data-ttu-id="f1b7d-148">失敗したデバイスの数</span><span class="sxs-lookup"><span data-stu-id="f1b7d-148">Number of failed devices</span></span>|
|<span data-ttu-id="f1b7d-149">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="f1b7d-149">lastUpdateDateTime</span></span>|<span data-ttu-id="f1b7d-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f1b7d-150">DateTimeOffset</span></span>|<span data-ttu-id="f1b7d-151">最終更新時刻</span><span class="sxs-lookup"><span data-stu-id="f1b7d-151">Last update time</span></span>|
|<span data-ttu-id="f1b7d-152">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="f1b7d-152">configurationVersion</span></span>|<span data-ttu-id="f1b7d-153">Int32</span><span class="sxs-lookup"><span data-stu-id="f1b7d-153">Int32</span></span>|<span data-ttu-id="f1b7d-154">対象の概要に関するポリシーのバージョン</span><span class="sxs-lookup"><span data-stu-id="f1b7d-154">Version of the policy for that overview</span></span>|



## <a name="response"></a><span data-ttu-id="f1b7d-155">応答</span><span class="sxs-lookup"><span data-stu-id="f1b7d-155">Response</span></span>
<span data-ttu-id="f1b7d-156">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="f1b7d-156">If successful, this method returns a `200 OK` response code and an updated [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f1b7d-157">例</span><span class="sxs-lookup"><span data-stu-id="f1b7d-157">Example</span></span>
### <a name="request"></a><span data-ttu-id="f1b7d-158">要求</span><span class="sxs-lookup"><span data-stu-id="f1b7d-158">Request</span></span>
<span data-ttu-id="f1b7d-159">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="f1b7d-159">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatusSummary
Content-type: application/json
Content-length: 299

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationDeviceSummary",
  "pendingCount": 12,
  "notApplicableCount": 2,
  "successCount": 12,
  "errorCount": 10,
  "failedCount": 11,
  "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
  "configurationVersion": 4
}
```

### <a name="response"></a><span data-ttu-id="f1b7d-160">応答</span><span class="sxs-lookup"><span data-stu-id="f1b7d-160">Response</span></span>
<span data-ttu-id="f1b7d-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="f1b7d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 348

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationDeviceSummary",
  "id": "9997c455-c455-9997-55c4-979955c49799",
  "pendingCount": 12,
  "notApplicableCount": 2,
  "successCount": 12,
  "errorCount": 10,
  "failedCount": 11,
  "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
  "configurationVersion": 4
}
```



