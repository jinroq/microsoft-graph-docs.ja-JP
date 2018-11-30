---
title: windowsPhone81CustomConfiguration の作成
description: 新しい windowsPhone81CustomConfiguration オブジェクトを作成します。
ms.openlocfilehash: cf3b897fe86350be5c2bd1c243d0dce3147e2c05
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27021424"
---
# <a name="create-windowsphone81customconfiguration"></a><span data-ttu-id="e3eb1-103">windowsPhone81CustomConfiguration の作成</span><span class="sxs-lookup"><span data-stu-id="e3eb1-103">Create windowsPhone81CustomConfiguration</span></span>

> <span data-ttu-id="e3eb1-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="e3eb1-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e3eb1-105">新しい [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="e3eb1-105">Create a new [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e3eb1-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="e3eb1-106">Prerequisites</span></span>
<span data-ttu-id="e3eb1-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e3eb1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e3eb1-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e3eb1-109">Permission type</span></span>|<span data-ttu-id="e3eb1-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="e3eb1-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e3eb1-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e3eb1-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e3eb1-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e3eb1-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e3eb1-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e3eb1-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e3eb1-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e3eb1-114">Not supported.</span></span>|
|<span data-ttu-id="e3eb1-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e3eb1-115">Application</span></span>|<span data-ttu-id="e3eb1-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e3eb1-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e3eb1-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e3eb1-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="e3eb1-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e3eb1-118">Request headers</span></span>
|<span data-ttu-id="e3eb1-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e3eb1-119">Header</span></span>|<span data-ttu-id="e3eb1-120">値</span><span class="sxs-lookup"><span data-stu-id="e3eb1-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e3eb1-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="e3eb1-121">Authorization</span></span>|<span data-ttu-id="e3eb1-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="e3eb1-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e3eb1-123">Accept</span><span class="sxs-lookup"><span data-stu-id="e3eb1-123">Accept</span></span>|<span data-ttu-id="e3eb1-124">application/json</span><span class="sxs-lookup"><span data-stu-id="e3eb1-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e3eb1-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="e3eb1-125">Request body</span></span>
<span data-ttu-id="e3eb1-126">要求本文で、windowsPhone81CustomConfiguration オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="e3eb1-126">In the request body, supply a JSON representation for the windowsPhone81CustomConfiguration object.</span></span>

<span data-ttu-id="e3eb1-127">次の表に、windowsPhone81CustomConfiguration の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="e3eb1-127">The following table shows the properties that are required when you create the windowsPhone81CustomConfiguration.</span></span>

|<span data-ttu-id="e3eb1-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e3eb1-128">Property</span></span>|<span data-ttu-id="e3eb1-129">型</span><span class="sxs-lookup"><span data-stu-id="e3eb1-129">Type</span></span>|<span data-ttu-id="e3eb1-130">説明</span><span class="sxs-lookup"><span data-stu-id="e3eb1-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e3eb1-131">id</span><span class="sxs-lookup"><span data-stu-id="e3eb1-131">id</span></span>|<span data-ttu-id="e3eb1-132">String</span><span class="sxs-lookup"><span data-stu-id="e3eb1-132">String</span></span>|<span data-ttu-id="e3eb1-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="e3eb1-133">Key of the entity.</span></span> <span data-ttu-id="e3eb1-134">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e3eb1-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e3eb1-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e3eb1-135">lastModifiedDateTime</span></span>|<span data-ttu-id="e3eb1-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e3eb1-136">DateTimeOffset</span></span>|<span data-ttu-id="e3eb1-137">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="e3eb1-137">DateTime the object was last modified.</span></span> <span data-ttu-id="e3eb1-138">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e3eb1-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e3eb1-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e3eb1-139">createdDateTime</span></span>|<span data-ttu-id="e3eb1-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e3eb1-140">DateTimeOffset</span></span>|<span data-ttu-id="e3eb1-141">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="e3eb1-141">DateTime the object was created.</span></span> <span data-ttu-id="e3eb1-142">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e3eb1-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e3eb1-143">説明</span><span class="sxs-lookup"><span data-stu-id="e3eb1-143">description</span></span>|<span data-ttu-id="e3eb1-144">String</span><span class="sxs-lookup"><span data-stu-id="e3eb1-144">String</span></span>|<span data-ttu-id="e3eb1-145">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="e3eb1-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="e3eb1-146">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e3eb1-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e3eb1-147">displayName</span><span class="sxs-lookup"><span data-stu-id="e3eb1-147">displayName</span></span>|<span data-ttu-id="e3eb1-148">String</span><span class="sxs-lookup"><span data-stu-id="e3eb1-148">String</span></span>|<span data-ttu-id="e3eb1-149">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="e3eb1-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="e3eb1-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e3eb1-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e3eb1-151">version</span><span class="sxs-lookup"><span data-stu-id="e3eb1-151">version</span></span>|<span data-ttu-id="e3eb1-152">Int32</span><span class="sxs-lookup"><span data-stu-id="e3eb1-152">Int32</span></span>|<span data-ttu-id="e3eb1-153">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="e3eb1-153">Version of the device configuration.</span></span> <span data-ttu-id="e3eb1-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e3eb1-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e3eb1-155">omaSettings</span><span class="sxs-lookup"><span data-stu-id="e3eb1-155">omaSettings</span></span>|<span data-ttu-id="e3eb1-156">[omaSetting](../resources/intune-deviceconfig-omasetting.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="e3eb1-156">[omaSetting](../resources/intune-deviceconfig-omasetting.md) collection</span></span>|<span data-ttu-id="e3eb1-157">OMA 設定。</span><span class="sxs-lookup"><span data-stu-id="e3eb1-157">OMA settings.</span></span> <span data-ttu-id="e3eb1-158">このコレクションには、最大で 1000 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="e3eb1-158">This collection can contain a maximum of 1000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="e3eb1-159">応答</span><span class="sxs-lookup"><span data-stu-id="e3eb1-159">Response</span></span>
<span data-ttu-id="e3eb1-160">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="e3eb1-160">If successful, this method returns a `201 Created` response code and a [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e3eb1-161">例</span><span class="sxs-lookup"><span data-stu-id="e3eb1-161">Example</span></span>
### <a name="request"></a><span data-ttu-id="e3eb1-162">要求</span><span class="sxs-lookup"><span data-stu-id="e3eb1-162">Request</span></span>
<span data-ttu-id="e3eb1-163">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="e3eb1-163">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 409

{
  "@odata.type": "#microsoft.graph.windowsPhone81CustomConfiguration",
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

### <a name="response"></a><span data-ttu-id="e3eb1-164">応答</span><span class="sxs-lookup"><span data-stu-id="e3eb1-164">Response</span></span>
<span data-ttu-id="e3eb1-p109">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="e3eb1-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 581

{
  "@odata.type": "#microsoft.graph.windowsPhone81CustomConfiguration",
  "id": "0d98693c-693c-0d98-3c69-980d3c69980d",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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



