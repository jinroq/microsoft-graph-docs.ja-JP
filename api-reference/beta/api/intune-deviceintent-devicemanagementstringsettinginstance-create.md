---
title: DeviceManagementStringSettingInstance の作成
description: 新しい deviceManagementStringSettingInstance オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d57cea9f9bb41d0ebb4ea2a61fb332488cd5ef1c
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33915790"
---
# <a name="create-devicemanagementstringsettinginstance"></a><span data-ttu-id="35c53-103">DeviceManagementStringSettingInstance の作成</span><span class="sxs-lookup"><span data-stu-id="35c53-103">Create deviceManagementStringSettingInstance</span></span>

> <span data-ttu-id="35c53-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="35c53-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="35c53-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="35c53-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="35c53-106">新しい[Devicemanagementstringsettinginstance](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="35c53-106">Create a new [deviceManagementStringSettingInstance](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="35c53-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="35c53-107">Prerequisites</span></span>
<span data-ttu-id="35c53-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="35c53-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="35c53-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="35c53-110">Permission type</span></span>|<span data-ttu-id="35c53-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="35c53-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="35c53-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="35c53-112">Delegated (work or school account)</span></span>|<span data-ttu-id="35c53-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="35c53-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="35c53-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="35c53-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="35c53-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="35c53-115">Not supported.</span></span>|
|<span data-ttu-id="35c53-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="35c53-116">Application</span></span>|<span data-ttu-id="35c53-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="35c53-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="35c53-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="35c53-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="35c53-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="35c53-119">Request headers</span></span>
|<span data-ttu-id="35c53-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="35c53-120">Header</span></span>|<span data-ttu-id="35c53-121">値</span><span class="sxs-lookup"><span data-stu-id="35c53-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="35c53-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="35c53-122">Authorization</span></span>|<span data-ttu-id="35c53-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="35c53-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="35c53-124">承諾</span><span class="sxs-lookup"><span data-stu-id="35c53-124">Accept</span></span>|<span data-ttu-id="35c53-125">application/json</span><span class="sxs-lookup"><span data-stu-id="35c53-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="35c53-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="35c53-126">Request body</span></span>
<span data-ttu-id="35c53-127">要求本文で、deviceManagementStringSettingInstance オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="35c53-127">In the request body, supply a JSON representation for the deviceManagementStringSettingInstance object.</span></span>

<span data-ttu-id="35c53-128">次の表に、deviceManagementStringSettingInstance の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="35c53-128">The following table shows the properties that are required when you create the deviceManagementStringSettingInstance.</span></span>

|<span data-ttu-id="35c53-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="35c53-129">Property</span></span>|<span data-ttu-id="35c53-130">型</span><span class="sxs-lookup"><span data-stu-id="35c53-130">Type</span></span>|<span data-ttu-id="35c53-131">説明</span><span class="sxs-lookup"><span data-stu-id="35c53-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="35c53-132">id</span><span class="sxs-lookup"><span data-stu-id="35c53-132">id</span></span>|<span data-ttu-id="35c53-133">String</span><span class="sxs-lookup"><span data-stu-id="35c53-133">String</span></span>|<span data-ttu-id="35c53-134">[Devicemanagementsettinginstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)から継承された設定インスタンス ID</span><span class="sxs-lookup"><span data-stu-id="35c53-134">The setting instance ID Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="35c53-135">definitionId</span><span class="sxs-lookup"><span data-stu-id="35c53-135">definitionId</span></span>|<span data-ttu-id="35c53-136">String</span><span class="sxs-lookup"><span data-stu-id="35c53-136">String</span></span>|<span data-ttu-id="35c53-137">[Devicemanagementsettinginstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)から継承されたこのインスタンスの設定定義の ID</span><span class="sxs-lookup"><span data-stu-id="35c53-137">The ID of the setting definition for this instance Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="35c53-138">valueJson</span><span class="sxs-lookup"><span data-stu-id="35c53-138">valueJson</span></span>|<span data-ttu-id="35c53-139">String</span><span class="sxs-lookup"><span data-stu-id="35c53-139">String</span></span>|<span data-ttu-id="35c53-140">[Devicemanagementsettinginstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)から継承された値の JSON 表現</span><span class="sxs-lookup"><span data-stu-id="35c53-140">JSON representation of the value Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="35c53-141">value</span><span class="sxs-lookup"><span data-stu-id="35c53-141">value</span></span>|<span data-ttu-id="35c53-142">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="35c53-142">String</span></span>|<span data-ttu-id="35c53-143">文字列型 (string) の値</span><span class="sxs-lookup"><span data-stu-id="35c53-143">The string value</span></span>|



## <a name="response"></a><span data-ttu-id="35c53-144">応答</span><span class="sxs-lookup"><span data-stu-id="35c53-144">Response</span></span>
<span data-ttu-id="35c53-145">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[Devicemanagementstringsettinginstance](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="35c53-145">If successful, this method returns a `201 Created` response code and a [deviceManagementStringSettingInstance](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="35c53-146">例</span><span class="sxs-lookup"><span data-stu-id="35c53-146">Example</span></span>

### <a name="request"></a><span data-ttu-id="35c53-147">要求</span><span class="sxs-lookup"><span data-stu-id="35c53-147">Request</span></span>
<span data-ttu-id="35c53-148">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="35c53-148">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/settings
Content-type: application/json
Content-length: 184

{
  "@odata.type": "#microsoft.graph.deviceManagementStringSettingInstance",
  "definitionId": "Definition Id value",
  "valueJson": "Value Json value",
  "value": "Value value"
}
```

### <a name="response"></a><span data-ttu-id="35c53-149">応答</span><span class="sxs-lookup"><span data-stu-id="35c53-149">Response</span></span>
<span data-ttu-id="35c53-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="35c53-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




