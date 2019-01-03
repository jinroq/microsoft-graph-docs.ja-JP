---
title: iosCustomConfiguration の作成
description: 新しい iosCustomConfiguration オブジェクトを作成します。
author: tfitzmac
ms.openlocfilehash: e22a670316ca7ffb4216c45cab5e8f3e6d7f3d65
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27343310"
---
# <a name="create-ioscustomconfiguration"></a><span data-ttu-id="1a61f-103">iosCustomConfiguration の作成</span><span class="sxs-lookup"><span data-stu-id="1a61f-103">Create iosCustomConfiguration</span></span>

> <span data-ttu-id="1a61f-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="1a61f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1a61f-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1a61f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1a61f-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="1a61f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1a61f-107">新しい [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="1a61f-107">Create a new [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1a61f-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="1a61f-108">Prerequisites</span></span>
<span data-ttu-id="1a61f-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1a61f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1a61f-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1a61f-111">Permission type</span></span>|<span data-ttu-id="1a61f-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="1a61f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1a61f-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="1a61f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1a61f-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1a61f-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1a61f-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1a61f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1a61f-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1a61f-116">Not supported.</span></span>|
|<span data-ttu-id="1a61f-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1a61f-117">Application</span></span>|<span data-ttu-id="1a61f-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1a61f-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1a61f-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1a61f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="1a61f-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1a61f-120">Request headers</span></span>
|<span data-ttu-id="1a61f-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1a61f-121">Header</span></span>|<span data-ttu-id="1a61f-122">値</span><span class="sxs-lookup"><span data-stu-id="1a61f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1a61f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1a61f-123">Authorization</span></span>|<span data-ttu-id="1a61f-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="1a61f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1a61f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="1a61f-125">Accept</span></span>|<span data-ttu-id="1a61f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1a61f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1a61f-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="1a61f-127">Request body</span></span>
<span data-ttu-id="1a61f-128">要求本文で、iosCustomConfiguration オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="1a61f-128">In the request body, supply a JSON representation for the iosCustomConfiguration object.</span></span>

<span data-ttu-id="1a61f-129">次の表に、iosCustomConfiguration の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="1a61f-129">The following table shows the properties that are required when you create the iosCustomConfiguration.</span></span>

|<span data-ttu-id="1a61f-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1a61f-130">Property</span></span>|<span data-ttu-id="1a61f-131">種類</span><span class="sxs-lookup"><span data-stu-id="1a61f-131">Type</span></span>|<span data-ttu-id="1a61f-132">説明</span><span class="sxs-lookup"><span data-stu-id="1a61f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1a61f-133">ID</span><span class="sxs-lookup"><span data-stu-id="1a61f-133">id</span></span>|<span data-ttu-id="1a61f-134">String</span><span class="sxs-lookup"><span data-stu-id="1a61f-134">String</span></span>|<span data-ttu-id="1a61f-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="1a61f-135">Key of the entity.</span></span> <span data-ttu-id="1a61f-136">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1a61f-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1a61f-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1a61f-137">lastModifiedDateTime</span></span>|<span data-ttu-id="1a61f-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1a61f-138">DateTimeOffset</span></span>|<span data-ttu-id="1a61f-139">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="1a61f-139">DateTime the object was last modified.</span></span> <span data-ttu-id="1a61f-140">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1a61f-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1a61f-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="1a61f-141">roleScopeTagIds</span></span>|<span data-ttu-id="1a61f-142">String コレクション</span><span class="sxs-lookup"><span data-stu-id="1a61f-142">String collection</span></span>|<span data-ttu-id="1a61f-143">このエンティティ インスタンスのスコープのタグのリストです。</span><span class="sxs-lookup"><span data-stu-id="1a61f-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="1a61f-144">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1a61f-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1a61f-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="1a61f-145">supportsScopeTags</span></span>|<span data-ttu-id="1a61f-146">ブール型</span><span class="sxs-lookup"><span data-stu-id="1a61f-146">Boolean</span></span>|<span data-ttu-id="1a61f-147">デバイスの構成を基になるスコープのタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="1a61f-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="1a61f-148">この値が false であり、エンティティをスコープ指定されたユーザーには表示されませんがある場合、ScopeTags プロパティに割り当てることは許可されていません。</span><span class="sxs-lookup"><span data-stu-id="1a61f-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="1a61f-149">これは、Silverlight で作成されたレガシ ポリシーに対して発生し、削除して、Azure ポータル内のポリシーを再作成することで解決できます。</span><span class="sxs-lookup"><span data-stu-id="1a61f-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="1a61f-150">このプロパティは読み取りのみ可能です。</span><span class="sxs-lookup"><span data-stu-id="1a61f-150">This property is read-only.</span></span> <span data-ttu-id="1a61f-151">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1a61f-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1a61f-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1a61f-152">createdDateTime</span></span>|<span data-ttu-id="1a61f-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1a61f-153">DateTimeOffset</span></span>|<span data-ttu-id="1a61f-154">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="1a61f-154">DateTime the object was created.</span></span> <span data-ttu-id="1a61f-155">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1a61f-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1a61f-156">説明</span><span class="sxs-lookup"><span data-stu-id="1a61f-156">description</span></span>|<span data-ttu-id="1a61f-157">String</span><span class="sxs-lookup"><span data-stu-id="1a61f-157">String</span></span>|<span data-ttu-id="1a61f-158">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="1a61f-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="1a61f-159">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1a61f-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1a61f-160">displayName</span><span class="sxs-lookup"><span data-stu-id="1a61f-160">displayName</span></span>|<span data-ttu-id="1a61f-161">String</span><span class="sxs-lookup"><span data-stu-id="1a61f-161">String</span></span>|<span data-ttu-id="1a61f-162">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="1a61f-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="1a61f-163">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1a61f-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1a61f-164">version</span><span class="sxs-lookup"><span data-stu-id="1a61f-164">version</span></span>|<span data-ttu-id="1a61f-165">Int32</span><span class="sxs-lookup"><span data-stu-id="1a61f-165">Int32</span></span>|<span data-ttu-id="1a61f-166">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="1a61f-166">Version of the device configuration.</span></span> <span data-ttu-id="1a61f-167">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1a61f-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1a61f-168">payloadName</span><span class="sxs-lookup"><span data-stu-id="1a61f-168">payloadName</span></span>|<span data-ttu-id="1a61f-169">String</span><span class="sxs-lookup"><span data-stu-id="1a61f-169">String</span></span>|<span data-ttu-id="1a61f-170">ユーザーに表示される名前。</span><span class="sxs-lookup"><span data-stu-id="1a61f-170">Name that is displayed to the user.</span></span>|
|<span data-ttu-id="1a61f-171">payloadFileName</span><span class="sxs-lookup"><span data-stu-id="1a61f-171">payloadFileName</span></span>|<span data-ttu-id="1a61f-172">String</span><span class="sxs-lookup"><span data-stu-id="1a61f-172">String</span></span>|<span data-ttu-id="1a61f-173">ペイロード ファイル名 (\*.mobileconfig</span><span class="sxs-lookup"><span data-stu-id="1a61f-173">Payload file name (\*.mobileconfig</span></span> | <span data-ttu-id="1a61f-174">\*.xml)。</span><span class="sxs-lookup"><span data-stu-id="1a61f-174">\*.xml).</span></span>|
|<span data-ttu-id="1a61f-175">payload</span><span class="sxs-lookup"><span data-stu-id="1a61f-175">payload</span></span>|<span data-ttu-id="1a61f-176">Binary</span><span class="sxs-lookup"><span data-stu-id="1a61f-176">Binary</span></span>|<span data-ttu-id="1a61f-177">ペイロード。</span><span class="sxs-lookup"><span data-stu-id="1a61f-177">Payload.</span></span> <span data-ttu-id="1a61f-178">(UTF8 でエンコードされたバイト配列)</span><span class="sxs-lookup"><span data-stu-id="1a61f-178">(UTF8 encoded byte array)</span></span>|



## <a name="response"></a><span data-ttu-id="1a61f-179">応答</span><span class="sxs-lookup"><span data-stu-id="1a61f-179">Response</span></span>
<span data-ttu-id="1a61f-180">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="1a61f-180">If successful, this method returns a `201 Created` response code and a [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1a61f-181">例</span><span class="sxs-lookup"><span data-stu-id="1a61f-181">Example</span></span>
### <a name="request"></a><span data-ttu-id="1a61f-182">要求</span><span class="sxs-lookup"><span data-stu-id="1a61f-182">Request</span></span>
<span data-ttu-id="1a61f-183">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="1a61f-183">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 435

{
  "@odata.type": "#microsoft.graph.iosCustomConfiguration",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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

### <a name="response"></a><span data-ttu-id="1a61f-184">応答</span><span class="sxs-lookup"><span data-stu-id="1a61f-184">Response</span></span>
<span data-ttu-id="1a61f-p112">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="1a61f-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




