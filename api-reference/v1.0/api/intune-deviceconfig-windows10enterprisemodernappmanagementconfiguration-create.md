---
title: windows10EnterpriseModernAppManagementConfiguration の作成
description: 新しい windows10EnterpriseModernAppManagementConfiguration オブジェクトを作成します。
ms.openlocfilehash: 0d324d2b6cdc2efa79a952418afb5459295931b7
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27021473"
---
# <a name="create-windows10enterprisemodernappmanagementconfiguration"></a><span data-ttu-id="d1df9-103">windows10EnterpriseModernAppManagementConfiguration の作成</span><span class="sxs-lookup"><span data-stu-id="d1df9-103">Create windows10EnterpriseModernAppManagementConfiguration</span></span>

> <span data-ttu-id="d1df9-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="d1df9-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d1df9-105">新しい [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="d1df9-105">Create a new [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d1df9-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="d1df9-106">Prerequisites</span></span>
<span data-ttu-id="d1df9-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d1df9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d1df9-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d1df9-109">Permission type</span></span>|<span data-ttu-id="d1df9-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="d1df9-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d1df9-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d1df9-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d1df9-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d1df9-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d1df9-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d1df9-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d1df9-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d1df9-114">Not supported.</span></span>|
|<span data-ttu-id="d1df9-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d1df9-115">Application</span></span>|<span data-ttu-id="d1df9-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d1df9-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d1df9-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d1df9-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="d1df9-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d1df9-118">Request headers</span></span>
|<span data-ttu-id="d1df9-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d1df9-119">Header</span></span>|<span data-ttu-id="d1df9-120">値</span><span class="sxs-lookup"><span data-stu-id="d1df9-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d1df9-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="d1df9-121">Authorization</span></span>|<span data-ttu-id="d1df9-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="d1df9-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d1df9-123">Accept</span><span class="sxs-lookup"><span data-stu-id="d1df9-123">Accept</span></span>|<span data-ttu-id="d1df9-124">application/json</span><span class="sxs-lookup"><span data-stu-id="d1df9-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d1df9-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="d1df9-125">Request body</span></span>
<span data-ttu-id="d1df9-126">要求本文で、windows10EnterpriseModernAppManagementConfiguration オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="d1df9-126">In the request body, supply a JSON representation for the windows10EnterpriseModernAppManagementConfiguration object.</span></span>

<span data-ttu-id="d1df9-127">次の表に、windows10EnterpriseModernAppManagementConfiguration の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="d1df9-127">The following table shows the properties that are required when you create the windows10EnterpriseModernAppManagementConfiguration.</span></span>

|<span data-ttu-id="d1df9-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d1df9-128">Property</span></span>|<span data-ttu-id="d1df9-129">型</span><span class="sxs-lookup"><span data-stu-id="d1df9-129">Type</span></span>|<span data-ttu-id="d1df9-130">説明</span><span class="sxs-lookup"><span data-stu-id="d1df9-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d1df9-131">id</span><span class="sxs-lookup"><span data-stu-id="d1df9-131">id</span></span>|<span data-ttu-id="d1df9-132">String</span><span class="sxs-lookup"><span data-stu-id="d1df9-132">String</span></span>|<span data-ttu-id="d1df9-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="d1df9-133">Key of the entity.</span></span> <span data-ttu-id="d1df9-134">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d1df9-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d1df9-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d1df9-135">lastModifiedDateTime</span></span>|<span data-ttu-id="d1df9-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d1df9-136">DateTimeOffset</span></span>|<span data-ttu-id="d1df9-137">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="d1df9-137">DateTime the object was last modified.</span></span> <span data-ttu-id="d1df9-138">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d1df9-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d1df9-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d1df9-139">createdDateTime</span></span>|<span data-ttu-id="d1df9-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d1df9-140">DateTimeOffset</span></span>|<span data-ttu-id="d1df9-141">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="d1df9-141">DateTime the object was created.</span></span> <span data-ttu-id="d1df9-142">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d1df9-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d1df9-143">説明</span><span class="sxs-lookup"><span data-stu-id="d1df9-143">description</span></span>|<span data-ttu-id="d1df9-144">String</span><span class="sxs-lookup"><span data-stu-id="d1df9-144">String</span></span>|<span data-ttu-id="d1df9-145">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="d1df9-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="d1df9-146">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d1df9-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d1df9-147">displayName</span><span class="sxs-lookup"><span data-stu-id="d1df9-147">displayName</span></span>|<span data-ttu-id="d1df9-148">String</span><span class="sxs-lookup"><span data-stu-id="d1df9-148">String</span></span>|<span data-ttu-id="d1df9-149">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="d1df9-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="d1df9-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d1df9-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d1df9-151">version</span><span class="sxs-lookup"><span data-stu-id="d1df9-151">version</span></span>|<span data-ttu-id="d1df9-152">Int32</span><span class="sxs-lookup"><span data-stu-id="d1df9-152">Int32</span></span>|<span data-ttu-id="d1df9-153">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="d1df9-153">Version of the device configuration.</span></span> <span data-ttu-id="d1df9-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d1df9-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d1df9-155">uninstallBuiltInApps</span><span class="sxs-lookup"><span data-stu-id="d1df9-155">uninstallBuiltInApps</span></span>|<span data-ttu-id="d1df9-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1df9-156">Boolean</span></span>|<span data-ttu-id="d1df9-157">組み込みの Windows アプリの固定リストをアンインストールするかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="d1df9-157">Indicates whether or not to uninstall a fixed list of built-in Windows apps.</span></span>|



## <a name="response"></a><span data-ttu-id="d1df9-158">応答</span><span class="sxs-lookup"><span data-stu-id="d1df9-158">Response</span></span>
<span data-ttu-id="d1df9-159">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="d1df9-159">If successful, this method returns a `201 Created` response code and a [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d1df9-160">例</span><span class="sxs-lookup"><span data-stu-id="d1df9-160">Example</span></span>
### <a name="request"></a><span data-ttu-id="d1df9-161">要求</span><span class="sxs-lookup"><span data-stu-id="d1df9-161">Request</span></span>
<span data-ttu-id="d1df9-162">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="d1df9-162">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 222

{
  "@odata.type": "#microsoft.graph.windows10EnterpriseModernAppManagementConfiguration",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "uninstallBuiltInApps": true
}
```

### <a name="response"></a><span data-ttu-id="d1df9-163">応答</span><span class="sxs-lookup"><span data-stu-id="d1df9-163">Response</span></span>
<span data-ttu-id="d1df9-p108">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="d1df9-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 394

{
  "@odata.type": "#microsoft.graph.windows10EnterpriseModernAppManagementConfiguration",
  "id": "d6577687-7687-d657-8776-57d6877657d6",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "uninstallBuiltInApps": true
}
```



