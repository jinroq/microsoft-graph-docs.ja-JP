---
title: AndroidWorkProfileCustomConfiguration を作成します。
description: 新しい androidWorkProfileCustomConfiguration オブジェクトを作成します。
author: tfitzmac
ms.openlocfilehash: 4b33b75e66845652315b91ae70e393e8c76c7ce0
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27353607"
---
# <a name="create-androidworkprofilecustomconfiguration"></a><span data-ttu-id="376cf-103">AndroidWorkProfileCustomConfiguration を作成します。</span><span class="sxs-lookup"><span data-stu-id="376cf-103">Create androidWorkProfileCustomConfiguration</span></span>

> <span data-ttu-id="376cf-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="376cf-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="376cf-105">新しい[androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="376cf-105">Create a new [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="376cf-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="376cf-106">Prerequisites</span></span>
<span data-ttu-id="376cf-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="376cf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="376cf-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="376cf-109">Permission type</span></span>|<span data-ttu-id="376cf-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="376cf-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="376cf-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="376cf-111">Delegated (work or school account)</span></span>|<span data-ttu-id="376cf-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="376cf-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="376cf-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="376cf-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="376cf-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="376cf-114">Not supported.</span></span>|
|<span data-ttu-id="376cf-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="376cf-115">Application</span></span>|<span data-ttu-id="376cf-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="376cf-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="376cf-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="376cf-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="376cf-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="376cf-118">Request headers</span></span>
|<span data-ttu-id="376cf-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="376cf-119">Header</span></span>|<span data-ttu-id="376cf-120">値</span><span class="sxs-lookup"><span data-stu-id="376cf-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="376cf-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="376cf-121">Authorization</span></span>|<span data-ttu-id="376cf-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="376cf-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="376cf-123">Accept</span><span class="sxs-lookup"><span data-stu-id="376cf-123">Accept</span></span>|<span data-ttu-id="376cf-124">application/json</span><span class="sxs-lookup"><span data-stu-id="376cf-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="376cf-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="376cf-125">Request body</span></span>
<span data-ttu-id="376cf-126">要求の本文に androidWorkProfileCustomConfiguration オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="376cf-126">In the request body, supply a JSON representation for the androidWorkProfileCustomConfiguration object.</span></span>

<span data-ttu-id="376cf-127">次の表は、androidWorkProfileCustomConfiguration を作成するときに必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="376cf-127">The following table shows the properties that are required when you create the androidWorkProfileCustomConfiguration.</span></span>

|<span data-ttu-id="376cf-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="376cf-128">Property</span></span>|<span data-ttu-id="376cf-129">種類</span><span class="sxs-lookup"><span data-stu-id="376cf-129">Type</span></span>|<span data-ttu-id="376cf-130">説明</span><span class="sxs-lookup"><span data-stu-id="376cf-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="376cf-131">ID</span><span class="sxs-lookup"><span data-stu-id="376cf-131">id</span></span>|<span data-ttu-id="376cf-132">String</span><span class="sxs-lookup"><span data-stu-id="376cf-132">String</span></span>|<span data-ttu-id="376cf-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="376cf-133">Key of the entity.</span></span> <span data-ttu-id="376cf-134">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="376cf-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="376cf-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="376cf-135">lastModifiedDateTime</span></span>|<span data-ttu-id="376cf-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="376cf-136">DateTimeOffset</span></span>|<span data-ttu-id="376cf-137">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="376cf-137">DateTime the object was last modified.</span></span> <span data-ttu-id="376cf-138">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="376cf-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="376cf-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="376cf-139">createdDateTime</span></span>|<span data-ttu-id="376cf-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="376cf-140">DateTimeOffset</span></span>|<span data-ttu-id="376cf-141">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="376cf-141">DateTime the object was created.</span></span> <span data-ttu-id="376cf-142">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="376cf-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="376cf-143">説明</span><span class="sxs-lookup"><span data-stu-id="376cf-143">description</span></span>|<span data-ttu-id="376cf-144">String</span><span class="sxs-lookup"><span data-stu-id="376cf-144">String</span></span>|<span data-ttu-id="376cf-145">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="376cf-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="376cf-146">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="376cf-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="376cf-147">displayName</span><span class="sxs-lookup"><span data-stu-id="376cf-147">displayName</span></span>|<span data-ttu-id="376cf-148">String</span><span class="sxs-lookup"><span data-stu-id="376cf-148">String</span></span>|<span data-ttu-id="376cf-149">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="376cf-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="376cf-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="376cf-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="376cf-151">version</span><span class="sxs-lookup"><span data-stu-id="376cf-151">version</span></span>|<span data-ttu-id="376cf-152">Int32</span><span class="sxs-lookup"><span data-stu-id="376cf-152">Int32</span></span>|<span data-ttu-id="376cf-153">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="376cf-153">Version of the device configuration.</span></span> <span data-ttu-id="376cf-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="376cf-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="376cf-155">omaSettings</span><span class="sxs-lookup"><span data-stu-id="376cf-155">omaSettings</span></span>|<span data-ttu-id="376cf-156">[omaSetting](../resources/intune-deviceconfig-omasetting.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="376cf-156">[omaSetting](../resources/intune-deviceconfig-omasetting.md) collection</span></span>|<span data-ttu-id="376cf-157">OMA 設定。</span><span class="sxs-lookup"><span data-stu-id="376cf-157">OMA settings.</span></span> <span data-ttu-id="376cf-158">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="376cf-158">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="376cf-159">応答</span><span class="sxs-lookup"><span data-stu-id="376cf-159">Response</span></span>
<span data-ttu-id="376cf-160">かどうかは成功すると、このメソッドが返されます、`201 Created`応答コードおよび応答の本文に[androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="376cf-160">If successful, this method returns a `201 Created` response code and a [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="376cf-161">例</span><span class="sxs-lookup"><span data-stu-id="376cf-161">Example</span></span>
### <a name="request"></a><span data-ttu-id="376cf-162">要求</span><span class="sxs-lookup"><span data-stu-id="376cf-162">Request</span></span>
<span data-ttu-id="376cf-163">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="376cf-163">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 413

{
  "@odata.type": "#microsoft.graph.androidWorkProfileCustomConfiguration",
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

### <a name="response"></a><span data-ttu-id="376cf-164">応答</span><span class="sxs-lookup"><span data-stu-id="376cf-164">Response</span></span>
<span data-ttu-id="376cf-p109">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="376cf-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 585

{
  "@odata.type": "#microsoft.graph.androidWorkProfileCustomConfiguration",
  "id": "76c5d59b-d59b-76c5-9bd5-c5769bd5c576",
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


