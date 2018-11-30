---
title: macOSDeviceFeaturesConfiguration の作成
description: 新しい macOSDeviceFeaturesConfiguration オブジェクトを作成します。
ms.openlocfilehash: 5bd8bda5b019fee81a50c117218264975883461a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27068795"
---
# <a name="create-macosdevicefeaturesconfiguration"></a><span data-ttu-id="1075b-103">macOSDeviceFeaturesConfiguration の作成</span><span class="sxs-lookup"><span data-stu-id="1075b-103">Create macOSDeviceFeaturesConfiguration</span></span>

> <span data-ttu-id="1075b-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="1075b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1075b-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1075b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1075b-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="1075b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1075b-107">新しい [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="1075b-107">Create a new [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1075b-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="1075b-108">Prerequisites</span></span>
<span data-ttu-id="1075b-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1075b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1075b-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1075b-111">Permission type</span></span>|<span data-ttu-id="1075b-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="1075b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1075b-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="1075b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1075b-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1075b-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1075b-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1075b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1075b-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1075b-116">Not supported.</span></span>|
|<span data-ttu-id="1075b-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1075b-117">Application</span></span>|<span data-ttu-id="1075b-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1075b-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1075b-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1075b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="1075b-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1075b-120">Request headers</span></span>
|<span data-ttu-id="1075b-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1075b-121">Header</span></span>|<span data-ttu-id="1075b-122">値</span><span class="sxs-lookup"><span data-stu-id="1075b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1075b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1075b-123">Authorization</span></span>|<span data-ttu-id="1075b-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="1075b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1075b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="1075b-125">Accept</span></span>|<span data-ttu-id="1075b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1075b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1075b-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="1075b-127">Request body</span></span>
<span data-ttu-id="1075b-128">要求本文で、macOSDeviceFeaturesConfiguration オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="1075b-128">In the request body, supply a JSON representation for the macOSDeviceFeaturesConfiguration object.</span></span>

<span data-ttu-id="1075b-129">次の表に、macOSDeviceFeaturesConfiguration の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="1075b-129">The following table shows the properties that are required when you create the macOSDeviceFeaturesConfiguration.</span></span>

|<span data-ttu-id="1075b-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1075b-130">Property</span></span>|<span data-ttu-id="1075b-131">型</span><span class="sxs-lookup"><span data-stu-id="1075b-131">Type</span></span>|<span data-ttu-id="1075b-132">説明</span><span class="sxs-lookup"><span data-stu-id="1075b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1075b-133">id</span><span class="sxs-lookup"><span data-stu-id="1075b-133">id</span></span>|<span data-ttu-id="1075b-134">String</span><span class="sxs-lookup"><span data-stu-id="1075b-134">String</span></span>|<span data-ttu-id="1075b-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="1075b-135">Key of the entity.</span></span> <span data-ttu-id="1075b-136">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1075b-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1075b-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1075b-137">lastModifiedDateTime</span></span>|<span data-ttu-id="1075b-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1075b-138">DateTimeOffset</span></span>|<span data-ttu-id="1075b-139">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="1075b-139">DateTime the object was last modified.</span></span> <span data-ttu-id="1075b-140">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1075b-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1075b-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="1075b-141">roleScopeTagIds</span></span>|<span data-ttu-id="1075b-142">String コレクション</span><span class="sxs-lookup"><span data-stu-id="1075b-142">String collection</span></span>|<span data-ttu-id="1075b-143">このエンティティ インスタンスのスコープのタグのリストです。</span><span class="sxs-lookup"><span data-stu-id="1075b-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="1075b-144">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1075b-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1075b-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="1075b-145">supportsScopeTags</span></span>|<span data-ttu-id="1075b-146">ブール値</span><span class="sxs-lookup"><span data-stu-id="1075b-146">Boolean</span></span>|<span data-ttu-id="1075b-147">デバイスの構成を基になるスコープのタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="1075b-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="1075b-148">この値が false であり、エンティティをスコープ指定されたユーザーには表示されませんがある場合、ScopeTags プロパティに割り当てることは許可されていません。</span><span class="sxs-lookup"><span data-stu-id="1075b-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="1075b-149">これは、Silverlight で作成されたレガシ ポリシーに対して発生し、削除して、Azure ポータル内のポリシーを再作成することで解決できます。</span><span class="sxs-lookup"><span data-stu-id="1075b-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="1075b-150">このプロパティは値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="1075b-150">This property is read-only.</span></span> <span data-ttu-id="1075b-151">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1075b-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1075b-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1075b-152">createdDateTime</span></span>|<span data-ttu-id="1075b-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1075b-153">DateTimeOffset</span></span>|<span data-ttu-id="1075b-154">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="1075b-154">DateTime the object was created.</span></span> <span data-ttu-id="1075b-155">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1075b-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1075b-156">説明</span><span class="sxs-lookup"><span data-stu-id="1075b-156">description</span></span>|<span data-ttu-id="1075b-157">String</span><span class="sxs-lookup"><span data-stu-id="1075b-157">String</span></span>|<span data-ttu-id="1075b-158">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="1075b-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="1075b-159">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1075b-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1075b-160">displayName</span><span class="sxs-lookup"><span data-stu-id="1075b-160">displayName</span></span>|<span data-ttu-id="1075b-161">String</span><span class="sxs-lookup"><span data-stu-id="1075b-161">String</span></span>|<span data-ttu-id="1075b-162">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="1075b-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="1075b-163">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1075b-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1075b-164">version</span><span class="sxs-lookup"><span data-stu-id="1075b-164">version</span></span>|<span data-ttu-id="1075b-165">Int32</span><span class="sxs-lookup"><span data-stu-id="1075b-165">Int32</span></span>|<span data-ttu-id="1075b-166">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="1075b-166">Version of the device configuration.</span></span> <span data-ttu-id="1075b-167">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1075b-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1075b-168">airPrintDestinations</span><span class="sxs-lookup"><span data-stu-id="1075b-168">airPrintDestinations</span></span>|<span data-ttu-id="1075b-169">[airPrintDestination](../resources/intune-deviceconfig-airprintdestination.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="1075b-169">[airPrintDestination](../resources/intune-deviceconfig-airprintdestination.md) collection</span></span>|<span data-ttu-id="1075b-170">常に表示されている必要があります AirPrint プリンターの配列。</span><span class="sxs-lookup"><span data-stu-id="1075b-170">An array of AirPrint printers that should always be shown.</span></span> <span data-ttu-id="1075b-171">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="1075b-171">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="1075b-172">[AppleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="1075b-172">Inherited from [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md)</span></span>|



## <a name="response"></a><span data-ttu-id="1075b-173">応答</span><span class="sxs-lookup"><span data-stu-id="1075b-173">Response</span></span>
<span data-ttu-id="1075b-174">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="1075b-174">If successful, this method returns a `201 Created` response code and a [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1075b-175">例</span><span class="sxs-lookup"><span data-stu-id="1075b-175">Example</span></span>
### <a name="request"></a><span data-ttu-id="1075b-176">要求</span><span class="sxs-lookup"><span data-stu-id="1075b-176">Request</span></span>
<span data-ttu-id="1075b-177">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="1075b-177">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 564

{
  "@odata.type": "#microsoft.graph.macOSDeviceFeaturesConfiguration",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "airPrintDestinations": [
    {
      "@odata.type": "microsoft.graph.airPrintDestination",
      "ipAddress": "Ip Address value",
      "resourcePath": "Resource Path value",
      "port": 4,
      "forceTls": true
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="1075b-178">応答</span><span class="sxs-lookup"><span data-stu-id="1075b-178">Response</span></span>
<span data-ttu-id="1075b-p112">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="1075b-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 672

{
  "@odata.type": "#microsoft.graph.macOSDeviceFeaturesConfiguration",
  "id": "49fa957d-957d-49fa-7d95-fa497d95fa49",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "airPrintDestinations": [
    {
      "@odata.type": "microsoft.graph.airPrintDestination",
      "ipAddress": "Ip Address value",
      "resourcePath": "Resource Path value",
      "port": 4,
      "forceTls": true
    }
  ]
}
```




