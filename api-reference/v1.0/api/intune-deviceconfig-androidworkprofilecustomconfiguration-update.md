---
title: androidWorkProfileCustomConfiguration の更新
description: androidWorkProfileCustomConfiguration オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8da7ceee5827bc97e628a8991682f951daf40964
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30256750"
---
# <a name="update-androidworkprofilecustomconfiguration"></a><span data-ttu-id="4666a-103">androidWorkProfileCustomConfiguration の更新</span><span class="sxs-lookup"><span data-stu-id="4666a-103">Update androidWorkProfileCustomConfiguration</span></span>

> <span data-ttu-id="4666a-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="4666a-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4666a-105">[androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="4666a-105">Update the properties of a [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4666a-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="4666a-106">Prerequisites</span></span>
<span data-ttu-id="4666a-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4666a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="4666a-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="4666a-109">Permission type</span></span>|<span data-ttu-id="4666a-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="4666a-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4666a-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="4666a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="4666a-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4666a-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4666a-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="4666a-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4666a-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4666a-114">Not supported.</span></span>|
|<span data-ttu-id="4666a-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="4666a-115">Application</span></span>|<span data-ttu-id="4666a-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4666a-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4666a-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="4666a-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="4666a-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4666a-118">Request headers</span></span>
|<span data-ttu-id="4666a-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4666a-119">Header</span></span>|<span data-ttu-id="4666a-120">値</span><span class="sxs-lookup"><span data-stu-id="4666a-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4666a-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="4666a-121">Authorization</span></span>|<span data-ttu-id="4666a-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="4666a-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4666a-123">承諾</span><span class="sxs-lookup"><span data-stu-id="4666a-123">Accept</span></span>|<span data-ttu-id="4666a-124">application/json</span><span class="sxs-lookup"><span data-stu-id="4666a-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4666a-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="4666a-125">Request body</span></span>
<span data-ttu-id="4666a-126">要求本文で、 [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="4666a-126">In the request body, supply a JSON representation for the [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) object.</span></span>

<span data-ttu-id="4666a-127">次の表に、 [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="4666a-127">The following table shows the properties that are required when you create the [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md).</span></span>

|<span data-ttu-id="4666a-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4666a-128">Property</span></span>|<span data-ttu-id="4666a-129">型</span><span class="sxs-lookup"><span data-stu-id="4666a-129">Type</span></span>|<span data-ttu-id="4666a-130">説明</span><span class="sxs-lookup"><span data-stu-id="4666a-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4666a-131">id</span><span class="sxs-lookup"><span data-stu-id="4666a-131">id</span></span>|<span data-ttu-id="4666a-132">文字列</span><span class="sxs-lookup"><span data-stu-id="4666a-132">String</span></span>|<span data-ttu-id="4666a-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="4666a-133">Key of the entity.</span></span> <span data-ttu-id="4666a-134">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4666a-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4666a-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4666a-135">lastModifiedDateTime</span></span>|<span data-ttu-id="4666a-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4666a-136">DateTimeOffset</span></span>|<span data-ttu-id="4666a-137">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="4666a-137">DateTime the object was last modified.</span></span> <span data-ttu-id="4666a-138">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4666a-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4666a-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4666a-139">createdDateTime</span></span>|<span data-ttu-id="4666a-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4666a-140">DateTimeOffset</span></span>|<span data-ttu-id="4666a-141">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="4666a-141">DateTime the object was created.</span></span> <span data-ttu-id="4666a-142">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4666a-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4666a-143">説明</span><span class="sxs-lookup"><span data-stu-id="4666a-143">description</span></span>|<span data-ttu-id="4666a-144">String</span><span class="sxs-lookup"><span data-stu-id="4666a-144">String</span></span>|<span data-ttu-id="4666a-145">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="4666a-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="4666a-146">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4666a-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4666a-147">displayName</span><span class="sxs-lookup"><span data-stu-id="4666a-147">displayName</span></span>|<span data-ttu-id="4666a-148">String</span><span class="sxs-lookup"><span data-stu-id="4666a-148">String</span></span>|<span data-ttu-id="4666a-149">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="4666a-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="4666a-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4666a-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4666a-151">version</span><span class="sxs-lookup"><span data-stu-id="4666a-151">version</span></span>|<span data-ttu-id="4666a-152">Int32</span><span class="sxs-lookup"><span data-stu-id="4666a-152">Int32</span></span>|<span data-ttu-id="4666a-153">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="4666a-153">Version of the device configuration.</span></span> <span data-ttu-id="4666a-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4666a-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4666a-155">omaSettings</span><span class="sxs-lookup"><span data-stu-id="4666a-155">omaSettings</span></span>|<span data-ttu-id="4666a-156">[omaSetting](../resources/intune-deviceconfig-omasetting.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="4666a-156">[omaSetting](../resources/intune-deviceconfig-omasetting.md) collection</span></span>|<span data-ttu-id="4666a-157">OMA 設定。</span><span class="sxs-lookup"><span data-stu-id="4666a-157">OMA settings.</span></span> <span data-ttu-id="4666a-158">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="4666a-158">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="4666a-159">応答</span><span class="sxs-lookup"><span data-stu-id="4666a-159">Response</span></span>
<span data-ttu-id="4666a-160">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="4666a-160">If successful, this method returns a `200 OK` response code and an updated [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4666a-161">例</span><span class="sxs-lookup"><span data-stu-id="4666a-161">Example</span></span>

### <a name="request"></a><span data-ttu-id="4666a-162">要求</span><span class="sxs-lookup"><span data-stu-id="4666a-162">Request</span></span>
<span data-ttu-id="4666a-163">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="4666a-163">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
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

### <a name="response"></a><span data-ttu-id="4666a-164">応答</span><span class="sxs-lookup"><span data-stu-id="4666a-164">Response</span></span>
<span data-ttu-id="4666a-p109">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="4666a-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



