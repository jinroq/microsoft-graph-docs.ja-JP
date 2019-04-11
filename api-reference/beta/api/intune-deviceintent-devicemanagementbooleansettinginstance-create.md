---
title: deviceManagementBooleanSettingInstance を作成する
description: 新しい deviceManagementBooleanSettingInstance オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 239fef02ae06cbacc193c06de03fdb6ba3dbedb9
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31770467"
---
# <a name="create-devicemanagementbooleansettinginstance"></a><span data-ttu-id="1f750-103">deviceManagementBooleanSettingInstance を作成する</span><span class="sxs-lookup"><span data-stu-id="1f750-103">Create deviceManagementBooleanSettingInstance</span></span>

> <span data-ttu-id="1f750-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1f750-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1f750-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="1f750-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1f750-106">新しい[deviceManagementBooleanSettingInstance](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="1f750-106">Create a new [deviceManagementBooleanSettingInstance](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1f750-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="1f750-107">Prerequisites</span></span>
<span data-ttu-id="1f750-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1f750-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1f750-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1f750-110">Permission type</span></span>|<span data-ttu-id="1f750-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="1f750-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1f750-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="1f750-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1f750-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1f750-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1f750-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1f750-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1f750-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1f750-115">Not supported.</span></span>|
|<span data-ttu-id="1f750-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1f750-116">Application</span></span>|<span data-ttu-id="1f750-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1f750-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1f750-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1f750-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/intents/{deviceManagementIntentId}/settings
POST /deviceManagement/templates/{deviceManagementTemplateId}/settings
POST /deviceManagement/intents/{deviceManagementIntentId}/categories/{deviceManagementIntentSettingCategoryId}/settings
POST /deviceManagement/templates/{deviceManagementTemplateId}/categories/{deviceManagementTemplateSettingCategoryId}/recommendedSettings
```

## <a name="request-headers"></a><span data-ttu-id="1f750-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1f750-119">Request headers</span></span>
|<span data-ttu-id="1f750-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1f750-120">Header</span></span>|<span data-ttu-id="1f750-121">値</span><span class="sxs-lookup"><span data-stu-id="1f750-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1f750-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="1f750-122">Authorization</span></span>|<span data-ttu-id="1f750-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="1f750-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1f750-124">承諾</span><span class="sxs-lookup"><span data-stu-id="1f750-124">Accept</span></span>|<span data-ttu-id="1f750-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1f750-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1f750-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="1f750-126">Request body</span></span>
<span data-ttu-id="1f750-127">要求本文で、deviceManagementBooleanSettingInstance オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="1f750-127">In the request body, supply a JSON representation for the deviceManagementBooleanSettingInstance object.</span></span>

<span data-ttu-id="1f750-128">次の表に、deviceManagementBooleanSettingInstance の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="1f750-128">The following table shows the properties that are required when you create the deviceManagementBooleanSettingInstance.</span></span>

|<span data-ttu-id="1f750-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1f750-129">Property</span></span>|<span data-ttu-id="1f750-130">型</span><span class="sxs-lookup"><span data-stu-id="1f750-130">Type</span></span>|<span data-ttu-id="1f750-131">説明</span><span class="sxs-lookup"><span data-stu-id="1f750-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1f750-132">id</span><span class="sxs-lookup"><span data-stu-id="1f750-132">id</span></span>|<span data-ttu-id="1f750-133">String</span><span class="sxs-lookup"><span data-stu-id="1f750-133">String</span></span>|<span data-ttu-id="1f750-134">[devicemanagementsettinginstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)から継承された設定インスタンス ID</span><span class="sxs-lookup"><span data-stu-id="1f750-134">The setting instance ID Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="1f750-135">definitionId</span><span class="sxs-lookup"><span data-stu-id="1f750-135">definitionId</span></span>|<span data-ttu-id="1f750-136">文字列</span><span class="sxs-lookup"><span data-stu-id="1f750-136">String</span></span>|<span data-ttu-id="1f750-137">[devicemanagementsettinginstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)から継承されたこのインスタンスの設定定義の ID</span><span class="sxs-lookup"><span data-stu-id="1f750-137">The ID of the setting definition for this instance Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="1f750-138">valuejson</span><span class="sxs-lookup"><span data-stu-id="1f750-138">valueJson</span></span>|<span data-ttu-id="1f750-139">文字列</span><span class="sxs-lookup"><span data-stu-id="1f750-139">String</span></span>|<span data-ttu-id="1f750-140">[devicemanagementsettinginstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)から継承された値の JSON 表現</span><span class="sxs-lookup"><span data-stu-id="1f750-140">JSON representation of the value Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="1f750-141">value</span><span class="sxs-lookup"><span data-stu-id="1f750-141">value</span></span>|<span data-ttu-id="1f750-142">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="1f750-142">Boolean</span></span>|<span data-ttu-id="1f750-143">ブール値</span><span class="sxs-lookup"><span data-stu-id="1f750-143">The boolean value</span></span>|



## <a name="response"></a><span data-ttu-id="1f750-144">応答</span><span class="sxs-lookup"><span data-stu-id="1f750-144">Response</span></span>
<span data-ttu-id="1f750-145">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[deviceManagementBooleanSettingInstance](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="1f750-145">If successful, this method returns a `201 Created` response code and a [deviceManagementBooleanSettingInstance](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1f750-146">例</span><span class="sxs-lookup"><span data-stu-id="1f750-146">Example</span></span>

### <a name="request"></a><span data-ttu-id="1f750-147">要求</span><span class="sxs-lookup"><span data-stu-id="1f750-147">Request</span></span>
<span data-ttu-id="1f750-148">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="1f750-148">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/settings
Content-type: application/json
Content-length: 176

{
  "@odata.type": "#microsoft.graph.deviceManagementBooleanSettingInstance",
  "definitionId": "Definition Id value",
  "valueJson": "Value Json value",
  "value": true
}
```

### <a name="response"></a><span data-ttu-id="1f750-149">応答</span><span class="sxs-lookup"><span data-stu-id="1f750-149">Response</span></span>
<span data-ttu-id="1f750-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="1f750-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





