---
title: windows10CustomConfiguration の更新
description: windows10CustomConfiguration オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 704ac214c2bc96dc21bcef2069d4bfd21c2514d1
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27865542"
---
# <a name="update-windows10customconfiguration"></a><span data-ttu-id="e99b4-103">windows10CustomConfiguration の更新</span><span class="sxs-lookup"><span data-stu-id="e99b4-103">Update windows10CustomConfiguration</span></span>

> <span data-ttu-id="e99b4-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="e99b4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e99b4-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e99b4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e99b4-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="e99b4-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e99b4-107">[windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="e99b4-107">Update the properties of a [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e99b4-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="e99b4-108">Prerequisites</span></span>
<span data-ttu-id="e99b4-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e99b4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e99b4-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e99b4-111">Permission type</span></span>|<span data-ttu-id="e99b4-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="e99b4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e99b4-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e99b4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e99b4-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e99b4-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e99b4-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e99b4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e99b4-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e99b4-116">Not supported.</span></span>|
|<span data-ttu-id="e99b4-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e99b4-117">Application</span></span>|<span data-ttu-id="e99b4-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e99b4-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e99b4-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e99b4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="e99b4-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e99b4-120">Request headers</span></span>
|<span data-ttu-id="e99b4-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e99b4-121">Header</span></span>|<span data-ttu-id="e99b4-122">値</span><span class="sxs-lookup"><span data-stu-id="e99b4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e99b4-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e99b4-123">Authorization</span></span>|<span data-ttu-id="e99b4-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="e99b4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e99b4-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e99b4-125">Accept</span></span>|<span data-ttu-id="e99b4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e99b4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e99b4-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="e99b4-127">Request body</span></span>
<span data-ttu-id="e99b4-128">要求本文で、[windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="e99b4-128">In the request body, supply a JSON representation for the [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md) object.</span></span>

<span data-ttu-id="e99b4-129">次の表に、[windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="e99b4-129">The following table shows the properties that are required when you create the [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md).</span></span>

|<span data-ttu-id="e99b4-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e99b4-130">Property</span></span>|<span data-ttu-id="e99b4-131">種類</span><span class="sxs-lookup"><span data-stu-id="e99b4-131">Type</span></span>|<span data-ttu-id="e99b4-132">説明</span><span class="sxs-lookup"><span data-stu-id="e99b4-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e99b4-133">ID</span><span class="sxs-lookup"><span data-stu-id="e99b4-133">id</span></span>|<span data-ttu-id="e99b4-134">String</span><span class="sxs-lookup"><span data-stu-id="e99b4-134">String</span></span>|<span data-ttu-id="e99b4-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="e99b4-135">Key of the entity.</span></span> <span data-ttu-id="e99b4-136">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e99b4-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e99b4-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e99b4-137">lastModifiedDateTime</span></span>|<span data-ttu-id="e99b4-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e99b4-138">DateTimeOffset</span></span>|<span data-ttu-id="e99b4-139">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="e99b4-139">DateTime the object was last modified.</span></span> <span data-ttu-id="e99b4-140">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e99b4-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e99b4-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="e99b4-141">roleScopeTagIds</span></span>|<span data-ttu-id="e99b4-142">String コレクション</span><span class="sxs-lookup"><span data-stu-id="e99b4-142">String collection</span></span>|<span data-ttu-id="e99b4-143">このエンティティ インスタンスのスコープのタグのリストです。</span><span class="sxs-lookup"><span data-stu-id="e99b4-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="e99b4-144">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e99b4-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e99b4-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="e99b4-145">supportsScopeTags</span></span>|<span data-ttu-id="e99b4-146">ブール型</span><span class="sxs-lookup"><span data-stu-id="e99b4-146">Boolean</span></span>|<span data-ttu-id="e99b4-147">デバイスの構成を基になるスコープのタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="e99b4-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="e99b4-148">この値が false であり、エンティティをスコープ指定されたユーザーには表示されませんがある場合、ScopeTags プロパティに割り当てることは許可されていません。</span><span class="sxs-lookup"><span data-stu-id="e99b4-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="e99b4-149">これは、Silverlight で作成されたレガシ ポリシーに対して発生し、削除して、Azure ポータル内のポリシーを再作成することで解決できます。</span><span class="sxs-lookup"><span data-stu-id="e99b4-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="e99b4-150">このプロパティは読み取りのみ可能です。</span><span class="sxs-lookup"><span data-stu-id="e99b4-150">This property is read-only.</span></span> <span data-ttu-id="e99b4-151">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e99b4-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e99b4-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e99b4-152">createdDateTime</span></span>|<span data-ttu-id="e99b4-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e99b4-153">DateTimeOffset</span></span>|<span data-ttu-id="e99b4-154">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="e99b4-154">DateTime the object was created.</span></span> <span data-ttu-id="e99b4-155">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e99b4-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e99b4-156">説明</span><span class="sxs-lookup"><span data-stu-id="e99b4-156">description</span></span>|<span data-ttu-id="e99b4-157">String</span><span class="sxs-lookup"><span data-stu-id="e99b4-157">String</span></span>|<span data-ttu-id="e99b4-158">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="e99b4-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="e99b4-159">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e99b4-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e99b4-160">displayName</span><span class="sxs-lookup"><span data-stu-id="e99b4-160">displayName</span></span>|<span data-ttu-id="e99b4-161">String</span><span class="sxs-lookup"><span data-stu-id="e99b4-161">String</span></span>|<span data-ttu-id="e99b4-162">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="e99b4-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="e99b4-163">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e99b4-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e99b4-164">version</span><span class="sxs-lookup"><span data-stu-id="e99b4-164">version</span></span>|<span data-ttu-id="e99b4-165">Int32</span><span class="sxs-lookup"><span data-stu-id="e99b4-165">Int32</span></span>|<span data-ttu-id="e99b4-166">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="e99b4-166">Version of the device configuration.</span></span> <span data-ttu-id="e99b4-167">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e99b4-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e99b4-168">omaSettings</span><span class="sxs-lookup"><span data-stu-id="e99b4-168">omaSettings</span></span>|<span data-ttu-id="e99b4-169">[omaSetting](../resources/intune-deviceconfig-omasetting.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="e99b4-169">[omaSetting](../resources/intune-deviceconfig-omasetting.md) collection</span></span>|<span data-ttu-id="e99b4-170">OMA 設定。</span><span class="sxs-lookup"><span data-stu-id="e99b4-170">OMA settings.</span></span> <span data-ttu-id="e99b4-171">このコレクションには、最大で 1000 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="e99b4-171">This collection can contain a maximum of 1000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="e99b4-172">応答</span><span class="sxs-lookup"><span data-stu-id="e99b4-172">Response</span></span>
<span data-ttu-id="e99b4-173">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="e99b4-173">If successful, this method returns a `200 OK` response code and an updated [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e99b4-174">例</span><span class="sxs-lookup"><span data-stu-id="e99b4-174">Example</span></span>
### <a name="request"></a><span data-ttu-id="e99b4-175">要求</span><span class="sxs-lookup"><span data-stu-id="e99b4-175">Request</span></span>
<span data-ttu-id="e99b4-176">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="e99b4-176">Here is an example of the request.</span></span>
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
  "omaSettings": [
    {
      "@odata.type": "microsoft.graph.omaSettingInteger",
      "displayName": "Display Name value",
      "description": "Description value",
      "omaUri": "Oma Uri value",
      "value": 5
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="e99b4-177">応答</span><span class="sxs-lookup"><span data-stu-id="e99b4-177">Response</span></span>
<span data-ttu-id="e99b4-p112">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="e99b4-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 668

{
  "@odata.type": "#microsoft.graph.windows10CustomConfiguration",
  "id": "d8ae266e-266e-d8ae-6e26-aed86e26aed8",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "omaSettings": [
    {
      "@odata.type": "microsoft.graph.omaSettingInteger",
      "displayName": "Display Name value",
      "description": "Description value",
      "omaUri": "Oma Uri value",
      "value": 5
    }
  ]
}
```





