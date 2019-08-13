---
title: Devicemanagement整数 Settinginstance の作成
description: 新しい Devicemanagement整数 Settinginstance オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 645afa20e3e3e4bd5a0afe4be445c713868eef59
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36343756"
---
# <a name="create-devicemanagementintegersettinginstance"></a><span data-ttu-id="53284-103">Devicemanagement整数 Settinginstance の作成</span><span class="sxs-lookup"><span data-stu-id="53284-103">Create deviceManagementIntegerSettingInstance</span></span>

> <span data-ttu-id="53284-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="53284-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="53284-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="53284-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="53284-106">新しい[Devicemanagement整数 Settinginstance](../resources/intune-deviceintent-devicemanagementintegersettinginstance.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="53284-106">Create a new [deviceManagementIntegerSettingInstance](../resources/intune-deviceintent-devicemanagementintegersettinginstance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="53284-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="53284-107">Prerequisites</span></span>
<span data-ttu-id="53284-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="53284-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="53284-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="53284-110">Permission type</span></span>|<span data-ttu-id="53284-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="53284-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="53284-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="53284-112">Delegated (work or school account)</span></span>|<span data-ttu-id="53284-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="53284-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="53284-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="53284-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="53284-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="53284-115">Not supported.</span></span>|
|<span data-ttu-id="53284-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="53284-116">Application</span></span>|<span data-ttu-id="53284-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="53284-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="53284-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="53284-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="53284-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="53284-119">Request headers</span></span>
|<span data-ttu-id="53284-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="53284-120">Header</span></span>|<span data-ttu-id="53284-121">値</span><span class="sxs-lookup"><span data-stu-id="53284-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="53284-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="53284-122">Authorization</span></span>|<span data-ttu-id="53284-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="53284-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="53284-124">承諾</span><span class="sxs-lookup"><span data-stu-id="53284-124">Accept</span></span>|<span data-ttu-id="53284-125">application/json</span><span class="sxs-lookup"><span data-stu-id="53284-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="53284-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="53284-126">Request body</span></span>
<span data-ttu-id="53284-127">要求本文で、Devicemanagement整数 Settinginstance オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="53284-127">In the request body, supply a JSON representation for the deviceManagementIntegerSettingInstance object.</span></span>

<span data-ttu-id="53284-128">次の表に、Devicemanagement整数 Settinginstance の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="53284-128">The following table shows the properties that are required when you create the deviceManagementIntegerSettingInstance.</span></span>

|<span data-ttu-id="53284-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="53284-129">Property</span></span>|<span data-ttu-id="53284-130">型</span><span class="sxs-lookup"><span data-stu-id="53284-130">Type</span></span>|<span data-ttu-id="53284-131">説明</span><span class="sxs-lookup"><span data-stu-id="53284-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="53284-132">id</span><span class="sxs-lookup"><span data-stu-id="53284-132">id</span></span>|<span data-ttu-id="53284-133">String</span><span class="sxs-lookup"><span data-stu-id="53284-133">String</span></span>|<span data-ttu-id="53284-134">[Devicemanagementsettinginstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)から継承された設定インスタンス ID</span><span class="sxs-lookup"><span data-stu-id="53284-134">The setting instance ID Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="53284-135">definitionId</span><span class="sxs-lookup"><span data-stu-id="53284-135">definitionId</span></span>|<span data-ttu-id="53284-136">String</span><span class="sxs-lookup"><span data-stu-id="53284-136">String</span></span>|<span data-ttu-id="53284-137">[Devicemanagementsettinginstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)から継承されたこのインスタンスの設定定義の ID</span><span class="sxs-lookup"><span data-stu-id="53284-137">The ID of the setting definition for this instance Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="53284-138">valueJson</span><span class="sxs-lookup"><span data-stu-id="53284-138">valueJson</span></span>|<span data-ttu-id="53284-139">String</span><span class="sxs-lookup"><span data-stu-id="53284-139">String</span></span>|<span data-ttu-id="53284-140">[Devicemanagementsettinginstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)から継承された値の JSON 表現</span><span class="sxs-lookup"><span data-stu-id="53284-140">JSON representation of the value Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="53284-141">値</span><span class="sxs-lookup"><span data-stu-id="53284-141">value</span></span>|<span data-ttu-id="53284-142">Int32</span><span class="sxs-lookup"><span data-stu-id="53284-142">Int32</span></span>|<span data-ttu-id="53284-143">整数型 (integer) の値</span><span class="sxs-lookup"><span data-stu-id="53284-143">The integer value</span></span>|



## <a name="response"></a><span data-ttu-id="53284-144">応答</span><span class="sxs-lookup"><span data-stu-id="53284-144">Response</span></span>
<span data-ttu-id="53284-145">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[Devicemanagement整数 settinginstance](../resources/intune-deviceintent-devicemanagementintegersettinginstance.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="53284-145">If successful, this method returns a `201 Created` response code and a [deviceManagementIntegerSettingInstance](../resources/intune-deviceintent-devicemanagementintegersettinginstance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="53284-146">例</span><span class="sxs-lookup"><span data-stu-id="53284-146">Example</span></span>

### <a name="request"></a><span data-ttu-id="53284-147">要求</span><span class="sxs-lookup"><span data-stu-id="53284-147">Request</span></span>
<span data-ttu-id="53284-148">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="53284-148">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/settings
Content-type: application/json
Content-length: 173

{
  "@odata.type": "#microsoft.graph.deviceManagementIntegerSettingInstance",
  "definitionId": "Definition Id value",
  "valueJson": "Value Json value",
  "value": 5
}
```

### <a name="response"></a><span data-ttu-id="53284-149">応答</span><span class="sxs-lookup"><span data-stu-id="53284-149">Response</span></span>
<span data-ttu-id="53284-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="53284-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 222

{
  "@odata.type": "#microsoft.graph.deviceManagementIntegerSettingInstance",
  "id": "60468ce7-8ce7-6046-e78c-4660e78c4660",
  "definitionId": "Definition Id value",
  "valueJson": "Value Json value",
  "value": 5
}
```






