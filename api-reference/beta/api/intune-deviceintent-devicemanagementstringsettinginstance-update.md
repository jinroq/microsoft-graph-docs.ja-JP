---
title: devicemanagementstringsettinginstance の更新
description: devicemanagementstringsettinginstance オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9862d1fa940df35806843850d0cb6c74dcd3672e
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31792413"
---
# <a name="update-devicemanagementstringsettinginstance"></a><span data-ttu-id="f157c-103">devicemanagementstringsettinginstance の更新</span><span class="sxs-lookup"><span data-stu-id="f157c-103">Update deviceManagementStringSettingInstance</span></span>

> <span data-ttu-id="f157c-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f157c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f157c-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="f157c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f157c-106">[devicemanagementstringsettinginstance](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="f157c-106">Update the properties of a [deviceManagementStringSettingInstance](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f157c-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="f157c-107">Prerequisites</span></span>
<span data-ttu-id="f157c-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f157c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f157c-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f157c-110">Permission type</span></span>|<span data-ttu-id="f157c-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="f157c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f157c-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f157c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f157c-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f157c-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f157c-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f157c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f157c-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f157c-115">Not supported.</span></span>|
|<span data-ttu-id="f157c-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f157c-116">Application</span></span>|<span data-ttu-id="f157c-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f157c-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f157c-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f157c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/intents/{deviceManagementIntentId}/settings/{deviceManagementSettingInstanceId}
PATCH /deviceManagement/templates/{deviceManagementTemplateId}/settings/{deviceManagementSettingInstanceId}
PATCH /deviceManagement/intents/{deviceManagementIntentId}/categories/{deviceManagementIntentSettingCategoryId}/settings/{deviceManagementSettingInstanceId}
PATCH /deviceManagement/templates/{deviceManagementTemplateId}/categories/{deviceManagementTemplateSettingCategoryId}/recommendedSettings/{deviceManagementSettingInstanceId}
```

## <a name="request-headers"></a><span data-ttu-id="f157c-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f157c-119">Request headers</span></span>
|<span data-ttu-id="f157c-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f157c-120">Header</span></span>|<span data-ttu-id="f157c-121">値</span><span class="sxs-lookup"><span data-stu-id="f157c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f157c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f157c-122">Authorization</span></span>|<span data-ttu-id="f157c-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="f157c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f157c-124">承諾</span><span class="sxs-lookup"><span data-stu-id="f157c-124">Accept</span></span>|<span data-ttu-id="f157c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f157c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f157c-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="f157c-126">Request body</span></span>
<span data-ttu-id="f157c-127">要求本文で、 [devicemanagementstringsettinginstance](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="f157c-127">In the request body, supply a JSON representation for the [deviceManagementStringSettingInstance](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md) object.</span></span>

<span data-ttu-id="f157c-128">次の表に、 [devicemanagementstringsettinginstance](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="f157c-128">The following table shows the properties that are required when you create the [deviceManagementStringSettingInstance](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md).</span></span>

|<span data-ttu-id="f157c-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f157c-129">Property</span></span>|<span data-ttu-id="f157c-130">型</span><span class="sxs-lookup"><span data-stu-id="f157c-130">Type</span></span>|<span data-ttu-id="f157c-131">説明</span><span class="sxs-lookup"><span data-stu-id="f157c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f157c-132">id</span><span class="sxs-lookup"><span data-stu-id="f157c-132">id</span></span>|<span data-ttu-id="f157c-133">String</span><span class="sxs-lookup"><span data-stu-id="f157c-133">String</span></span>|<span data-ttu-id="f157c-134">[devicemanagementsettinginstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)から継承された設定インスタンス ID</span><span class="sxs-lookup"><span data-stu-id="f157c-134">The setting instance ID Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="f157c-135">definitionId</span><span class="sxs-lookup"><span data-stu-id="f157c-135">definitionId</span></span>|<span data-ttu-id="f157c-136">文字列</span><span class="sxs-lookup"><span data-stu-id="f157c-136">String</span></span>|<span data-ttu-id="f157c-137">[devicemanagementsettinginstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)から継承されたこのインスタンスの設定定義の ID</span><span class="sxs-lookup"><span data-stu-id="f157c-137">The ID of the setting definition for this instance Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="f157c-138">valuejson</span><span class="sxs-lookup"><span data-stu-id="f157c-138">valueJson</span></span>|<span data-ttu-id="f157c-139">文字列</span><span class="sxs-lookup"><span data-stu-id="f157c-139">String</span></span>|<span data-ttu-id="f157c-140">[devicemanagementsettinginstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)から継承された値の JSON 表現</span><span class="sxs-lookup"><span data-stu-id="f157c-140">JSON representation of the value Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="f157c-141">value</span><span class="sxs-lookup"><span data-stu-id="f157c-141">value</span></span>|<span data-ttu-id="f157c-142">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="f157c-142">String</span></span>|<span data-ttu-id="f157c-143">文字列型 (string) の値</span><span class="sxs-lookup"><span data-stu-id="f157c-143">The string value</span></span>|



## <a name="response"></a><span data-ttu-id="f157c-144">応答</span><span class="sxs-lookup"><span data-stu-id="f157c-144">Response</span></span>
<span data-ttu-id="f157c-145">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[devicemanagementstringsettinginstance](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="f157c-145">If successful, this method returns a `200 OK` response code and an updated [deviceManagementStringSettingInstance](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f157c-146">例</span><span class="sxs-lookup"><span data-stu-id="f157c-146">Example</span></span>

### <a name="request"></a><span data-ttu-id="f157c-147">要求</span><span class="sxs-lookup"><span data-stu-id="f157c-147">Request</span></span>
<span data-ttu-id="f157c-148">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="f157c-148">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/settings/{deviceManagementSettingInstanceId}
Content-type: application/json
Content-length: 184

{
  "@odata.type": "#microsoft.graph.deviceManagementStringSettingInstance",
  "definitionId": "Definition Id value",
  "valueJson": "Value Json value",
  "value": "Value value"
}
```

### <a name="response"></a><span data-ttu-id="f157c-149">応答</span><span class="sxs-lookup"><span data-stu-id="f157c-149">Response</span></span>
<span data-ttu-id="f157c-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="f157c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 233

{
  "@odata.type": "#microsoft.graph.deviceManagementStringSettingInstance",
  "id": "fef30638-0638-fef3-3806-f3fe3806f3fe",
  "definitionId": "Definition Id value",
  "valueJson": "Value Json value",
  "value": "Value value"
}
```





