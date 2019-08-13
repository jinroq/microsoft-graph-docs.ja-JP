---
title: DeviceManagementComplexSettingInstance の作成
description: 新しい deviceManagementComplexSettingInstance オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: bd7cc4a8775a66fdc258dcf33f30cd6de2289ee0
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36343812"
---
# <a name="create-devicemanagementcomplexsettinginstance"></a><span data-ttu-id="6e031-103">DeviceManagementComplexSettingInstance の作成</span><span class="sxs-lookup"><span data-stu-id="6e031-103">Create deviceManagementComplexSettingInstance</span></span>

> <span data-ttu-id="6e031-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6e031-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6e031-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="6e031-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6e031-106">新しい[Devicemanagementcomplexsettinginstance](../resources/intune-deviceintent-devicemanagementcomplexsettinginstance.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="6e031-106">Create a new [deviceManagementComplexSettingInstance](../resources/intune-deviceintent-devicemanagementcomplexsettinginstance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6e031-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="6e031-107">Prerequisites</span></span>
<span data-ttu-id="6e031-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6e031-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6e031-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="6e031-110">Permission type</span></span>|<span data-ttu-id="6e031-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="6e031-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6e031-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="6e031-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6e031-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6e031-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6e031-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="6e031-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6e031-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6e031-115">Not supported.</span></span>|
|<span data-ttu-id="6e031-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="6e031-116">Application</span></span>|<span data-ttu-id="6e031-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6e031-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6e031-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="6e031-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="6e031-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6e031-119">Request headers</span></span>
|<span data-ttu-id="6e031-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6e031-120">Header</span></span>|<span data-ttu-id="6e031-121">値</span><span class="sxs-lookup"><span data-stu-id="6e031-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6e031-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="6e031-122">Authorization</span></span>|<span data-ttu-id="6e031-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="6e031-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6e031-124">承諾</span><span class="sxs-lookup"><span data-stu-id="6e031-124">Accept</span></span>|<span data-ttu-id="6e031-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6e031-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6e031-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="6e031-126">Request body</span></span>
<span data-ttu-id="6e031-127">要求本文で、deviceManagementComplexSettingInstance オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="6e031-127">In the request body, supply a JSON representation for the deviceManagementComplexSettingInstance object.</span></span>

<span data-ttu-id="6e031-128">次の表に、deviceManagementComplexSettingInstance の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="6e031-128">The following table shows the properties that are required when you create the deviceManagementComplexSettingInstance.</span></span>

|<span data-ttu-id="6e031-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6e031-129">Property</span></span>|<span data-ttu-id="6e031-130">型</span><span class="sxs-lookup"><span data-stu-id="6e031-130">Type</span></span>|<span data-ttu-id="6e031-131">説明</span><span class="sxs-lookup"><span data-stu-id="6e031-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6e031-132">id</span><span class="sxs-lookup"><span data-stu-id="6e031-132">id</span></span>|<span data-ttu-id="6e031-133">String</span><span class="sxs-lookup"><span data-stu-id="6e031-133">String</span></span>|<span data-ttu-id="6e031-134">[Devicemanagementsettinginstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)から継承された設定インスタンス ID</span><span class="sxs-lookup"><span data-stu-id="6e031-134">The setting instance ID Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="6e031-135">definitionId</span><span class="sxs-lookup"><span data-stu-id="6e031-135">definitionId</span></span>|<span data-ttu-id="6e031-136">String</span><span class="sxs-lookup"><span data-stu-id="6e031-136">String</span></span>|<span data-ttu-id="6e031-137">[Devicemanagementsettinginstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)から継承されたこのインスタンスの設定定義の ID</span><span class="sxs-lookup"><span data-stu-id="6e031-137">The ID of the setting definition for this instance Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="6e031-138">valueJson</span><span class="sxs-lookup"><span data-stu-id="6e031-138">valueJson</span></span>|<span data-ttu-id="6e031-139">String</span><span class="sxs-lookup"><span data-stu-id="6e031-139">String</span></span>|<span data-ttu-id="6e031-140">[Devicemanagementsettinginstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)から継承された値の JSON 表現</span><span class="sxs-lookup"><span data-stu-id="6e031-140">JSON representation of the value Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|



## <a name="response"></a><span data-ttu-id="6e031-141">応答</span><span class="sxs-lookup"><span data-stu-id="6e031-141">Response</span></span>
<span data-ttu-id="6e031-142">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[Devicemanagementcomplexsettinginstance](../resources/intune-deviceintent-devicemanagementcomplexsettinginstance.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="6e031-142">If successful, this method returns a `201 Created` response code and a [deviceManagementComplexSettingInstance](../resources/intune-deviceintent-devicemanagementcomplexsettinginstance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6e031-143">例</span><span class="sxs-lookup"><span data-stu-id="6e031-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="6e031-144">要求</span><span class="sxs-lookup"><span data-stu-id="6e031-144">Request</span></span>
<span data-ttu-id="6e031-145">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="6e031-145">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/settings
Content-type: application/json
Content-length: 158

{
  "@odata.type": "#microsoft.graph.deviceManagementComplexSettingInstance",
  "definitionId": "Definition Id value",
  "valueJson": "Value Json value"
}
```

### <a name="response"></a><span data-ttu-id="6e031-146">応答</span><span class="sxs-lookup"><span data-stu-id="6e031-146">Response</span></span>
<span data-ttu-id="6e031-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="6e031-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 207

{
  "@odata.type": "#microsoft.graph.deviceManagementComplexSettingInstance",
  "id": "4deb3935-3935-4deb-3539-eb4d3539eb4d",
  "definitionId": "Definition Id value",
  "valueJson": "Value Json value"
}
```






