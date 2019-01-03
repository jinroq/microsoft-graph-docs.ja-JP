---
title: deviceConfigurationDeviceStatus の作成
description: 新しい deviceConfigurationDeviceStatus オブジェクトを作成します。
author: tfitzmac
ms.openlocfilehash: 05e8280d7b4bda79feef9cd6f5055f00ee783822
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27306546"
---
# <a name="create-deviceconfigurationdevicestatus"></a><span data-ttu-id="53e1a-103">deviceConfigurationDeviceStatus の作成</span><span class="sxs-lookup"><span data-stu-id="53e1a-103">Create deviceConfigurationDeviceStatus</span></span>

> <span data-ttu-id="53e1a-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="53e1a-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="53e1a-105">新しい [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="53e1a-105">Create a new [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="53e1a-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="53e1a-106">Prerequisites</span></span>
<span data-ttu-id="53e1a-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="53e1a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="53e1a-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="53e1a-109">Permission type</span></span>|<span data-ttu-id="53e1a-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="53e1a-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="53e1a-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="53e1a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="53e1a-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="53e1a-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="53e1a-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="53e1a-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="53e1a-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="53e1a-114">Not supported.</span></span>|
|<span data-ttu-id="53e1a-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="53e1a-115">Application</span></span>|<span data-ttu-id="53e1a-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="53e1a-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="53e1a-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="53e1a-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatuses
```

## <a name="request-headers"></a><span data-ttu-id="53e1a-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="53e1a-118">Request headers</span></span>
|<span data-ttu-id="53e1a-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="53e1a-119">Header</span></span>|<span data-ttu-id="53e1a-120">値</span><span class="sxs-lookup"><span data-stu-id="53e1a-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="53e1a-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="53e1a-121">Authorization</span></span>|<span data-ttu-id="53e1a-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="53e1a-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="53e1a-123">Accept</span><span class="sxs-lookup"><span data-stu-id="53e1a-123">Accept</span></span>|<span data-ttu-id="53e1a-124">application/json</span><span class="sxs-lookup"><span data-stu-id="53e1a-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="53e1a-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="53e1a-125">Request body</span></span>
<span data-ttu-id="53e1a-126">要求本文で、deviceConfigurationDeviceStatus オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="53e1a-126">In the request body, supply a JSON representation for the deviceConfigurationDeviceStatus object.</span></span>

<span data-ttu-id="53e1a-127">次の表に、deviceConfigurationDeviceStatus の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="53e1a-127">The following table shows the properties that are required when you create the deviceConfigurationDeviceStatus.</span></span>

|<span data-ttu-id="53e1a-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="53e1a-128">Property</span></span>|<span data-ttu-id="53e1a-129">種類</span><span class="sxs-lookup"><span data-stu-id="53e1a-129">Type</span></span>|<span data-ttu-id="53e1a-130">説明</span><span class="sxs-lookup"><span data-stu-id="53e1a-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="53e1a-131">ID</span><span class="sxs-lookup"><span data-stu-id="53e1a-131">id</span></span>|<span data-ttu-id="53e1a-132">String</span><span class="sxs-lookup"><span data-stu-id="53e1a-132">String</span></span>|<span data-ttu-id="53e1a-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="53e1a-133">Key of the entity.</span></span>|
|<span data-ttu-id="53e1a-134">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="53e1a-134">deviceDisplayName</span></span>|<span data-ttu-id="53e1a-135">String</span><span class="sxs-lookup"><span data-stu-id="53e1a-135">String</span></span>|<span data-ttu-id="53e1a-136">DevicePolicyStatus のデバイス名。</span><span class="sxs-lookup"><span data-stu-id="53e1a-136">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="53e1a-137">userName</span><span class="sxs-lookup"><span data-stu-id="53e1a-137">userName</span></span>|<span data-ttu-id="53e1a-138">String</span><span class="sxs-lookup"><span data-stu-id="53e1a-138">String</span></span>|<span data-ttu-id="53e1a-139">レポートされているユーザー名</span><span class="sxs-lookup"><span data-stu-id="53e1a-139">The User Name that is being reported</span></span>|
|<span data-ttu-id="53e1a-140">deviceModel</span><span class="sxs-lookup"><span data-stu-id="53e1a-140">deviceModel</span></span>|<span data-ttu-id="53e1a-141">String</span><span class="sxs-lookup"><span data-stu-id="53e1a-141">String</span></span>|<span data-ttu-id="53e1a-142">レポートされているデバイス モデル</span><span class="sxs-lookup"><span data-stu-id="53e1a-142">The device model that is being reported</span></span>|
|<span data-ttu-id="53e1a-143">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="53e1a-143">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="53e1a-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="53e1a-144">DateTimeOffset</span></span>|<span data-ttu-id="53e1a-145">デバイス コンプライアンスの猶予期間が過ぎる DateTime</span><span class="sxs-lookup"><span data-stu-id="53e1a-145">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="53e1a-146">status</span><span class="sxs-lookup"><span data-stu-id="53e1a-146">status</span></span>|[<span data-ttu-id="53e1a-147">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="53e1a-147">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="53e1a-148">ポリシー レポートのコンプライアンスの状態。</span><span class="sxs-lookup"><span data-stu-id="53e1a-148">Compliance status of the policy report.</span></span> <span data-ttu-id="53e1a-149">可能な値は、`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned` です。</span><span class="sxs-lookup"><span data-stu-id="53e1a-149">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="53e1a-150">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="53e1a-150">lastReportedDateTime</span></span>|<span data-ttu-id="53e1a-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="53e1a-151">DateTimeOffset</span></span>|<span data-ttu-id="53e1a-152">ポリシー レポートの最終変更日時。</span><span class="sxs-lookup"><span data-stu-id="53e1a-152">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="53e1a-153">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="53e1a-153">userPrincipalName</span></span>|<span data-ttu-id="53e1a-154">String</span><span class="sxs-lookup"><span data-stu-id="53e1a-154">String</span></span>|<span data-ttu-id="53e1a-155">UserPrincipalName。</span><span class="sxs-lookup"><span data-stu-id="53e1a-155">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="53e1a-156">応答</span><span class="sxs-lookup"><span data-stu-id="53e1a-156">Response</span></span>
<span data-ttu-id="53e1a-157">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="53e1a-157">If successful, this method returns a `201 Created` response code and a [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="53e1a-158">例</span><span class="sxs-lookup"><span data-stu-id="53e1a-158">Example</span></span>
### <a name="request"></a><span data-ttu-id="53e1a-159">要求</span><span class="sxs-lookup"><span data-stu-id="53e1a-159">Request</span></span>
<span data-ttu-id="53e1a-160">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="53e1a-160">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatuses
Content-type: application/json
Content-length: 429

{
  "@odata.type": "#microsoft.graph.deviceConfigurationDeviceStatus",
  "deviceDisplayName": "Device Display Name value",
  "userName": "User Name value",
  "deviceModel": "Device Model value",
  "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="53e1a-161">応答</span><span class="sxs-lookup"><span data-stu-id="53e1a-161">Response</span></span>
<span data-ttu-id="53e1a-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="53e1a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 478

{
  "@odata.type": "#microsoft.graph.deviceConfigurationDeviceStatus",
  "id": "674e98e5-98e5-674e-e598-4e67e5984e67",
  "deviceDisplayName": "Device Display Name value",
  "userName": "User Name value",
  "deviceModel": "Device Model value",
  "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```


