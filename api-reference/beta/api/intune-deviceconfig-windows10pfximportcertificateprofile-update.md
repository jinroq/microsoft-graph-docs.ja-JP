---
title: Windows10PFXImportCertificateProfile を更新します。
description: Windows10PFXImportCertificateProfile オブジェクトのプロパティを更新します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: eae2c39f2244dab4db2b4b034f04d2ce11008c2c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29408804"
---
# <a name="update-windows10pfximportcertificateprofile"></a><span data-ttu-id="50d92-103">Windows10PFXImportCertificateProfile を更新します。</span><span class="sxs-lookup"><span data-stu-id="50d92-103">Update windows10PFXImportCertificateProfile</span></span>

> <span data-ttu-id="50d92-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="50d92-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="50d92-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="50d92-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="50d92-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="50d92-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="50d92-107">[Windows10PFXImportCertificateProfile](../resources/intune-deviceconfig-windows10pfximportcertificateprofile.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="50d92-107">Update the properties of a [windows10PFXImportCertificateProfile](../resources/intune-deviceconfig-windows10pfximportcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="50d92-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="50d92-108">Prerequisites</span></span>
<span data-ttu-id="50d92-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="50d92-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="50d92-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="50d92-111">Permission type</span></span>|<span data-ttu-id="50d92-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="50d92-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="50d92-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="50d92-113">Delegated (work or school account)</span></span>|<span data-ttu-id="50d92-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="50d92-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="50d92-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="50d92-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="50d92-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="50d92-116">Not supported.</span></span>|
|<span data-ttu-id="50d92-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="50d92-117">Application</span></span>|<span data-ttu-id="50d92-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="50d92-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="50d92-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="50d92-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="50d92-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="50d92-120">Request headers</span></span>
|<span data-ttu-id="50d92-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="50d92-121">Header</span></span>|<span data-ttu-id="50d92-122">値</span><span class="sxs-lookup"><span data-stu-id="50d92-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="50d92-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="50d92-123">Authorization</span></span>|<span data-ttu-id="50d92-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="50d92-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="50d92-125">Accept</span><span class="sxs-lookup"><span data-stu-id="50d92-125">Accept</span></span>|<span data-ttu-id="50d92-126">application/json</span><span class="sxs-lookup"><span data-stu-id="50d92-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="50d92-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="50d92-127">Request body</span></span>
<span data-ttu-id="50d92-128">要求の本文に[windows10PFXImportCertificateProfile](../resources/intune-deviceconfig-windows10pfximportcertificateprofile.md)オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="50d92-128">In the request body, supply a JSON representation for the [windows10PFXImportCertificateProfile](../resources/intune-deviceconfig-windows10pfximportcertificateprofile.md) object.</span></span>

<span data-ttu-id="50d92-129">[Windows10PFXImportCertificateProfile](../resources/intune-deviceconfig-windows10pfximportcertificateprofile.md)を作成するときに必要なプロパティを次の表に示します。</span><span class="sxs-lookup"><span data-stu-id="50d92-129">The following table shows the properties that are required when you create the [windows10PFXImportCertificateProfile](../resources/intune-deviceconfig-windows10pfximportcertificateprofile.md).</span></span>

|<span data-ttu-id="50d92-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="50d92-130">Property</span></span>|<span data-ttu-id="50d92-131">型</span><span class="sxs-lookup"><span data-stu-id="50d92-131">Type</span></span>|<span data-ttu-id="50d92-132">説明</span><span class="sxs-lookup"><span data-stu-id="50d92-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="50d92-133">id</span><span class="sxs-lookup"><span data-stu-id="50d92-133">id</span></span>|<span data-ttu-id="50d92-134">String</span><span class="sxs-lookup"><span data-stu-id="50d92-134">String</span></span>|<span data-ttu-id="50d92-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="50d92-135">Key of the entity.</span></span> <span data-ttu-id="50d92-136">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="50d92-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="50d92-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="50d92-137">lastModifiedDateTime</span></span>|<span data-ttu-id="50d92-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="50d92-138">DateTimeOffset</span></span>|<span data-ttu-id="50d92-139">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="50d92-139">DateTime the object was last modified.</span></span> <span data-ttu-id="50d92-140">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="50d92-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="50d92-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="50d92-141">roleScopeTagIds</span></span>|<span data-ttu-id="50d92-142">String コレクション</span><span class="sxs-lookup"><span data-stu-id="50d92-142">String collection</span></span>|<span data-ttu-id="50d92-143">このエンティティ インスタンスのスコープのタグのリストです。</span><span class="sxs-lookup"><span data-stu-id="50d92-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="50d92-144">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="50d92-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="50d92-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="50d92-145">supportsScopeTags</span></span>|<span data-ttu-id="50d92-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="50d92-146">Boolean</span></span>|<span data-ttu-id="50d92-147">デバイスの構成を基になるスコープのタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="50d92-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="50d92-148">この値が false であり、エンティティをスコープ指定されたユーザーには表示されませんがある場合、ScopeTags プロパティに割り当てることは許可されていません。</span><span class="sxs-lookup"><span data-stu-id="50d92-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="50d92-149">これは、Silverlight で作成されたレガシ ポリシーに対して発生し、削除して、Azure ポータル内のポリシーを再作成することで解決できます。</span><span class="sxs-lookup"><span data-stu-id="50d92-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="50d92-150">このプロパティは読み取りのみ可能です。</span><span class="sxs-lookup"><span data-stu-id="50d92-150">This property is read-only.</span></span> <span data-ttu-id="50d92-151">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="50d92-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="50d92-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="50d92-152">createdDateTime</span></span>|<span data-ttu-id="50d92-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="50d92-153">DateTimeOffset</span></span>|<span data-ttu-id="50d92-154">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="50d92-154">DateTime the object was created.</span></span> <span data-ttu-id="50d92-155">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="50d92-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="50d92-156">説明</span><span class="sxs-lookup"><span data-stu-id="50d92-156">description</span></span>|<span data-ttu-id="50d92-157">String</span><span class="sxs-lookup"><span data-stu-id="50d92-157">String</span></span>|<span data-ttu-id="50d92-158">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="50d92-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="50d92-159">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="50d92-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="50d92-160">displayName</span><span class="sxs-lookup"><span data-stu-id="50d92-160">displayName</span></span>|<span data-ttu-id="50d92-161">String</span><span class="sxs-lookup"><span data-stu-id="50d92-161">String</span></span>|<span data-ttu-id="50d92-162">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="50d92-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="50d92-163">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="50d92-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="50d92-164">version</span><span class="sxs-lookup"><span data-stu-id="50d92-164">version</span></span>|<span data-ttu-id="50d92-165">Int32</span><span class="sxs-lookup"><span data-stu-id="50d92-165">Int32</span></span>|<span data-ttu-id="50d92-166">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="50d92-166">Version of the device configuration.</span></span> <span data-ttu-id="50d92-167">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="50d92-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="50d92-168">keyStorageProvider</span><span class="sxs-lookup"><span data-stu-id="50d92-168">keyStorageProvider</span></span>|[<span data-ttu-id="50d92-169">keyStorageProviderOption</span><span class="sxs-lookup"><span data-stu-id="50d92-169">keyStorageProviderOption</span></span>](../resources/intune-deviceconfig-keystorageprovideroption.md)|<span data-ttu-id="50d92-170">まだ記載されていません。</span><span class="sxs-lookup"><span data-stu-id="50d92-170">Not yet documented.</span></span> <span data-ttu-id="50d92-171">可能な値は、`useTpmKspOtherwiseUseSoftwareKsp`、`useTpmKspOtherwiseFail`、`usePassportForWorkKspOtherwiseFail`、`useSoftwareKsp` です。</span><span class="sxs-lookup"><span data-stu-id="50d92-171">Possible values are: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span></span>|



## <a name="response"></a><span data-ttu-id="50d92-172">応答</span><span class="sxs-lookup"><span data-stu-id="50d92-172">Response</span></span>
<span data-ttu-id="50d92-173">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に更新された[windows10PFXImportCertificateProfile](../resources/intune-deviceconfig-windows10pfximportcertificateprofile.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="50d92-173">If successful, this method returns a `200 OK` response code and an updated [windows10PFXImportCertificateProfile](../resources/intune-deviceconfig-windows10pfximportcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="50d92-174">例</span><span class="sxs-lookup"><span data-stu-id="50d92-174">Example</span></span>

### <a name="request"></a><span data-ttu-id="50d92-175">要求</span><span class="sxs-lookup"><span data-stu-id="50d92-175">Request</span></span>
<span data-ttu-id="50d92-176">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="50d92-176">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 317

{
  "@odata.type": "#microsoft.graph.windows10PFXImportCertificateProfile",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "keyStorageProvider": "useTpmKspOtherwiseFail"
}
```

### <a name="response"></a><span data-ttu-id="50d92-177">応答</span><span class="sxs-lookup"><span data-stu-id="50d92-177">Response</span></span>
<span data-ttu-id="50d92-p112">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="50d92-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 489

{
  "@odata.type": "#microsoft.graph.windows10PFXImportCertificateProfile",
  "id": "4244277a-277a-4244-7a27-44427a274442",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "keyStorageProvider": "useTpmKspOtherwiseFail"
}
```




