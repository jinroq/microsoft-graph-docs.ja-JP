---
title: DeviceManagementBooleanSettingInstance の更新
description: DeviceManagementBooleanSettingInstance オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ab568b8f882487156212805e76c9786948b95d0c
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34960889"
---
# <a name="update-devicemanagementbooleansettinginstance"></a><span data-ttu-id="64bbb-103">DeviceManagementBooleanSettingInstance の更新</span><span class="sxs-lookup"><span data-stu-id="64bbb-103">Update deviceManagementBooleanSettingInstance</span></span>

> <span data-ttu-id="64bbb-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="64bbb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="64bbb-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="64bbb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="64bbb-106">[DeviceManagementBooleanSettingInstance](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="64bbb-106">Update the properties of a [deviceManagementBooleanSettingInstance](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="64bbb-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="64bbb-107">Prerequisites</span></span>
<span data-ttu-id="64bbb-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="64bbb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="64bbb-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="64bbb-110">Permission type</span></span>|<span data-ttu-id="64bbb-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="64bbb-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="64bbb-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="64bbb-112">Delegated (work or school account)</span></span>|<span data-ttu-id="64bbb-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="64bbb-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="64bbb-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="64bbb-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="64bbb-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="64bbb-115">Not supported.</span></span>|
|<span data-ttu-id="64bbb-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="64bbb-116">Application</span></span>|<span data-ttu-id="64bbb-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="64bbb-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="64bbb-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="64bbb-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="64bbb-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="64bbb-119">Request headers</span></span>
|<span data-ttu-id="64bbb-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="64bbb-120">Header</span></span>|<span data-ttu-id="64bbb-121">値</span><span class="sxs-lookup"><span data-stu-id="64bbb-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="64bbb-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="64bbb-122">Authorization</span></span>|<span data-ttu-id="64bbb-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="64bbb-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="64bbb-124">承諾</span><span class="sxs-lookup"><span data-stu-id="64bbb-124">Accept</span></span>|<span data-ttu-id="64bbb-125">application/json</span><span class="sxs-lookup"><span data-stu-id="64bbb-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="64bbb-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="64bbb-126">Request body</span></span>
<span data-ttu-id="64bbb-127">要求本文で、 [deviceManagementBooleanSettingInstance](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="64bbb-127">In the request body, supply a JSON representation for the [deviceManagementBooleanSettingInstance](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md) object.</span></span>

<span data-ttu-id="64bbb-128">次の表に、 [deviceManagementBooleanSettingInstance](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="64bbb-128">The following table shows the properties that are required when you create the [deviceManagementBooleanSettingInstance](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md).</span></span>

|<span data-ttu-id="64bbb-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="64bbb-129">Property</span></span>|<span data-ttu-id="64bbb-130">型</span><span class="sxs-lookup"><span data-stu-id="64bbb-130">Type</span></span>|<span data-ttu-id="64bbb-131">説明</span><span class="sxs-lookup"><span data-stu-id="64bbb-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="64bbb-132">id</span><span class="sxs-lookup"><span data-stu-id="64bbb-132">id</span></span>|<span data-ttu-id="64bbb-133">String</span><span class="sxs-lookup"><span data-stu-id="64bbb-133">String</span></span>|<span data-ttu-id="64bbb-134">[Devicemanagementsettinginstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)から継承された設定インスタンス ID</span><span class="sxs-lookup"><span data-stu-id="64bbb-134">The setting instance ID Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="64bbb-135">definitionId</span><span class="sxs-lookup"><span data-stu-id="64bbb-135">definitionId</span></span>|<span data-ttu-id="64bbb-136">String</span><span class="sxs-lookup"><span data-stu-id="64bbb-136">String</span></span>|<span data-ttu-id="64bbb-137">[Devicemanagementsettinginstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)から継承されたこのインスタンスの設定定義の ID</span><span class="sxs-lookup"><span data-stu-id="64bbb-137">The ID of the setting definition for this instance Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="64bbb-138">valueJson</span><span class="sxs-lookup"><span data-stu-id="64bbb-138">valueJson</span></span>|<span data-ttu-id="64bbb-139">String</span><span class="sxs-lookup"><span data-stu-id="64bbb-139">String</span></span>|<span data-ttu-id="64bbb-140">[Devicemanagementsettinginstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)から継承された値の JSON 表現</span><span class="sxs-lookup"><span data-stu-id="64bbb-140">JSON representation of the value Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="64bbb-141">value</span><span class="sxs-lookup"><span data-stu-id="64bbb-141">value</span></span>|<span data-ttu-id="64bbb-142">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="64bbb-142">Boolean</span></span>|<span data-ttu-id="64bbb-143">ブール値</span><span class="sxs-lookup"><span data-stu-id="64bbb-143">The boolean value</span></span>|



## <a name="response"></a><span data-ttu-id="64bbb-144">応答</span><span class="sxs-lookup"><span data-stu-id="64bbb-144">Response</span></span>
<span data-ttu-id="64bbb-145">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[deviceManagementBooleanSettingInstance](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="64bbb-145">If successful, this method returns a `200 OK` response code and an updated [deviceManagementBooleanSettingInstance](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="64bbb-146">例</span><span class="sxs-lookup"><span data-stu-id="64bbb-146">Example</span></span>

### <a name="request"></a><span data-ttu-id="64bbb-147">要求</span><span class="sxs-lookup"><span data-stu-id="64bbb-147">Request</span></span>
<span data-ttu-id="64bbb-148">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="64bbb-148">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/settings/{deviceManagementSettingInstanceId}
Content-type: application/json
Content-length: 176

{
  "@odata.type": "#microsoft.graph.deviceManagementBooleanSettingInstance",
  "definitionId": "Definition Id value",
  "valueJson": "Value Json value",
  "value": true
}
```

### <a name="response"></a><span data-ttu-id="64bbb-149">応答</span><span class="sxs-lookup"><span data-stu-id="64bbb-149">Response</span></span>
<span data-ttu-id="64bbb-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="64bbb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 225

{
  "@odata.type": "#microsoft.graph.deviceManagementBooleanSettingInstance",
  "id": "bb9b0041-0041-bb9b-4100-9bbb41009bbb",
  "definitionId": "Definition Id value",
  "valueJson": "Value Json value",
  "value": true
}
```





