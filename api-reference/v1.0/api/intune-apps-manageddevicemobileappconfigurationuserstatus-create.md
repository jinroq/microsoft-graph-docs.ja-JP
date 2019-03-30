---
title: managedDeviceMobileAppConfigurationUserStatus の作成
description: 新しい managedDeviceMobileAppConfigurationUserStatus オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1b912d21fae21652d9a801443aee7e1d08446dd7
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/29/2019
ms.locfileid: "30980286"
---
# <a name="create-manageddevicemobileappconfigurationuserstatus"></a><span data-ttu-id="dac60-103">managedDeviceMobileAppConfigurationUserStatus の作成</span><span class="sxs-lookup"><span data-stu-id="dac60-103">Create managedDeviceMobileAppConfigurationUserStatus</span></span>

> <span data-ttu-id="dac60-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="dac60-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dac60-105">新しい [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="dac60-105">Create a new [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dac60-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="dac60-106">Prerequisites</span></span>
<span data-ttu-id="dac60-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="dac60-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dac60-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="dac60-109">Permission type</span></span>|<span data-ttu-id="dac60-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="dac60-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dac60-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="dac60-111">Delegated (work or school account)</span></span>|<span data-ttu-id="dac60-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dac60-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="dac60-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="dac60-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dac60-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="dac60-114">Not supported.</span></span>|
|<span data-ttu-id="dac60-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="dac60-115">Application</span></span>|<span data-ttu-id="dac60-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="dac60-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="dac60-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="dac60-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/userStatuses
```

## <a name="request-headers"></a><span data-ttu-id="dac60-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="dac60-118">Request headers</span></span>
|<span data-ttu-id="dac60-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="dac60-119">Header</span></span>|<span data-ttu-id="dac60-120">値</span><span class="sxs-lookup"><span data-stu-id="dac60-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dac60-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="dac60-121">Authorization</span></span>|<span data-ttu-id="dac60-122">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="dac60-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dac60-123">承諾</span><span class="sxs-lookup"><span data-stu-id="dac60-123">Accept</span></span>|<span data-ttu-id="dac60-124">application/json</span><span class="sxs-lookup"><span data-stu-id="dac60-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dac60-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="dac60-125">Request body</span></span>
<span data-ttu-id="dac60-126">要求本文で、managedDeviceMobileAppConfigurationUserStatus オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="dac60-126">In the request body, supply a JSON representation for the managedDeviceMobileAppConfigurationUserStatus object.</span></span>

<span data-ttu-id="dac60-127">次の表に、managedDeviceMobileAppConfigurationUserStatus の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="dac60-127">The following table shows the properties that are required when you create the managedDeviceMobileAppConfigurationUserStatus.</span></span>

|<span data-ttu-id="dac60-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="dac60-128">Property</span></span>|<span data-ttu-id="dac60-129">型</span><span class="sxs-lookup"><span data-stu-id="dac60-129">Type</span></span>|<span data-ttu-id="dac60-130">説明</span><span class="sxs-lookup"><span data-stu-id="dac60-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dac60-131">id</span><span class="sxs-lookup"><span data-stu-id="dac60-131">id</span></span>|<span data-ttu-id="dac60-132">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="dac60-132">String</span></span>|<span data-ttu-id="dac60-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="dac60-133">Key of the entity.</span></span>|
|<span data-ttu-id="dac60-134">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="dac60-134">userDisplayName</span></span>|<span data-ttu-id="dac60-135">String</span><span class="sxs-lookup"><span data-stu-id="dac60-135">String</span></span>|<span data-ttu-id="dac60-136">DevicePolicyStatus のユーザー名。</span><span class="sxs-lookup"><span data-stu-id="dac60-136">User name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="dac60-137">devicesCount</span><span class="sxs-lookup"><span data-stu-id="dac60-137">devicesCount</span></span>|<span data-ttu-id="dac60-138">Int32</span><span class="sxs-lookup"><span data-stu-id="dac60-138">Int32</span></span>|<span data-ttu-id="dac60-139">そのユーザーのデバイスの数。</span><span class="sxs-lookup"><span data-stu-id="dac60-139">Devices count for that user.</span></span>|
|<span data-ttu-id="dac60-140">status</span><span class="sxs-lookup"><span data-stu-id="dac60-140">status</span></span>|[<span data-ttu-id="dac60-141">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="dac60-141">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="dac60-142">ポリシー レポートのコンプライアンスの状態。</span><span class="sxs-lookup"><span data-stu-id="dac60-142">Compliance status of the policy report.</span></span> <span data-ttu-id="dac60-143">可能な値は、`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned` です。</span><span class="sxs-lookup"><span data-stu-id="dac60-143">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="dac60-144">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="dac60-144">lastReportedDateTime</span></span>|<span data-ttu-id="dac60-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dac60-145">DateTimeOffset</span></span>|<span data-ttu-id="dac60-146">ポリシー レポートの最終変更日時。</span><span class="sxs-lookup"><span data-stu-id="dac60-146">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="dac60-147">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="dac60-147">userPrincipalName</span></span>|<span data-ttu-id="dac60-148">String</span><span class="sxs-lookup"><span data-stu-id="dac60-148">String</span></span>|<span data-ttu-id="dac60-149">UserPrincipalName。</span><span class="sxs-lookup"><span data-stu-id="dac60-149">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="dac60-150">応答</span><span class="sxs-lookup"><span data-stu-id="dac60-150">Response</span></span>
<span data-ttu-id="dac60-151">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="dac60-151">If successful, this method returns a `201 Created` response code and a [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dac60-152">例</span><span class="sxs-lookup"><span data-stu-id="dac60-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="dac60-153">要求</span><span class="sxs-lookup"><span data-stu-id="dac60-153">Request</span></span>
<span data-ttu-id="dac60-154">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="dac60-154">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/userStatuses
Content-type: application/json
Content-length: 306

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationUserStatus",
  "userDisplayName": "User Display Name value",
  "devicesCount": 12,
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="dac60-155">応答</span><span class="sxs-lookup"><span data-stu-id="dac60-155">Response</span></span>
<span data-ttu-id="dac60-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="dac60-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 355

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationUserStatus",
  "id": "44960944-0944-4496-4409-964444099644",
  "userDisplayName": "User Display Name value",
  "devicesCount": 12,
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```



