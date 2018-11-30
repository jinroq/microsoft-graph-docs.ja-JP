---
title: IosEducationDeviceConfiguration を作成します。
description: 新しい iosEducationDeviceConfiguration オブジェクトを作成します。
ms.openlocfilehash: 188611f92b1fa4e4e9ab3ea9fa44a057fe14e11b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27070189"
---
# <a name="create-ioseducationdeviceconfiguration"></a><span data-ttu-id="61480-103">IosEducationDeviceConfiguration を作成します。</span><span class="sxs-lookup"><span data-stu-id="61480-103">Create iosEducationDeviceConfiguration</span></span>

> <span data-ttu-id="61480-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="61480-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="61480-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="61480-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="61480-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="61480-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="61480-107">新しい[iosEducationDeviceConfiguration](../resources/intune-deviceconfig-ioseducationdeviceconfiguration.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="61480-107">Create a new [iosEducationDeviceConfiguration](../resources/intune-deviceconfig-ioseducationdeviceconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="61480-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="61480-108">Prerequisites</span></span>
<span data-ttu-id="61480-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="61480-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="61480-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="61480-111">Permission type</span></span>|<span data-ttu-id="61480-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="61480-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="61480-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="61480-113">Delegated (work or school account)</span></span>|<span data-ttu-id="61480-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="61480-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="61480-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="61480-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="61480-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="61480-116">Not supported.</span></span>|
|<span data-ttu-id="61480-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="61480-117">Application</span></span>|<span data-ttu-id="61480-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="61480-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="61480-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="61480-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="61480-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="61480-120">Request headers</span></span>
|<span data-ttu-id="61480-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="61480-121">Header</span></span>|<span data-ttu-id="61480-122">値</span><span class="sxs-lookup"><span data-stu-id="61480-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="61480-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="61480-123">Authorization</span></span>|<span data-ttu-id="61480-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="61480-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="61480-125">Accept</span><span class="sxs-lookup"><span data-stu-id="61480-125">Accept</span></span>|<span data-ttu-id="61480-126">application/json</span><span class="sxs-lookup"><span data-stu-id="61480-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="61480-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="61480-127">Request body</span></span>
<span data-ttu-id="61480-128">要求の本文に iosEducationDeviceConfiguration オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="61480-128">In the request body, supply a JSON representation for the iosEducationDeviceConfiguration object.</span></span>

<span data-ttu-id="61480-129">次の表は、iosEducationDeviceConfiguration を作成するときに必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="61480-129">The following table shows the properties that are required when you create the iosEducationDeviceConfiguration.</span></span>

|<span data-ttu-id="61480-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="61480-130">Property</span></span>|<span data-ttu-id="61480-131">型</span><span class="sxs-lookup"><span data-stu-id="61480-131">Type</span></span>|<span data-ttu-id="61480-132">説明</span><span class="sxs-lookup"><span data-stu-id="61480-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="61480-133">id</span><span class="sxs-lookup"><span data-stu-id="61480-133">id</span></span>|<span data-ttu-id="61480-134">String</span><span class="sxs-lookup"><span data-stu-id="61480-134">String</span></span>|<span data-ttu-id="61480-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="61480-135">Key of the entity.</span></span> <span data-ttu-id="61480-136">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="61480-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="61480-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="61480-137">lastModifiedDateTime</span></span>|<span data-ttu-id="61480-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="61480-138">DateTimeOffset</span></span>|<span data-ttu-id="61480-139">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="61480-139">DateTime the object was last modified.</span></span> <span data-ttu-id="61480-140">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="61480-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="61480-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="61480-141">roleScopeTagIds</span></span>|<span data-ttu-id="61480-142">String コレクション</span><span class="sxs-lookup"><span data-stu-id="61480-142">String collection</span></span>|<span data-ttu-id="61480-143">このエンティティ インスタンスのスコープのタグのリストです。</span><span class="sxs-lookup"><span data-stu-id="61480-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="61480-144">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="61480-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="61480-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="61480-145">supportsScopeTags</span></span>|<span data-ttu-id="61480-146">ブール値</span><span class="sxs-lookup"><span data-stu-id="61480-146">Boolean</span></span>|<span data-ttu-id="61480-147">デバイスの構成を基になるスコープのタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="61480-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="61480-148">この値が false であり、エンティティをスコープ指定されたユーザーには表示されませんがある場合、ScopeTags プロパティに割り当てることは許可されていません。</span><span class="sxs-lookup"><span data-stu-id="61480-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="61480-149">これは、Silverlight で作成されたレガシ ポリシーに対して発生し、削除して、Azure ポータル内のポリシーを再作成することで解決できます。</span><span class="sxs-lookup"><span data-stu-id="61480-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="61480-150">このプロパティは値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="61480-150">This property is read-only.</span></span> <span data-ttu-id="61480-151">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="61480-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="61480-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="61480-152">createdDateTime</span></span>|<span data-ttu-id="61480-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="61480-153">DateTimeOffset</span></span>|<span data-ttu-id="61480-154">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="61480-154">DateTime the object was created.</span></span> <span data-ttu-id="61480-155">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="61480-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="61480-156">説明</span><span class="sxs-lookup"><span data-stu-id="61480-156">description</span></span>|<span data-ttu-id="61480-157">String</span><span class="sxs-lookup"><span data-stu-id="61480-157">String</span></span>|<span data-ttu-id="61480-158">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="61480-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="61480-159">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="61480-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="61480-160">displayName</span><span class="sxs-lookup"><span data-stu-id="61480-160">displayName</span></span>|<span data-ttu-id="61480-161">String</span><span class="sxs-lookup"><span data-stu-id="61480-161">String</span></span>|<span data-ttu-id="61480-162">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="61480-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="61480-163">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="61480-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="61480-164">version</span><span class="sxs-lookup"><span data-stu-id="61480-164">version</span></span>|<span data-ttu-id="61480-165">Int32</span><span class="sxs-lookup"><span data-stu-id="61480-165">Int32</span></span>|<span data-ttu-id="61480-166">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="61480-166">Version of the device configuration.</span></span> <span data-ttu-id="61480-167">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="61480-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="61480-168">応答</span><span class="sxs-lookup"><span data-stu-id="61480-168">Response</span></span>
<span data-ttu-id="61480-169">かどうかは成功すると、このメソッドが返されます、`201 Created`応答コードおよび応答の本文に[iosEducationDeviceConfiguration](../resources/intune-deviceconfig-ioseducationdeviceconfiguration.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="61480-169">If successful, this method returns a `201 Created` response code and a [iosEducationDeviceConfiguration](../resources/intune-deviceconfig-ioseducationdeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="61480-170">例</span><span class="sxs-lookup"><span data-stu-id="61480-170">Example</span></span>
### <a name="request"></a><span data-ttu-id="61480-171">要求</span><span class="sxs-lookup"><span data-stu-id="61480-171">Request</span></span>
<span data-ttu-id="61480-172">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="61480-172">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 325

{
  "@odata.type": "#microsoft.graph.iosEducationDeviceConfiguration",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7
}
```

### <a name="response"></a><span data-ttu-id="61480-173">応答</span><span class="sxs-lookup"><span data-stu-id="61480-173">Response</span></span>
<span data-ttu-id="61480-p111">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="61480-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 433

{
  "@odata.type": "#microsoft.graph.iosEducationDeviceConfiguration",
  "id": "3d563be4-3be4-3d56-e43b-563de43b563d",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7
}
```




