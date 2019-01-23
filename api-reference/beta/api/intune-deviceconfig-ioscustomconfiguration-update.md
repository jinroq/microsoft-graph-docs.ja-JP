---
title: iosCustomConfiguration の更新
description: iosCustomConfiguration オブジェクトのプロパティを更新します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 6c6a5d4e96aa05271d0cc6968df70bf8035b09c4
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29416000"
---
# <a name="update-ioscustomconfiguration"></a><span data-ttu-id="9629a-103">iosCustomConfiguration の更新</span><span class="sxs-lookup"><span data-stu-id="9629a-103">Update iosCustomConfiguration</span></span>

> <span data-ttu-id="9629a-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="9629a-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="9629a-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9629a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9629a-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="9629a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9629a-107">[iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="9629a-107">Update the properties of a [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9629a-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="9629a-108">Prerequisites</span></span>
<span data-ttu-id="9629a-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9629a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="9629a-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="9629a-111">Permission type</span></span>|<span data-ttu-id="9629a-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="9629a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9629a-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="9629a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9629a-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9629a-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9629a-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="9629a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9629a-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9629a-116">Not supported.</span></span>|
|<span data-ttu-id="9629a-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="9629a-117">Application</span></span>|<span data-ttu-id="9629a-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9629a-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9629a-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="9629a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="9629a-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9629a-120">Request headers</span></span>
|<span data-ttu-id="9629a-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9629a-121">Header</span></span>|<span data-ttu-id="9629a-122">値</span><span class="sxs-lookup"><span data-stu-id="9629a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9629a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9629a-123">Authorization</span></span>|<span data-ttu-id="9629a-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="9629a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9629a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="9629a-125">Accept</span></span>|<span data-ttu-id="9629a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9629a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9629a-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="9629a-127">Request body</span></span>
<span data-ttu-id="9629a-128">要求本文で、[iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="9629a-128">In the request body, supply a JSON representation for the [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) object.</span></span>

<span data-ttu-id="9629a-129">次の表に、[iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="9629a-129">The following table shows the properties that are required when you create the [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md).</span></span>

|<span data-ttu-id="9629a-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9629a-130">Property</span></span>|<span data-ttu-id="9629a-131">型</span><span class="sxs-lookup"><span data-stu-id="9629a-131">Type</span></span>|<span data-ttu-id="9629a-132">説明</span><span class="sxs-lookup"><span data-stu-id="9629a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9629a-133">id</span><span class="sxs-lookup"><span data-stu-id="9629a-133">id</span></span>|<span data-ttu-id="9629a-134">String</span><span class="sxs-lookup"><span data-stu-id="9629a-134">String</span></span>|<span data-ttu-id="9629a-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="9629a-135">Key of the entity.</span></span> <span data-ttu-id="9629a-136">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9629a-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9629a-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9629a-137">lastModifiedDateTime</span></span>|<span data-ttu-id="9629a-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9629a-138">DateTimeOffset</span></span>|<span data-ttu-id="9629a-139">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="9629a-139">DateTime the object was last modified.</span></span> <span data-ttu-id="9629a-140">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9629a-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9629a-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="9629a-141">roleScopeTagIds</span></span>|<span data-ttu-id="9629a-142">String コレクション</span><span class="sxs-lookup"><span data-stu-id="9629a-142">String collection</span></span>|<span data-ttu-id="9629a-143">このエンティティ インスタンスのスコープのタグのリストです。</span><span class="sxs-lookup"><span data-stu-id="9629a-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="9629a-144">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9629a-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9629a-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="9629a-145">supportsScopeTags</span></span>|<span data-ttu-id="9629a-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="9629a-146">Boolean</span></span>|<span data-ttu-id="9629a-147">デバイスの構成を基になるスコープのタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="9629a-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="9629a-148">この値が false であり、エンティティをスコープ指定されたユーザーには表示されませんがある場合、ScopeTags プロパティに割り当てることは許可されていません。</span><span class="sxs-lookup"><span data-stu-id="9629a-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="9629a-149">これは、Silverlight で作成されたレガシ ポリシーに対して発生し、削除して、Azure ポータル内のポリシーを再作成することで解決できます。</span><span class="sxs-lookup"><span data-stu-id="9629a-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="9629a-150">このプロパティは読み取りのみ可能です。</span><span class="sxs-lookup"><span data-stu-id="9629a-150">This property is read-only.</span></span> <span data-ttu-id="9629a-151">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9629a-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9629a-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9629a-152">createdDateTime</span></span>|<span data-ttu-id="9629a-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9629a-153">DateTimeOffset</span></span>|<span data-ttu-id="9629a-154">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="9629a-154">DateTime the object was created.</span></span> <span data-ttu-id="9629a-155">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9629a-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9629a-156">説明</span><span class="sxs-lookup"><span data-stu-id="9629a-156">description</span></span>|<span data-ttu-id="9629a-157">String</span><span class="sxs-lookup"><span data-stu-id="9629a-157">String</span></span>|<span data-ttu-id="9629a-158">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="9629a-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="9629a-159">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9629a-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9629a-160">displayName</span><span class="sxs-lookup"><span data-stu-id="9629a-160">displayName</span></span>|<span data-ttu-id="9629a-161">String</span><span class="sxs-lookup"><span data-stu-id="9629a-161">String</span></span>|<span data-ttu-id="9629a-162">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="9629a-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="9629a-163">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9629a-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9629a-164">version</span><span class="sxs-lookup"><span data-stu-id="9629a-164">version</span></span>|<span data-ttu-id="9629a-165">Int32</span><span class="sxs-lookup"><span data-stu-id="9629a-165">Int32</span></span>|<span data-ttu-id="9629a-166">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="9629a-166">Version of the device configuration.</span></span> <span data-ttu-id="9629a-167">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9629a-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9629a-168">payloadName</span><span class="sxs-lookup"><span data-stu-id="9629a-168">payloadName</span></span>|<span data-ttu-id="9629a-169">String</span><span class="sxs-lookup"><span data-stu-id="9629a-169">String</span></span>|<span data-ttu-id="9629a-170">ユーザーに表示される名前。</span><span class="sxs-lookup"><span data-stu-id="9629a-170">Name that is displayed to the user.</span></span>|
|<span data-ttu-id="9629a-171">payloadFileName</span><span class="sxs-lookup"><span data-stu-id="9629a-171">payloadFileName</span></span>|<span data-ttu-id="9629a-172">String</span><span class="sxs-lookup"><span data-stu-id="9629a-172">String</span></span>|<span data-ttu-id="9629a-173">ペイロード ファイル名 (\*.mobileconfig</span><span class="sxs-lookup"><span data-stu-id="9629a-173">Payload file name (\*.mobileconfig</span></span> | <span data-ttu-id="9629a-174">\*.xml)。</span><span class="sxs-lookup"><span data-stu-id="9629a-174">\*.xml).</span></span>|
|<span data-ttu-id="9629a-175">payload</span><span class="sxs-lookup"><span data-stu-id="9629a-175">payload</span></span>|<span data-ttu-id="9629a-176">Binary</span><span class="sxs-lookup"><span data-stu-id="9629a-176">Binary</span></span>|<span data-ttu-id="9629a-177">ペイロード。</span><span class="sxs-lookup"><span data-stu-id="9629a-177">Payload.</span></span> <span data-ttu-id="9629a-178">(UTF8 でエンコードされたバイト配列)</span><span class="sxs-lookup"><span data-stu-id="9629a-178">(UTF8 encoded byte array)</span></span>|



## <a name="response"></a><span data-ttu-id="9629a-179">応答</span><span class="sxs-lookup"><span data-stu-id="9629a-179">Response</span></span>
<span data-ttu-id="9629a-180">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="9629a-180">If successful, this method returns a `200 OK` response code and an updated [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9629a-181">例</span><span class="sxs-lookup"><span data-stu-id="9629a-181">Example</span></span>

### <a name="request"></a><span data-ttu-id="9629a-182">要求</span><span class="sxs-lookup"><span data-stu-id="9629a-182">Request</span></span>
<span data-ttu-id="9629a-183">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="9629a-183">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 371

{
  "@odata.type": "#microsoft.graph.iosCustomConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "payloadName": "Payload Name value",
  "payloadFileName": "Payload File Name value",
  "payload": "cGF5bG9hZA=="
}
```

### <a name="response"></a><span data-ttu-id="9629a-184">応答</span><span class="sxs-lookup"><span data-stu-id="9629a-184">Response</span></span>
<span data-ttu-id="9629a-p112">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="9629a-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 543

{
  "@odata.type": "#microsoft.graph.iosCustomConfiguration",
  "id": "f34428e3-28e3-f344-e328-44f3e32844f3",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "payloadName": "Payload Name value",
  "payloadFileName": "Payload File Name value",
  "payload": "cGF5bG9hZA=="
}
```




