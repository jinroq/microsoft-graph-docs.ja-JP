---
title: DefaultDeviceCompliancePolicy を作成します。
description: 新しい defaultDeviceCompliancePolicy オブジェクトを作成します。
ms.openlocfilehash: 8c05cc7eedc1249175b6738ea241dea37fa5cad4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27067228"
---
# <a name="create-defaultdevicecompliancepolicy"></a><span data-ttu-id="c453c-103">DefaultDeviceCompliancePolicy を作成します。</span><span class="sxs-lookup"><span data-stu-id="c453c-103">Create defaultDeviceCompliancePolicy</span></span>

> <span data-ttu-id="c453c-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="c453c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c453c-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c453c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c453c-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="c453c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c453c-107">新しい[defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="c453c-107">Create a new [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c453c-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="c453c-108">Prerequisites</span></span>
<span data-ttu-id="c453c-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c453c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c453c-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c453c-111">Permission type</span></span>|<span data-ttu-id="c453c-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="c453c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c453c-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c453c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c453c-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c453c-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c453c-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c453c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c453c-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c453c-116">Not supported.</span></span>|
|<span data-ttu-id="c453c-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c453c-117">Application</span></span>|<span data-ttu-id="c453c-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c453c-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c453c-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c453c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="c453c-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c453c-120">Request headers</span></span>
|<span data-ttu-id="c453c-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c453c-121">Header</span></span>|<span data-ttu-id="c453c-122">値</span><span class="sxs-lookup"><span data-stu-id="c453c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c453c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c453c-123">Authorization</span></span>|<span data-ttu-id="c453c-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="c453c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c453c-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c453c-125">Accept</span></span>|<span data-ttu-id="c453c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c453c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c453c-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="c453c-127">Request body</span></span>
<span data-ttu-id="c453c-128">要求の本文に defaultDeviceCompliancePolicy オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="c453c-128">In the request body, supply a JSON representation for the defaultDeviceCompliancePolicy object.</span></span>

<span data-ttu-id="c453c-129">次の表は、defaultDeviceCompliancePolicy を作成するときに必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="c453c-129">The following table shows the properties that are required when you create the defaultDeviceCompliancePolicy.</span></span>

|<span data-ttu-id="c453c-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c453c-130">Property</span></span>|<span data-ttu-id="c453c-131">型</span><span class="sxs-lookup"><span data-stu-id="c453c-131">Type</span></span>|<span data-ttu-id="c453c-132">説明</span><span class="sxs-lookup"><span data-stu-id="c453c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c453c-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="c453c-133">roleScopeTagIds</span></span>|<span data-ttu-id="c453c-134">String コレクション</span><span class="sxs-lookup"><span data-stu-id="c453c-134">String collection</span></span>|<span data-ttu-id="c453c-135">このエンティティ インスタンスのスコープのタグのリストです。</span><span class="sxs-lookup"><span data-stu-id="c453c-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="c453c-136">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c453c-136">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="c453c-137">id</span><span class="sxs-lookup"><span data-stu-id="c453c-137">id</span></span>|<span data-ttu-id="c453c-138">String</span><span class="sxs-lookup"><span data-stu-id="c453c-138">String</span></span>|<span data-ttu-id="c453c-139">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="c453c-139">Key of the entity.</span></span> <span data-ttu-id="c453c-140">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c453c-140">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="c453c-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c453c-141">createdDateTime</span></span>|<span data-ttu-id="c453c-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c453c-142">DateTimeOffset</span></span>|<span data-ttu-id="c453c-143">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="c453c-143">DateTime the object was created.</span></span> <span data-ttu-id="c453c-144">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c453c-144">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="c453c-145">説明</span><span class="sxs-lookup"><span data-stu-id="c453c-145">description</span></span>|<span data-ttu-id="c453c-146">String</span><span class="sxs-lookup"><span data-stu-id="c453c-146">String</span></span>|<span data-ttu-id="c453c-147">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="c453c-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="c453c-148">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c453c-148">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="c453c-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c453c-149">lastModifiedDateTime</span></span>|<span data-ttu-id="c453c-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c453c-150">DateTimeOffset</span></span>|<span data-ttu-id="c453c-151">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="c453c-151">DateTime the object was last modified.</span></span> <span data-ttu-id="c453c-152">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c453c-152">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="c453c-153">displayName</span><span class="sxs-lookup"><span data-stu-id="c453c-153">displayName</span></span>|<span data-ttu-id="c453c-154">String</span><span class="sxs-lookup"><span data-stu-id="c453c-154">String</span></span>|<span data-ttu-id="c453c-155">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="c453c-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="c453c-156">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c453c-156">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="c453c-157">version</span><span class="sxs-lookup"><span data-stu-id="c453c-157">version</span></span>|<span data-ttu-id="c453c-158">Int32</span><span class="sxs-lookup"><span data-stu-id="c453c-158">Int32</span></span>|<span data-ttu-id="c453c-159">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="c453c-159">Version of the device configuration.</span></span> <span data-ttu-id="c453c-160">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c453c-160">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|



## <a name="response"></a><span data-ttu-id="c453c-161">応答</span><span class="sxs-lookup"><span data-stu-id="c453c-161">Response</span></span>
<span data-ttu-id="c453c-162">かどうかは成功すると、このメソッドが返されます、`201 Created`応答コードおよび応答の本文に[defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="c453c-162">If successful, this method returns a `201 Created` response code and a [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c453c-163">例</span><span class="sxs-lookup"><span data-stu-id="c453c-163">Example</span></span>
### <a name="request"></a><span data-ttu-id="c453c-164">要求</span><span class="sxs-lookup"><span data-stu-id="c453c-164">Request</span></span>
<span data-ttu-id="c453c-165">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="c453c-165">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies
Content-type: application/json
Content-length: 293

{
  "@odata.type": "#microsoft.graph.defaultDeviceCompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7
}
```

### <a name="response"></a><span data-ttu-id="c453c-166">応答</span><span class="sxs-lookup"><span data-stu-id="c453c-166">Response</span></span>
<span data-ttu-id="c453c-p110">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="c453c-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 401

{
  "@odata.type": "#microsoft.graph.defaultDeviceCompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "id": "a285f027-f027-a285-27f0-85a227f085a2",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7
}
```





