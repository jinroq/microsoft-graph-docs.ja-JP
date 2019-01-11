---
title: deviceConfigurationUserOverview の更新
description: deviceConfigurationUserOverview オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: dcb5734661093b4d6bdc8da226af1c77dd7e72f5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27812391"
---
# <a name="update-deviceconfigurationuseroverview"></a><span data-ttu-id="959e5-103">deviceConfigurationUserOverview の更新</span><span class="sxs-lookup"><span data-stu-id="959e5-103">Update deviceConfigurationUserOverview</span></span>

> <span data-ttu-id="959e5-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="959e5-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="959e5-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="959e5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="959e5-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="959e5-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="959e5-107">[deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="959e5-107">Update the properties of a [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="959e5-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="959e5-108">Prerequisites</span></span>
<span data-ttu-id="959e5-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="959e5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="959e5-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="959e5-111">Permission type</span></span>|<span data-ttu-id="959e5-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="959e5-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="959e5-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="959e5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="959e5-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="959e5-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="959e5-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="959e5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="959e5-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="959e5-116">Not supported.</span></span>|
|<span data-ttu-id="959e5-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="959e5-117">Application</span></span>|<span data-ttu-id="959e5-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="959e5-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="959e5-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="959e5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/userStatusOverview
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/rootCertificate/userStatusOverview
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/userStatusOverview
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/rootCertificate/userStatusOverview
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/rootCertificate/userStatusOverview
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSScepCertificateProfile/rootCertificate/userStatusOverview
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/userStatusOverview
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/userStatusOverview
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/userStatusOverview
```

## <a name="request-headers"></a><span data-ttu-id="959e5-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="959e5-120">Request headers</span></span>
|<span data-ttu-id="959e5-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="959e5-121">Header</span></span>|<span data-ttu-id="959e5-122">値</span><span class="sxs-lookup"><span data-stu-id="959e5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="959e5-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="959e5-123">Authorization</span></span>|<span data-ttu-id="959e5-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="959e5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="959e5-125">Accept</span><span class="sxs-lookup"><span data-stu-id="959e5-125">Accept</span></span>|<span data-ttu-id="959e5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="959e5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="959e5-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="959e5-127">Request body</span></span>
<span data-ttu-id="959e5-128">要求本文で、[deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="959e5-128">In the request body, supply a JSON representation for the [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) object.</span></span>

<span data-ttu-id="959e5-129">次の表に、[deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="959e5-129">The following table shows the properties that are required when you create the [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md).</span></span>

|<span data-ttu-id="959e5-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="959e5-130">Property</span></span>|<span data-ttu-id="959e5-131">種類</span><span class="sxs-lookup"><span data-stu-id="959e5-131">Type</span></span>|<span data-ttu-id="959e5-132">説明</span><span class="sxs-lookup"><span data-stu-id="959e5-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="959e5-133">ID</span><span class="sxs-lookup"><span data-stu-id="959e5-133">id</span></span>|<span data-ttu-id="959e5-134">String</span><span class="sxs-lookup"><span data-stu-id="959e5-134">String</span></span>|<span data-ttu-id="959e5-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="959e5-135">Key of the entity.</span></span>|
|<span data-ttu-id="959e5-136">pendingCount</span><span class="sxs-lookup"><span data-stu-id="959e5-136">pendingCount</span></span>|<span data-ttu-id="959e5-137">Int32</span><span class="sxs-lookup"><span data-stu-id="959e5-137">Int32</span></span>|<span data-ttu-id="959e5-138">保留中のユーザーの数</span><span class="sxs-lookup"><span data-stu-id="959e5-138">Number of pending Users</span></span>|
|<span data-ttu-id="959e5-139">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="959e5-139">notApplicableCount</span></span>|<span data-ttu-id="959e5-140">Int32</span><span class="sxs-lookup"><span data-stu-id="959e5-140">Int32</span></span>|<span data-ttu-id="959e5-141">適用されないユーザーの数</span><span class="sxs-lookup"><span data-stu-id="959e5-141">Number of not applicable users</span></span>|
|<span data-ttu-id="959e5-142">successCount</span><span class="sxs-lookup"><span data-stu-id="959e5-142">successCount</span></span>|<span data-ttu-id="959e5-143">Int32</span><span class="sxs-lookup"><span data-stu-id="959e5-143">Int32</span></span>|<span data-ttu-id="959e5-144">成功したユーザーの数</span><span class="sxs-lookup"><span data-stu-id="959e5-144">Number of succeeded Users</span></span>|
|<span data-ttu-id="959e5-145">errorCount</span><span class="sxs-lookup"><span data-stu-id="959e5-145">errorCount</span></span>|<span data-ttu-id="959e5-146">Int32</span><span class="sxs-lookup"><span data-stu-id="959e5-146">Int32</span></span>|<span data-ttu-id="959e5-147">エラー ユーザーの数</span><span class="sxs-lookup"><span data-stu-id="959e5-147">Number of error Users</span></span>|
|<span data-ttu-id="959e5-148">failedCount</span><span class="sxs-lookup"><span data-stu-id="959e5-148">failedCount</span></span>|<span data-ttu-id="959e5-149">Int32</span><span class="sxs-lookup"><span data-stu-id="959e5-149">Int32</span></span>|<span data-ttu-id="959e5-150">失敗したユーザーの数</span><span class="sxs-lookup"><span data-stu-id="959e5-150">Number of failed Users</span></span>|
|<span data-ttu-id="959e5-151">conflictCount</span><span class="sxs-lookup"><span data-stu-id="959e5-151">conflictCount</span></span>|<span data-ttu-id="959e5-152">Int32</span><span class="sxs-lookup"><span data-stu-id="959e5-152">Int32</span></span>|<span data-ttu-id="959e5-153">競合しているユーザーの数</span><span class="sxs-lookup"><span data-stu-id="959e5-153">Number of users in conflict</span></span>|
|<span data-ttu-id="959e5-154">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="959e5-154">lastUpdateDateTime</span></span>|<span data-ttu-id="959e5-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="959e5-155">DateTimeOffset</span></span>|<span data-ttu-id="959e5-156">最終更新時刻</span><span class="sxs-lookup"><span data-stu-id="959e5-156">Last update time</span></span>|
|<span data-ttu-id="959e5-157">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="959e5-157">configurationVersion</span></span>|<span data-ttu-id="959e5-158">Int32</span><span class="sxs-lookup"><span data-stu-id="959e5-158">Int32</span></span>|<span data-ttu-id="959e5-159">対象の概要に関するポリシーのバージョン</span><span class="sxs-lookup"><span data-stu-id="959e5-159">Version of the policy for that overview</span></span>|



## <a name="response"></a><span data-ttu-id="959e5-160">応答</span><span class="sxs-lookup"><span data-stu-id="959e5-160">Response</span></span>
<span data-ttu-id="959e5-161">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="959e5-161">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="959e5-162">例</span><span class="sxs-lookup"><span data-stu-id="959e5-162">Example</span></span>
### <a name="request"></a><span data-ttu-id="959e5-163">要求</span><span class="sxs-lookup"><span data-stu-id="959e5-163">Request</span></span>
<span data-ttu-id="959e5-164">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="959e5-164">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/userStatusOverview
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

### <a name="response"></a><span data-ttu-id="959e5-165">応答</span><span class="sxs-lookup"><span data-stu-id="959e5-165">Response</span></span>
<span data-ttu-id="959e5-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="959e5-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 355

{
  "@odata.type": "#microsoft.graph.deviceConfigurationUserOverview",
  "id": "000e52d7-52d7-000e-d752-0e00d7520e00",
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





