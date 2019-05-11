---
title: windowsPhone81CustomConfiguration の作成
description: 新しい windowsPhone81CustomConfiguration オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 648a4906125b4d7282a8614e3ebea741c481258f
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33917822"
---
# <a name="create-windowsphone81customconfiguration"></a><span data-ttu-id="8631f-103">windowsPhone81CustomConfiguration の作成</span><span class="sxs-lookup"><span data-stu-id="8631f-103">Create windowsPhone81CustomConfiguration</span></span>

> <span data-ttu-id="8631f-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8631f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8631f-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="8631f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8631f-106">新しい [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="8631f-106">Create a new [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8631f-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="8631f-107">Prerequisites</span></span>
<span data-ttu-id="8631f-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8631f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8631f-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8631f-110">Permission type</span></span>|<span data-ttu-id="8631f-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="8631f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8631f-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="8631f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8631f-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8631f-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8631f-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8631f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8631f-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8631f-115">Not supported.</span></span>|
|<span data-ttu-id="8631f-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8631f-116">Application</span></span>|<span data-ttu-id="8631f-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8631f-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8631f-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8631f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="8631f-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8631f-119">Request headers</span></span>
|<span data-ttu-id="8631f-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8631f-120">Header</span></span>|<span data-ttu-id="8631f-121">値</span><span class="sxs-lookup"><span data-stu-id="8631f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8631f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="8631f-122">Authorization</span></span>|<span data-ttu-id="8631f-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="8631f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8631f-124">承諾</span><span class="sxs-lookup"><span data-stu-id="8631f-124">Accept</span></span>|<span data-ttu-id="8631f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="8631f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8631f-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="8631f-126">Request body</span></span>
<span data-ttu-id="8631f-127">要求本文で、windowsPhone81CustomConfiguration オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="8631f-127">In the request body, supply a JSON representation for the windowsPhone81CustomConfiguration object.</span></span>

<span data-ttu-id="8631f-128">次の表に、windowsPhone81CustomConfiguration の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="8631f-128">The following table shows the properties that are required when you create the windowsPhone81CustomConfiguration.</span></span>

|<span data-ttu-id="8631f-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8631f-129">Property</span></span>|<span data-ttu-id="8631f-130">型</span><span class="sxs-lookup"><span data-stu-id="8631f-130">Type</span></span>|<span data-ttu-id="8631f-131">説明</span><span class="sxs-lookup"><span data-stu-id="8631f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8631f-132">id</span><span class="sxs-lookup"><span data-stu-id="8631f-132">id</span></span>|<span data-ttu-id="8631f-133">文字列</span><span class="sxs-lookup"><span data-stu-id="8631f-133">String</span></span>|<span data-ttu-id="8631f-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="8631f-134">Key of the entity.</span></span> <span data-ttu-id="8631f-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8631f-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8631f-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8631f-136">lastModifiedDateTime</span></span>|<span data-ttu-id="8631f-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8631f-137">DateTimeOffset</span></span>|<span data-ttu-id="8631f-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="8631f-138">DateTime the object was last modified.</span></span> <span data-ttu-id="8631f-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8631f-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8631f-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="8631f-140">roleScopeTagIds</span></span>|<span data-ttu-id="8631f-141">String collection</span><span class="sxs-lookup"><span data-stu-id="8631f-141">String collection</span></span>|<span data-ttu-id="8631f-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="8631f-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="8631f-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8631f-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8631f-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="8631f-144">supportsScopeTags</span></span>|<span data-ttu-id="8631f-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="8631f-145">Boolean</span></span>|<span data-ttu-id="8631f-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="8631f-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="8631f-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="8631f-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="8631f-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="8631f-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="8631f-149">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="8631f-149">This property is read-only.</span></span> <span data-ttu-id="8631f-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8631f-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8631f-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8631f-151">createdDateTime</span></span>|<span data-ttu-id="8631f-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8631f-152">DateTimeOffset</span></span>|<span data-ttu-id="8631f-153">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="8631f-153">DateTime the object was created.</span></span> <span data-ttu-id="8631f-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8631f-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8631f-155">description</span><span class="sxs-lookup"><span data-stu-id="8631f-155">description</span></span>|<span data-ttu-id="8631f-156">String</span><span class="sxs-lookup"><span data-stu-id="8631f-156">String</span></span>|<span data-ttu-id="8631f-157">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="8631f-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="8631f-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8631f-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8631f-159">displayName</span><span class="sxs-lookup"><span data-stu-id="8631f-159">displayName</span></span>|<span data-ttu-id="8631f-160">String</span><span class="sxs-lookup"><span data-stu-id="8631f-160">String</span></span>|<span data-ttu-id="8631f-161">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="8631f-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="8631f-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8631f-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8631f-163">version</span><span class="sxs-lookup"><span data-stu-id="8631f-163">version</span></span>|<span data-ttu-id="8631f-164">Int32</span><span class="sxs-lookup"><span data-stu-id="8631f-164">Int32</span></span>|<span data-ttu-id="8631f-165">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="8631f-165">Version of the device configuration.</span></span> <span data-ttu-id="8631f-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8631f-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8631f-167">omaSettings</span><span class="sxs-lookup"><span data-stu-id="8631f-167">omaSettings</span></span>|<span data-ttu-id="8631f-168">[omaSetting](../resources/intune-deviceconfig-omasetting.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="8631f-168">[omaSetting](../resources/intune-deviceconfig-omasetting.md) collection</span></span>|<span data-ttu-id="8631f-169">OMA 設定。</span><span class="sxs-lookup"><span data-stu-id="8631f-169">OMA settings.</span></span> <span data-ttu-id="8631f-170">このコレクションには、最大で 1000 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="8631f-170">This collection can contain a maximum of 1000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="8631f-171">応答</span><span class="sxs-lookup"><span data-stu-id="8631f-171">Response</span></span>
<span data-ttu-id="8631f-172">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="8631f-172">If successful, this method returns a `201 Created` response code and a [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8631f-173">例</span><span class="sxs-lookup"><span data-stu-id="8631f-173">Example</span></span>

### <a name="request"></a><span data-ttu-id="8631f-174">要求</span><span class="sxs-lookup"><span data-stu-id="8631f-174">Request</span></span>
<span data-ttu-id="8631f-175">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="8631f-175">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 501

{
  "@odata.type": "#microsoft.graph.windowsPhone81CustomConfiguration",
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

### <a name="response"></a><span data-ttu-id="8631f-176">応答</span><span class="sxs-lookup"><span data-stu-id="8631f-176">Response</span></span>
<span data-ttu-id="8631f-p111">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="8631f-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 673

{
  "@odata.type": "#microsoft.graph.windowsPhone81CustomConfiguration",
  "id": "0d98693c-693c-0d98-3c69-980d3c69980d",
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




