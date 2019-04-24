---
title: iosCustomConfiguration の作成
description: 新しい iosCustomConfiguration オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b19affa1478c2b40526dea48bcf1050659beedb3
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32467590"
---
# <a name="create-ioscustomconfiguration"></a><span data-ttu-id="423c4-103">iosCustomConfiguration の作成</span><span class="sxs-lookup"><span data-stu-id="423c4-103">Create iosCustomConfiguration</span></span>

> <span data-ttu-id="423c4-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="423c4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="423c4-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="423c4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="423c4-106">新しい [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="423c4-106">Create a new [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="423c4-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="423c4-107">Prerequisites</span></span>
<span data-ttu-id="423c4-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="423c4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="423c4-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="423c4-110">Permission type</span></span>|<span data-ttu-id="423c4-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="423c4-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="423c4-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="423c4-112">Delegated (work or school account)</span></span>|<span data-ttu-id="423c4-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="423c4-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="423c4-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="423c4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="423c4-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="423c4-115">Not supported.</span></span>|
|<span data-ttu-id="423c4-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="423c4-116">Application</span></span>|<span data-ttu-id="423c4-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="423c4-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="423c4-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="423c4-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="423c4-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="423c4-119">Request headers</span></span>
|<span data-ttu-id="423c4-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="423c4-120">Header</span></span>|<span data-ttu-id="423c4-121">値</span><span class="sxs-lookup"><span data-stu-id="423c4-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="423c4-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="423c4-122">Authorization</span></span>|<span data-ttu-id="423c4-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="423c4-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="423c4-124">承諾</span><span class="sxs-lookup"><span data-stu-id="423c4-124">Accept</span></span>|<span data-ttu-id="423c4-125">application/json</span><span class="sxs-lookup"><span data-stu-id="423c4-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="423c4-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="423c4-126">Request body</span></span>
<span data-ttu-id="423c4-127">要求本文で、iosCustomConfiguration オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="423c4-127">In the request body, supply a JSON representation for the iosCustomConfiguration object.</span></span>

<span data-ttu-id="423c4-128">次の表に、iosCustomConfiguration の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="423c4-128">The following table shows the properties that are required when you create the iosCustomConfiguration.</span></span>

|<span data-ttu-id="423c4-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="423c4-129">Property</span></span>|<span data-ttu-id="423c4-130">型</span><span class="sxs-lookup"><span data-stu-id="423c4-130">Type</span></span>|<span data-ttu-id="423c4-131">説明</span><span class="sxs-lookup"><span data-stu-id="423c4-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="423c4-132">id</span><span class="sxs-lookup"><span data-stu-id="423c4-132">id</span></span>|<span data-ttu-id="423c4-133">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="423c4-133">String</span></span>|<span data-ttu-id="423c4-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="423c4-134">Key of the entity.</span></span> <span data-ttu-id="423c4-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="423c4-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="423c4-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="423c4-136">lastModifiedDateTime</span></span>|<span data-ttu-id="423c4-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="423c4-137">DateTimeOffset</span></span>|<span data-ttu-id="423c4-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="423c4-138">DateTime the object was last modified.</span></span> <span data-ttu-id="423c4-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="423c4-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="423c4-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="423c4-140">roleScopeTagIds</span></span>|<span data-ttu-id="423c4-141">String collection</span><span class="sxs-lookup"><span data-stu-id="423c4-141">String collection</span></span>|<span data-ttu-id="423c4-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="423c4-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="423c4-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="423c4-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="423c4-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="423c4-144">supportsScopeTags</span></span>|<span data-ttu-id="423c4-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="423c4-145">Boolean</span></span>|<span data-ttu-id="423c4-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="423c4-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="423c4-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="423c4-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="423c4-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="423c4-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="423c4-149">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="423c4-149">This property is read-only.</span></span> <span data-ttu-id="423c4-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="423c4-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="423c4-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="423c4-151">createdDateTime</span></span>|<span data-ttu-id="423c4-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="423c4-152">DateTimeOffset</span></span>|<span data-ttu-id="423c4-153">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="423c4-153">DateTime the object was created.</span></span> <span data-ttu-id="423c4-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="423c4-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="423c4-155">説明</span><span class="sxs-lookup"><span data-stu-id="423c4-155">description</span></span>|<span data-ttu-id="423c4-156">String</span><span class="sxs-lookup"><span data-stu-id="423c4-156">String</span></span>|<span data-ttu-id="423c4-157">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="423c4-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="423c4-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="423c4-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="423c4-159">displayName</span><span class="sxs-lookup"><span data-stu-id="423c4-159">displayName</span></span>|<span data-ttu-id="423c4-160">String</span><span class="sxs-lookup"><span data-stu-id="423c4-160">String</span></span>|<span data-ttu-id="423c4-161">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="423c4-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="423c4-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="423c4-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="423c4-163">version</span><span class="sxs-lookup"><span data-stu-id="423c4-163">version</span></span>|<span data-ttu-id="423c4-164">Int32</span><span class="sxs-lookup"><span data-stu-id="423c4-164">Int32</span></span>|<span data-ttu-id="423c4-165">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="423c4-165">Version of the device configuration.</span></span> <span data-ttu-id="423c4-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="423c4-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="423c4-167">payloadName</span><span class="sxs-lookup"><span data-stu-id="423c4-167">payloadName</span></span>|<span data-ttu-id="423c4-168">String</span><span class="sxs-lookup"><span data-stu-id="423c4-168">String</span></span>|<span data-ttu-id="423c4-169">ユーザーに表示される名前。</span><span class="sxs-lookup"><span data-stu-id="423c4-169">Name that is displayed to the user.</span></span>|
|<span data-ttu-id="423c4-170">payloadFileName</span><span class="sxs-lookup"><span data-stu-id="423c4-170">payloadFileName</span></span>|<span data-ttu-id="423c4-171">String</span><span class="sxs-lookup"><span data-stu-id="423c4-171">String</span></span>|<span data-ttu-id="423c4-172">ペイロード ファイル名 (\*.mobileconfig</span><span class="sxs-lookup"><span data-stu-id="423c4-172">Payload file name (\*.mobileconfig</span></span> | <span data-ttu-id="423c4-173">\*.xml)。</span><span class="sxs-lookup"><span data-stu-id="423c4-173">\*.xml).</span></span>|
|<span data-ttu-id="423c4-174">payload</span><span class="sxs-lookup"><span data-stu-id="423c4-174">payload</span></span>|<span data-ttu-id="423c4-175">Binary</span><span class="sxs-lookup"><span data-stu-id="423c4-175">Binary</span></span>|<span data-ttu-id="423c4-176">ペイロード。</span><span class="sxs-lookup"><span data-stu-id="423c4-176">Payload.</span></span> <span data-ttu-id="423c4-177">(UTF8 でエンコードされたバイト配列)</span><span class="sxs-lookup"><span data-stu-id="423c4-177">(UTF8 encoded byte array)</span></span>|



## <a name="response"></a><span data-ttu-id="423c4-178">応答</span><span class="sxs-lookup"><span data-stu-id="423c4-178">Response</span></span>
<span data-ttu-id="423c4-179">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="423c4-179">If successful, this method returns a `201 Created` response code and a [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="423c4-180">例</span><span class="sxs-lookup"><span data-stu-id="423c4-180">Example</span></span>

### <a name="request"></a><span data-ttu-id="423c4-181">要求</span><span class="sxs-lookup"><span data-stu-id="423c4-181">Request</span></span>
<span data-ttu-id="423c4-182">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="423c4-182">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="423c4-183">応答</span><span class="sxs-lookup"><span data-stu-id="423c4-183">Response</span></span>
<span data-ttu-id="423c4-p111">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="423c4-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





