---
title: DefaultDeviceCompliancePolicy を更新します。
description: DefaultDeviceCompliancePolicy オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: dae2317d87063c82739a50a15d53b59ca6adac37
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27949466"
---
# <a name="update-defaultdevicecompliancepolicy"></a><span data-ttu-id="b63e0-103">DefaultDeviceCompliancePolicy を更新します。</span><span class="sxs-lookup"><span data-stu-id="b63e0-103">Update defaultDeviceCompliancePolicy</span></span>

> <span data-ttu-id="b63e0-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="b63e0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b63e0-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b63e0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b63e0-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="b63e0-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b63e0-107">[DefaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="b63e0-107">Update the properties of a [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b63e0-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="b63e0-108">Prerequisites</span></span>
<span data-ttu-id="b63e0-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b63e0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b63e0-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b63e0-111">Permission type</span></span>|<span data-ttu-id="b63e0-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="b63e0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b63e0-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b63e0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b63e0-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b63e0-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b63e0-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b63e0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b63e0-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b63e0-116">Not supported.</span></span>|
|<span data-ttu-id="b63e0-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b63e0-117">Application</span></span>|<span data-ttu-id="b63e0-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b63e0-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b63e0-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b63e0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="b63e0-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b63e0-120">Request headers</span></span>
|<span data-ttu-id="b63e0-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b63e0-121">Header</span></span>|<span data-ttu-id="b63e0-122">値</span><span class="sxs-lookup"><span data-stu-id="b63e0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b63e0-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b63e0-123">Authorization</span></span>|<span data-ttu-id="b63e0-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="b63e0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b63e0-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b63e0-125">Accept</span></span>|<span data-ttu-id="b63e0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b63e0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b63e0-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="b63e0-127">Request body</span></span>
<span data-ttu-id="b63e0-128">要求の本文に[defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md)オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="b63e0-128">In the request body, supply a JSON representation for the [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) object.</span></span>

<span data-ttu-id="b63e0-129">[DefaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md)を作成するときに必要なプロパティを次の表に示します。</span><span class="sxs-lookup"><span data-stu-id="b63e0-129">The following table shows the properties that are required when you create the [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md).</span></span>

|<span data-ttu-id="b63e0-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b63e0-130">Property</span></span>|<span data-ttu-id="b63e0-131">種類</span><span class="sxs-lookup"><span data-stu-id="b63e0-131">Type</span></span>|<span data-ttu-id="b63e0-132">説明</span><span class="sxs-lookup"><span data-stu-id="b63e0-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b63e0-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="b63e0-133">roleScopeTagIds</span></span>|<span data-ttu-id="b63e0-134">String コレクション</span><span class="sxs-lookup"><span data-stu-id="b63e0-134">String collection</span></span>|<span data-ttu-id="b63e0-135">このエンティティ インスタンスのスコープのタグのリストです。</span><span class="sxs-lookup"><span data-stu-id="b63e0-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="b63e0-136">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b63e0-136">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="b63e0-137">id</span><span class="sxs-lookup"><span data-stu-id="b63e0-137">id</span></span>|<span data-ttu-id="b63e0-138">String</span><span class="sxs-lookup"><span data-stu-id="b63e0-138">String</span></span>|<span data-ttu-id="b63e0-139">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="b63e0-139">Key of the entity.</span></span> <span data-ttu-id="b63e0-140">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b63e0-140">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="b63e0-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b63e0-141">createdDateTime</span></span>|<span data-ttu-id="b63e0-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b63e0-142">DateTimeOffset</span></span>|<span data-ttu-id="b63e0-143">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="b63e0-143">DateTime the object was created.</span></span> <span data-ttu-id="b63e0-144">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b63e0-144">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="b63e0-145">説明</span><span class="sxs-lookup"><span data-stu-id="b63e0-145">description</span></span>|<span data-ttu-id="b63e0-146">String</span><span class="sxs-lookup"><span data-stu-id="b63e0-146">String</span></span>|<span data-ttu-id="b63e0-147">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="b63e0-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="b63e0-148">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b63e0-148">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="b63e0-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b63e0-149">lastModifiedDateTime</span></span>|<span data-ttu-id="b63e0-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b63e0-150">DateTimeOffset</span></span>|<span data-ttu-id="b63e0-151">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="b63e0-151">DateTime the object was last modified.</span></span> <span data-ttu-id="b63e0-152">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b63e0-152">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="b63e0-153">displayName</span><span class="sxs-lookup"><span data-stu-id="b63e0-153">displayName</span></span>|<span data-ttu-id="b63e0-154">String</span><span class="sxs-lookup"><span data-stu-id="b63e0-154">String</span></span>|<span data-ttu-id="b63e0-155">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="b63e0-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="b63e0-156">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b63e0-156">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="b63e0-157">version</span><span class="sxs-lookup"><span data-stu-id="b63e0-157">version</span></span>|<span data-ttu-id="b63e0-158">Int32</span><span class="sxs-lookup"><span data-stu-id="b63e0-158">Int32</span></span>|<span data-ttu-id="b63e0-159">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="b63e0-159">Version of the device configuration.</span></span> <span data-ttu-id="b63e0-160">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b63e0-160">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|



## <a name="response"></a><span data-ttu-id="b63e0-161">応答</span><span class="sxs-lookup"><span data-stu-id="b63e0-161">Response</span></span>
<span data-ttu-id="b63e0-162">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に更新された[defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="b63e0-162">If successful, this method returns a `200 OK` response code and an updated [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b63e0-163">例</span><span class="sxs-lookup"><span data-stu-id="b63e0-163">Example</span></span>
### <a name="request"></a><span data-ttu-id="b63e0-164">要求</span><span class="sxs-lookup"><span data-stu-id="b63e0-164">Request</span></span>
<span data-ttu-id="b63e0-165">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="b63e0-165">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
Content-type: application/json
Content-length: 225

{
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7
}
```

### <a name="response"></a><span data-ttu-id="b63e0-166">応答</span><span class="sxs-lookup"><span data-stu-id="b63e0-166">Response</span></span>
<span data-ttu-id="b63e0-p110">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="b63e0-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





