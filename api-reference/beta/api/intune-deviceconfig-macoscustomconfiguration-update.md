---
title: macOSCustomConfiguration の更新
description: macOSCustomConfiguration オブジェクトのプロパティを更新します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: c0fc777a86b751a187cd15b651a9bd4d352486e9
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29405164"
---
# <a name="update-macoscustomconfiguration"></a><span data-ttu-id="ae53f-103">macOSCustomConfiguration の更新</span><span class="sxs-lookup"><span data-stu-id="ae53f-103">Update macOSCustomConfiguration</span></span>

> <span data-ttu-id="ae53f-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="ae53f-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="ae53f-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ae53f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ae53f-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="ae53f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ae53f-107">[macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="ae53f-107">Update the properties of a [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ae53f-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="ae53f-108">Prerequisites</span></span>
<span data-ttu-id="ae53f-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ae53f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="ae53f-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ae53f-111">Permission type</span></span>|<span data-ttu-id="ae53f-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="ae53f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ae53f-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ae53f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ae53f-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ae53f-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ae53f-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ae53f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ae53f-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ae53f-116">Not supported.</span></span>|
|<span data-ttu-id="ae53f-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ae53f-117">Application</span></span>|<span data-ttu-id="ae53f-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ae53f-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ae53f-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ae53f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="ae53f-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ae53f-120">Request headers</span></span>
|<span data-ttu-id="ae53f-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ae53f-121">Header</span></span>|<span data-ttu-id="ae53f-122">値</span><span class="sxs-lookup"><span data-stu-id="ae53f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ae53f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ae53f-123">Authorization</span></span>|<span data-ttu-id="ae53f-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="ae53f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ae53f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ae53f-125">Accept</span></span>|<span data-ttu-id="ae53f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ae53f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ae53f-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="ae53f-127">Request body</span></span>
<span data-ttu-id="ae53f-128">要求本文で、[macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="ae53f-128">In the request body, supply a JSON representation for the [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md) object.</span></span>

<span data-ttu-id="ae53f-129">次の表に、[macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="ae53f-129">The following table shows the properties that are required when you create the [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md).</span></span>

|<span data-ttu-id="ae53f-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ae53f-130">Property</span></span>|<span data-ttu-id="ae53f-131">型</span><span class="sxs-lookup"><span data-stu-id="ae53f-131">Type</span></span>|<span data-ttu-id="ae53f-132">説明</span><span class="sxs-lookup"><span data-stu-id="ae53f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ae53f-133">id</span><span class="sxs-lookup"><span data-stu-id="ae53f-133">id</span></span>|<span data-ttu-id="ae53f-134">String</span><span class="sxs-lookup"><span data-stu-id="ae53f-134">String</span></span>|<span data-ttu-id="ae53f-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="ae53f-135">Key of the entity.</span></span> <span data-ttu-id="ae53f-136">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ae53f-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ae53f-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ae53f-137">lastModifiedDateTime</span></span>|<span data-ttu-id="ae53f-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ae53f-138">DateTimeOffset</span></span>|<span data-ttu-id="ae53f-139">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="ae53f-139">DateTime the object was last modified.</span></span> <span data-ttu-id="ae53f-140">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ae53f-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ae53f-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="ae53f-141">roleScopeTagIds</span></span>|<span data-ttu-id="ae53f-142">String コレクション</span><span class="sxs-lookup"><span data-stu-id="ae53f-142">String collection</span></span>|<span data-ttu-id="ae53f-143">このエンティティ インスタンスのスコープのタグのリストです。</span><span class="sxs-lookup"><span data-stu-id="ae53f-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="ae53f-144">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ae53f-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ae53f-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="ae53f-145">supportsScopeTags</span></span>|<span data-ttu-id="ae53f-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="ae53f-146">Boolean</span></span>|<span data-ttu-id="ae53f-147">デバイスの構成を基になるスコープのタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ae53f-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="ae53f-148">この値が false であり、エンティティをスコープ指定されたユーザーには表示されませんがある場合、ScopeTags プロパティに割り当てることは許可されていません。</span><span class="sxs-lookup"><span data-stu-id="ae53f-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="ae53f-149">これは、Silverlight で作成されたレガシ ポリシーに対して発生し、削除して、Azure ポータル内のポリシーを再作成することで解決できます。</span><span class="sxs-lookup"><span data-stu-id="ae53f-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="ae53f-150">このプロパティは読み取りのみ可能です。</span><span class="sxs-lookup"><span data-stu-id="ae53f-150">This property is read-only.</span></span> <span data-ttu-id="ae53f-151">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ae53f-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ae53f-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ae53f-152">createdDateTime</span></span>|<span data-ttu-id="ae53f-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ae53f-153">DateTimeOffset</span></span>|<span data-ttu-id="ae53f-154">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="ae53f-154">DateTime the object was created.</span></span> <span data-ttu-id="ae53f-155">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ae53f-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ae53f-156">説明</span><span class="sxs-lookup"><span data-stu-id="ae53f-156">description</span></span>|<span data-ttu-id="ae53f-157">String</span><span class="sxs-lookup"><span data-stu-id="ae53f-157">String</span></span>|<span data-ttu-id="ae53f-158">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="ae53f-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="ae53f-159">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ae53f-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ae53f-160">displayName</span><span class="sxs-lookup"><span data-stu-id="ae53f-160">displayName</span></span>|<span data-ttu-id="ae53f-161">String</span><span class="sxs-lookup"><span data-stu-id="ae53f-161">String</span></span>|<span data-ttu-id="ae53f-162">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="ae53f-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="ae53f-163">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ae53f-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ae53f-164">version</span><span class="sxs-lookup"><span data-stu-id="ae53f-164">version</span></span>|<span data-ttu-id="ae53f-165">Int32</span><span class="sxs-lookup"><span data-stu-id="ae53f-165">Int32</span></span>|<span data-ttu-id="ae53f-166">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="ae53f-166">Version of the device configuration.</span></span> <span data-ttu-id="ae53f-167">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ae53f-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ae53f-168">payloadName</span><span class="sxs-lookup"><span data-stu-id="ae53f-168">payloadName</span></span>|<span data-ttu-id="ae53f-169">String</span><span class="sxs-lookup"><span data-stu-id="ae53f-169">String</span></span>|<span data-ttu-id="ae53f-170">ユーザーに表示される名前。</span><span class="sxs-lookup"><span data-stu-id="ae53f-170">Name that is displayed to the user.</span></span>|
|<span data-ttu-id="ae53f-171">payloadFileName</span><span class="sxs-lookup"><span data-stu-id="ae53f-171">payloadFileName</span></span>|<span data-ttu-id="ae53f-172">String</span><span class="sxs-lookup"><span data-stu-id="ae53f-172">String</span></span>|<span data-ttu-id="ae53f-173">ペイロード ファイル名 (\*.mobileconfig</span><span class="sxs-lookup"><span data-stu-id="ae53f-173">Payload file name (\*.mobileconfig</span></span> | <span data-ttu-id="ae53f-174">\*.xml)。</span><span class="sxs-lookup"><span data-stu-id="ae53f-174">\*.xml).</span></span>|
|<span data-ttu-id="ae53f-175">payload</span><span class="sxs-lookup"><span data-stu-id="ae53f-175">payload</span></span>|<span data-ttu-id="ae53f-176">Binary</span><span class="sxs-lookup"><span data-stu-id="ae53f-176">Binary</span></span>|<span data-ttu-id="ae53f-177">ペイロード。</span><span class="sxs-lookup"><span data-stu-id="ae53f-177">Payload.</span></span> <span data-ttu-id="ae53f-178">(UTF8 でエンコードされたバイト配列)</span><span class="sxs-lookup"><span data-stu-id="ae53f-178">(UTF8 encoded byte array)</span></span>|



## <a name="response"></a><span data-ttu-id="ae53f-179">応答</span><span class="sxs-lookup"><span data-stu-id="ae53f-179">Response</span></span>
<span data-ttu-id="ae53f-180">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="ae53f-180">If successful, this method returns a `200 OK` response code and an updated [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ae53f-181">例</span><span class="sxs-lookup"><span data-stu-id="ae53f-181">Example</span></span>

### <a name="request"></a><span data-ttu-id="ae53f-182">要求</span><span class="sxs-lookup"><span data-stu-id="ae53f-182">Request</span></span>
<span data-ttu-id="ae53f-183">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ae53f-183">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 373

{
  "@odata.type": "#microsoft.graph.macOSCustomConfiguration",
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

### <a name="response"></a><span data-ttu-id="ae53f-184">応答</span><span class="sxs-lookup"><span data-stu-id="ae53f-184">Response</span></span>
<span data-ttu-id="ae53f-p112">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="ae53f-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 545

{
  "@odata.type": "#microsoft.graph.macOSCustomConfiguration",
  "id": "a253835d-835d-a253-5d83-53a25d8353a2",
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




