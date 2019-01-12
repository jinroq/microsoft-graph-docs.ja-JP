---
title: macOSDeviceFeaturesConfiguration の更新
description: macOSDeviceFeaturesConfiguration オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 718e64382b54280ecc135ea1d651363cc44f6767
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27954065"
---
# <a name="update-macosdevicefeaturesconfiguration"></a><span data-ttu-id="1296a-103">macOSDeviceFeaturesConfiguration の更新</span><span class="sxs-lookup"><span data-stu-id="1296a-103">Update macOSDeviceFeaturesConfiguration</span></span>

> <span data-ttu-id="1296a-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="1296a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1296a-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1296a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1296a-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="1296a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1296a-107">[macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="1296a-107">Update the properties of a [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1296a-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="1296a-108">Prerequisites</span></span>
<span data-ttu-id="1296a-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1296a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1296a-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1296a-111">Permission type</span></span>|<span data-ttu-id="1296a-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="1296a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1296a-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="1296a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1296a-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1296a-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1296a-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1296a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1296a-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1296a-116">Not supported.</span></span>|
|<span data-ttu-id="1296a-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1296a-117">Application</span></span>|<span data-ttu-id="1296a-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1296a-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1296a-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1296a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="1296a-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1296a-120">Request headers</span></span>
|<span data-ttu-id="1296a-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1296a-121">Header</span></span>|<span data-ttu-id="1296a-122">値</span><span class="sxs-lookup"><span data-stu-id="1296a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1296a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1296a-123">Authorization</span></span>|<span data-ttu-id="1296a-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="1296a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1296a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="1296a-125">Accept</span></span>|<span data-ttu-id="1296a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1296a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1296a-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="1296a-127">Request body</span></span>
<span data-ttu-id="1296a-128">要求本文で、[macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="1296a-128">In the request body, supply a JSON representation for the [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) object.</span></span>

<span data-ttu-id="1296a-129">次の表に、[macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="1296a-129">The following table shows the properties that are required when you create the [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md).</span></span>

|<span data-ttu-id="1296a-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1296a-130">Property</span></span>|<span data-ttu-id="1296a-131">型</span><span class="sxs-lookup"><span data-stu-id="1296a-131">Type</span></span>|<span data-ttu-id="1296a-132">説明</span><span class="sxs-lookup"><span data-stu-id="1296a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1296a-133">ID</span><span class="sxs-lookup"><span data-stu-id="1296a-133">id</span></span>|<span data-ttu-id="1296a-134">String</span><span class="sxs-lookup"><span data-stu-id="1296a-134">String</span></span>|<span data-ttu-id="1296a-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="1296a-135">Key of the entity.</span></span> <span data-ttu-id="1296a-136">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1296a-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1296a-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1296a-137">lastModifiedDateTime</span></span>|<span data-ttu-id="1296a-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1296a-138">DateTimeOffset</span></span>|<span data-ttu-id="1296a-139">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="1296a-139">DateTime the object was last modified.</span></span> <span data-ttu-id="1296a-140">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1296a-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1296a-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="1296a-141">roleScopeTagIds</span></span>|<span data-ttu-id="1296a-142">String コレクション</span><span class="sxs-lookup"><span data-stu-id="1296a-142">String collection</span></span>|<span data-ttu-id="1296a-143">このエンティティ インスタンスのスコープのタグのリストです。</span><span class="sxs-lookup"><span data-stu-id="1296a-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="1296a-144">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1296a-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1296a-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="1296a-145">supportsScopeTags</span></span>|<span data-ttu-id="1296a-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="1296a-146">Boolean</span></span>|<span data-ttu-id="1296a-147">デバイスの構成を基になるスコープのタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="1296a-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="1296a-148">この値が false であり、エンティティをスコープ指定されたユーザーには表示されませんがある場合、ScopeTags プロパティに割り当てることは許可されていません。</span><span class="sxs-lookup"><span data-stu-id="1296a-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="1296a-149">これは、Silverlight で作成されたレガシ ポリシーに対して発生し、削除して、Azure ポータル内のポリシーを再作成することで解決できます。</span><span class="sxs-lookup"><span data-stu-id="1296a-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="1296a-150">このプロパティは読み取りのみ可能です。</span><span class="sxs-lookup"><span data-stu-id="1296a-150">This property is read-only.</span></span> <span data-ttu-id="1296a-151">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1296a-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1296a-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1296a-152">createdDateTime</span></span>|<span data-ttu-id="1296a-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1296a-153">DateTimeOffset</span></span>|<span data-ttu-id="1296a-154">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="1296a-154">DateTime the object was created.</span></span> <span data-ttu-id="1296a-155">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1296a-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1296a-156">説明</span><span class="sxs-lookup"><span data-stu-id="1296a-156">description</span></span>|<span data-ttu-id="1296a-157">String</span><span class="sxs-lookup"><span data-stu-id="1296a-157">String</span></span>|<span data-ttu-id="1296a-158">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="1296a-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="1296a-159">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1296a-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1296a-160">displayName</span><span class="sxs-lookup"><span data-stu-id="1296a-160">displayName</span></span>|<span data-ttu-id="1296a-161">String</span><span class="sxs-lookup"><span data-stu-id="1296a-161">String</span></span>|<span data-ttu-id="1296a-162">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="1296a-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="1296a-163">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1296a-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1296a-164">version</span><span class="sxs-lookup"><span data-stu-id="1296a-164">version</span></span>|<span data-ttu-id="1296a-165">Int32</span><span class="sxs-lookup"><span data-stu-id="1296a-165">Int32</span></span>|<span data-ttu-id="1296a-166">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="1296a-166">Version of the device configuration.</span></span> <span data-ttu-id="1296a-167">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1296a-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1296a-168">airPrintDestinations</span><span class="sxs-lookup"><span data-stu-id="1296a-168">airPrintDestinations</span></span>|<span data-ttu-id="1296a-169">[airPrintDestination](../resources/intune-deviceconfig-airprintdestination.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="1296a-169">[airPrintDestination](../resources/intune-deviceconfig-airprintdestination.md) collection</span></span>|<span data-ttu-id="1296a-170">常に表示されている必要があります AirPrint プリンターの配列。</span><span class="sxs-lookup"><span data-stu-id="1296a-170">An array of AirPrint printers that should always be shown.</span></span> <span data-ttu-id="1296a-171">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="1296a-171">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="1296a-172">[AppleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="1296a-172">Inherited from [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md)</span></span>|



## <a name="response"></a><span data-ttu-id="1296a-173">応答</span><span class="sxs-lookup"><span data-stu-id="1296a-173">Response</span></span>
<span data-ttu-id="1296a-174">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="1296a-174">If successful, this method returns a `200 OK` response code and an updated [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1296a-175">例</span><span class="sxs-lookup"><span data-stu-id="1296a-175">Example</span></span>
### <a name="request"></a><span data-ttu-id="1296a-176">要求</span><span class="sxs-lookup"><span data-stu-id="1296a-176">Request</span></span>
<span data-ttu-id="1296a-177">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="1296a-177">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 493

{
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

### <a name="response"></a><span data-ttu-id="1296a-178">応答</span><span class="sxs-lookup"><span data-stu-id="1296a-178">Response</span></span>
<span data-ttu-id="1296a-p112">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="1296a-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





