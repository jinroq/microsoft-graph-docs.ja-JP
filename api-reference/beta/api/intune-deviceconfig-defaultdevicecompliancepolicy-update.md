---
title: defaultdevicecompliancepolicy の更新
description: defaultdevicecompliancepolicy オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 83b1c534c8b5e27e91bb6a1153f3b0a8f25496d0
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30157702"
---
# <a name="update-defaultdevicecompliancepolicy"></a><span data-ttu-id="434d1-103">defaultdevicecompliancepolicy の更新</span><span class="sxs-lookup"><span data-stu-id="434d1-103">Update defaultDeviceCompliancePolicy</span></span>

> <span data-ttu-id="434d1-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="434d1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="434d1-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="434d1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="434d1-106">[defaultdevicecompliancepolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="434d1-106">Update the properties of a [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="434d1-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="434d1-107">Prerequisites</span></span>
<span data-ttu-id="434d1-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="434d1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="434d1-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="434d1-110">Permission type</span></span>|<span data-ttu-id="434d1-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="434d1-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="434d1-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="434d1-112">Delegated (work or school account)</span></span>|<span data-ttu-id="434d1-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="434d1-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="434d1-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="434d1-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="434d1-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="434d1-115">Not supported.</span></span>|
|<span data-ttu-id="434d1-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="434d1-116">Application</span></span>|<span data-ttu-id="434d1-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="434d1-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="434d1-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="434d1-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="434d1-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="434d1-119">Request headers</span></span>
|<span data-ttu-id="434d1-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="434d1-120">Header</span></span>|<span data-ttu-id="434d1-121">値</span><span class="sxs-lookup"><span data-stu-id="434d1-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="434d1-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="434d1-122">Authorization</span></span>|<span data-ttu-id="434d1-123">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="434d1-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="434d1-124">承諾</span><span class="sxs-lookup"><span data-stu-id="434d1-124">Accept</span></span>|<span data-ttu-id="434d1-125">application/json</span><span class="sxs-lookup"><span data-stu-id="434d1-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="434d1-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="434d1-126">Request body</span></span>
<span data-ttu-id="434d1-127">要求本文で、 [defaultdevicecompliancepolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="434d1-127">In the request body, supply a JSON representation for the [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) object.</span></span>

<span data-ttu-id="434d1-128">次の表に、 [defaultdevicecompliancepolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="434d1-128">The following table shows the properties that are required when you create the [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md).</span></span>

|<span data-ttu-id="434d1-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="434d1-129">Property</span></span>|<span data-ttu-id="434d1-130">型</span><span class="sxs-lookup"><span data-stu-id="434d1-130">Type</span></span>|<span data-ttu-id="434d1-131">説明</span><span class="sxs-lookup"><span data-stu-id="434d1-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="434d1-132">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="434d1-132">roleScopeTagIds</span></span>|<span data-ttu-id="434d1-133">String collection</span><span class="sxs-lookup"><span data-stu-id="434d1-133">String collection</span></span>|<span data-ttu-id="434d1-134">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="434d1-134">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="434d1-135">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="434d1-135">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="434d1-136">id</span><span class="sxs-lookup"><span data-stu-id="434d1-136">id</span></span>|<span data-ttu-id="434d1-137">文字列</span><span class="sxs-lookup"><span data-stu-id="434d1-137">String</span></span>|<span data-ttu-id="434d1-138">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="434d1-138">Key of the entity.</span></span> <span data-ttu-id="434d1-139">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="434d1-139">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="434d1-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="434d1-140">createdDateTime</span></span>|<span data-ttu-id="434d1-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="434d1-141">DateTimeOffset</span></span>|<span data-ttu-id="434d1-142">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="434d1-142">DateTime the object was created.</span></span> <span data-ttu-id="434d1-143">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="434d1-143">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="434d1-144">説明</span><span class="sxs-lookup"><span data-stu-id="434d1-144">description</span></span>|<span data-ttu-id="434d1-145">String</span><span class="sxs-lookup"><span data-stu-id="434d1-145">String</span></span>|<span data-ttu-id="434d1-146">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="434d1-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="434d1-147">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="434d1-147">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="434d1-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="434d1-148">lastModifiedDateTime</span></span>|<span data-ttu-id="434d1-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="434d1-149">DateTimeOffset</span></span>|<span data-ttu-id="434d1-150">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="434d1-150">DateTime the object was last modified.</span></span> <span data-ttu-id="434d1-151">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="434d1-151">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="434d1-152">displayName</span><span class="sxs-lookup"><span data-stu-id="434d1-152">displayName</span></span>|<span data-ttu-id="434d1-153">String</span><span class="sxs-lookup"><span data-stu-id="434d1-153">String</span></span>|<span data-ttu-id="434d1-154">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="434d1-154">Admin provided name of the device configuration.</span></span> <span data-ttu-id="434d1-155">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="434d1-155">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="434d1-156">version</span><span class="sxs-lookup"><span data-stu-id="434d1-156">version</span></span>|<span data-ttu-id="434d1-157">Int32</span><span class="sxs-lookup"><span data-stu-id="434d1-157">Int32</span></span>|<span data-ttu-id="434d1-158">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="434d1-158">Version of the device configuration.</span></span> <span data-ttu-id="434d1-159">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="434d1-159">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|



## <a name="response"></a><span data-ttu-id="434d1-160">応答</span><span class="sxs-lookup"><span data-stu-id="434d1-160">Response</span></span>
<span data-ttu-id="434d1-161">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[defaultdevicecompliancepolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="434d1-161">If successful, this method returns a `200 OK` response code and an updated [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="434d1-162">例</span><span class="sxs-lookup"><span data-stu-id="434d1-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="434d1-163">要求</span><span class="sxs-lookup"><span data-stu-id="434d1-163">Request</span></span>
<span data-ttu-id="434d1-164">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="434d1-164">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
Content-type: application/json
Content-length: 229

{
  "@odata.type": "#microsoft.graph.defaultDeviceCompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7
}
```

### <a name="response"></a><span data-ttu-id="434d1-165">応答</span><span class="sxs-lookup"><span data-stu-id="434d1-165">Response</span></span>
<span data-ttu-id="434d1-p109">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="434d1-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




