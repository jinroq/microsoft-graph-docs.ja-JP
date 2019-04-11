---
title: devicemanagementcollectionsettinginstance の作成
description: 新しい devicemanagementcollectionsettinginstance オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f141460a8f67d257702c9f307970f710ef19b0d3
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31801821"
---
# <a name="create-devicemanagementcollectionsettinginstance"></a><span data-ttu-id="cc8bc-103">devicemanagementcollectionsettinginstance の作成</span><span class="sxs-lookup"><span data-stu-id="cc8bc-103">Create deviceManagementCollectionSettingInstance</span></span>

> <span data-ttu-id="cc8bc-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cc8bc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cc8bc-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="cc8bc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cc8bc-106">新しい[devicemanagementcollectionsettinginstance](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="cc8bc-106">Create a new [deviceManagementCollectionSettingInstance](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cc8bc-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="cc8bc-107">Prerequisites</span></span>
<span data-ttu-id="cc8bc-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="cc8bc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cc8bc-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="cc8bc-110">Permission type</span></span>|<span data-ttu-id="cc8bc-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="cc8bc-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cc8bc-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="cc8bc-112">Delegated (work or school account)</span></span>|<span data-ttu-id="cc8bc-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cc8bc-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="cc8bc-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="cc8bc-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cc8bc-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cc8bc-115">Not supported.</span></span>|
|<span data-ttu-id="cc8bc-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="cc8bc-116">Application</span></span>|<span data-ttu-id="cc8bc-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cc8bc-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cc8bc-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="cc8bc-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="cc8bc-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="cc8bc-119">Request headers</span></span>
|<span data-ttu-id="cc8bc-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="cc8bc-120">Header</span></span>|<span data-ttu-id="cc8bc-121">値</span><span class="sxs-lookup"><span data-stu-id="cc8bc-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cc8bc-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="cc8bc-122">Authorization</span></span>|<span data-ttu-id="cc8bc-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="cc8bc-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cc8bc-124">承諾</span><span class="sxs-lookup"><span data-stu-id="cc8bc-124">Accept</span></span>|<span data-ttu-id="cc8bc-125">application/json</span><span class="sxs-lookup"><span data-stu-id="cc8bc-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cc8bc-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="cc8bc-126">Request body</span></span>
<span data-ttu-id="cc8bc-127">要求本文で、devicemanagementcollectionsettinginstance オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="cc8bc-127">In the request body, supply a JSON representation for the deviceManagementCollectionSettingInstance object.</span></span>

<span data-ttu-id="cc8bc-128">次の表に、devicemanagementcollectionsettinginstance の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="cc8bc-128">The following table shows the properties that are required when you create the deviceManagementCollectionSettingInstance.</span></span>

|<span data-ttu-id="cc8bc-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cc8bc-129">Property</span></span>|<span data-ttu-id="cc8bc-130">型</span><span class="sxs-lookup"><span data-stu-id="cc8bc-130">Type</span></span>|<span data-ttu-id="cc8bc-131">説明</span><span class="sxs-lookup"><span data-stu-id="cc8bc-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cc8bc-132">id</span><span class="sxs-lookup"><span data-stu-id="cc8bc-132">id</span></span>|<span data-ttu-id="cc8bc-133">String</span><span class="sxs-lookup"><span data-stu-id="cc8bc-133">String</span></span>|<span data-ttu-id="cc8bc-134">[devicemanagementsettinginstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)から継承された設定インスタンス ID</span><span class="sxs-lookup"><span data-stu-id="cc8bc-134">The setting instance ID Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="cc8bc-135">definitionId</span><span class="sxs-lookup"><span data-stu-id="cc8bc-135">definitionId</span></span>|<span data-ttu-id="cc8bc-136">文字列</span><span class="sxs-lookup"><span data-stu-id="cc8bc-136">String</span></span>|<span data-ttu-id="cc8bc-137">[devicemanagementsettinginstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)から継承されたこのインスタンスの設定定義の ID</span><span class="sxs-lookup"><span data-stu-id="cc8bc-137">The ID of the setting definition for this instance Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="cc8bc-138">valuejson</span><span class="sxs-lookup"><span data-stu-id="cc8bc-138">valueJson</span></span>|<span data-ttu-id="cc8bc-139">文字列</span><span class="sxs-lookup"><span data-stu-id="cc8bc-139">String</span></span>|<span data-ttu-id="cc8bc-140">[devicemanagementsettinginstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)から継承された値の JSON 表現</span><span class="sxs-lookup"><span data-stu-id="cc8bc-140">JSON representation of the value Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|



## <a name="response"></a><span data-ttu-id="cc8bc-141">応答</span><span class="sxs-lookup"><span data-stu-id="cc8bc-141">Response</span></span>
<span data-ttu-id="cc8bc-142">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[devicemanagementcollectionsettinginstance](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="cc8bc-142">If successful, this method returns a `201 Created` response code and a [deviceManagementCollectionSettingInstance](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cc8bc-143">例</span><span class="sxs-lookup"><span data-stu-id="cc8bc-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="cc8bc-144">要求</span><span class="sxs-lookup"><span data-stu-id="cc8bc-144">Request</span></span>
<span data-ttu-id="cc8bc-145">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="cc8bc-145">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/settings
Content-type: application/json
Content-length: 161

{
  "@odata.type": "#microsoft.graph.deviceManagementCollectionSettingInstance",
  "definitionId": "Definition Id value",
  "valueJson": "Value Json value"
}
```

### <a name="response"></a><span data-ttu-id="cc8bc-146">応答</span><span class="sxs-lookup"><span data-stu-id="cc8bc-146">Response</span></span>
<span data-ttu-id="cc8bc-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="cc8bc-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 210

{
  "@odata.type": "#microsoft.graph.deviceManagementCollectionSettingInstance",
  "id": "6ce278f7-78f7-6ce2-f778-e26cf778e26c",
  "definitionId": "Definition Id value",
  "valueJson": "Value Json value"
}
```





