---
title: androidCustomConfiguration の作成
description: 新しい androidCustomConfiguration オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: ad23e4129d65b5dc70f10a06e4f7bef393e96d22
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27966903"
---
# <a name="create-androidcustomconfiguration"></a><span data-ttu-id="27aef-103">androidCustomConfiguration の作成</span><span class="sxs-lookup"><span data-stu-id="27aef-103">Create androidCustomConfiguration</span></span>

> <span data-ttu-id="27aef-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="27aef-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="27aef-105">新しい [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="27aef-105">Create a new [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="27aef-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="27aef-106">Prerequisites</span></span>
<span data-ttu-id="27aef-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="27aef-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="27aef-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="27aef-109">Permission type</span></span>|<span data-ttu-id="27aef-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="27aef-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="27aef-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="27aef-111">Delegated (work or school account)</span></span>|<span data-ttu-id="27aef-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="27aef-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="27aef-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="27aef-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="27aef-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="27aef-114">Not supported.</span></span>|
|<span data-ttu-id="27aef-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="27aef-115">Application</span></span>|<span data-ttu-id="27aef-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="27aef-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="27aef-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="27aef-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="27aef-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="27aef-118">Request headers</span></span>
|<span data-ttu-id="27aef-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="27aef-119">Header</span></span>|<span data-ttu-id="27aef-120">値</span><span class="sxs-lookup"><span data-stu-id="27aef-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="27aef-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="27aef-121">Authorization</span></span>|<span data-ttu-id="27aef-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="27aef-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="27aef-123">Accept</span><span class="sxs-lookup"><span data-stu-id="27aef-123">Accept</span></span>|<span data-ttu-id="27aef-124">application/json</span><span class="sxs-lookup"><span data-stu-id="27aef-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="27aef-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="27aef-125">Request body</span></span>
<span data-ttu-id="27aef-126">要求本文で、androidCustomConfiguration オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="27aef-126">In the request body, supply a JSON representation for the androidCustomConfiguration object.</span></span>

<span data-ttu-id="27aef-127">次の表に、androidCustomConfiguration の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="27aef-127">The following table shows the properties that are required when you create the androidCustomConfiguration.</span></span>

|<span data-ttu-id="27aef-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="27aef-128">Property</span></span>|<span data-ttu-id="27aef-129">種類</span><span class="sxs-lookup"><span data-stu-id="27aef-129">Type</span></span>|<span data-ttu-id="27aef-130">説明</span><span class="sxs-lookup"><span data-stu-id="27aef-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="27aef-131">ID</span><span class="sxs-lookup"><span data-stu-id="27aef-131">id</span></span>|<span data-ttu-id="27aef-132">String</span><span class="sxs-lookup"><span data-stu-id="27aef-132">String</span></span>|<span data-ttu-id="27aef-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="27aef-133">Key of the entity.</span></span> <span data-ttu-id="27aef-134">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="27aef-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="27aef-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="27aef-135">lastModifiedDateTime</span></span>|<span data-ttu-id="27aef-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="27aef-136">DateTimeOffset</span></span>|<span data-ttu-id="27aef-137">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="27aef-137">DateTime the object was last modified.</span></span> <span data-ttu-id="27aef-138">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="27aef-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="27aef-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="27aef-139">createdDateTime</span></span>|<span data-ttu-id="27aef-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="27aef-140">DateTimeOffset</span></span>|<span data-ttu-id="27aef-141">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="27aef-141">DateTime the object was created.</span></span> <span data-ttu-id="27aef-142">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="27aef-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="27aef-143">説明</span><span class="sxs-lookup"><span data-stu-id="27aef-143">description</span></span>|<span data-ttu-id="27aef-144">String</span><span class="sxs-lookup"><span data-stu-id="27aef-144">String</span></span>|<span data-ttu-id="27aef-145">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="27aef-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="27aef-146">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="27aef-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="27aef-147">displayName</span><span class="sxs-lookup"><span data-stu-id="27aef-147">displayName</span></span>|<span data-ttu-id="27aef-148">String</span><span class="sxs-lookup"><span data-stu-id="27aef-148">String</span></span>|<span data-ttu-id="27aef-149">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="27aef-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="27aef-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="27aef-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="27aef-151">version</span><span class="sxs-lookup"><span data-stu-id="27aef-151">version</span></span>|<span data-ttu-id="27aef-152">Int32</span><span class="sxs-lookup"><span data-stu-id="27aef-152">Int32</span></span>|<span data-ttu-id="27aef-153">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="27aef-153">Version of the device configuration.</span></span> <span data-ttu-id="27aef-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="27aef-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="27aef-155">omaSettings</span><span class="sxs-lookup"><span data-stu-id="27aef-155">omaSettings</span></span>|<span data-ttu-id="27aef-156">[omaSetting](../resources/intune-deviceconfig-omasetting.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="27aef-156">[omaSetting](../resources/intune-deviceconfig-omasetting.md) collection</span></span>|<span data-ttu-id="27aef-157">OMA 設定。</span><span class="sxs-lookup"><span data-stu-id="27aef-157">OMA settings.</span></span> <span data-ttu-id="27aef-158">このコレクションには、最大で 1000 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="27aef-158">This collection can contain a maximum of 1000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="27aef-159">応答</span><span class="sxs-lookup"><span data-stu-id="27aef-159">Response</span></span>
<span data-ttu-id="27aef-160">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="27aef-160">If successful, this method returns a `201 Created` response code and a [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="27aef-161">例</span><span class="sxs-lookup"><span data-stu-id="27aef-161">Example</span></span>
### <a name="request"></a><span data-ttu-id="27aef-162">要求</span><span class="sxs-lookup"><span data-stu-id="27aef-162">Request</span></span>
<span data-ttu-id="27aef-163">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="27aef-163">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 402

{
  "@odata.type": "#microsoft.graph.androidCustomConfiguration",
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

### <a name="response"></a><span data-ttu-id="27aef-164">応答</span><span class="sxs-lookup"><span data-stu-id="27aef-164">Response</span></span>
<span data-ttu-id="27aef-p109">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="27aef-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 574

{
  "@odata.type": "#microsoft.graph.androidCustomConfiguration",
  "id": "619b5e6d-5e6d-619b-6d5e-9b616d5e9b61",
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



