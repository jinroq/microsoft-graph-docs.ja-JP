---
title: DeviceManagementComplexSettingInstance の更新
description: DeviceManagementComplexSettingInstance オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 91c721291177f506bb7af817454ce4dae8cf542e
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34960616"
---
# <a name="update-devicemanagementcomplexsettinginstance"></a><span data-ttu-id="c9e91-103">DeviceManagementComplexSettingInstance の更新</span><span class="sxs-lookup"><span data-stu-id="c9e91-103">Update deviceManagementComplexSettingInstance</span></span>

> <span data-ttu-id="c9e91-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c9e91-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c9e91-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="c9e91-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c9e91-106">[Devicemanagementcomplexsettinginstance](../resources/intune-deviceintent-devicemanagementcomplexsettinginstance.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="c9e91-106">Update the properties of a [deviceManagementComplexSettingInstance](../resources/intune-deviceintent-devicemanagementcomplexsettinginstance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c9e91-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="c9e91-107">Prerequisites</span></span>
<span data-ttu-id="c9e91-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c9e91-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c9e91-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c9e91-110">Permission type</span></span>|<span data-ttu-id="c9e91-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="c9e91-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c9e91-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c9e91-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c9e91-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c9e91-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c9e91-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c9e91-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c9e91-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c9e91-115">Not supported.</span></span>|
|<span data-ttu-id="c9e91-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c9e91-116">Application</span></span>|<span data-ttu-id="c9e91-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c9e91-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c9e91-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c9e91-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="c9e91-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c9e91-119">Request headers</span></span>
|<span data-ttu-id="c9e91-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c9e91-120">Header</span></span>|<span data-ttu-id="c9e91-121">値</span><span class="sxs-lookup"><span data-stu-id="c9e91-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c9e91-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c9e91-122">Authorization</span></span>|<span data-ttu-id="c9e91-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="c9e91-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c9e91-124">承諾</span><span class="sxs-lookup"><span data-stu-id="c9e91-124">Accept</span></span>|<span data-ttu-id="c9e91-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c9e91-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c9e91-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="c9e91-126">Request body</span></span>
<span data-ttu-id="c9e91-127">要求本文で、 [Devicemanagementcomplexsettinginstance](../resources/intune-deviceintent-devicemanagementcomplexsettinginstance.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="c9e91-127">In the request body, supply a JSON representation for the [deviceManagementComplexSettingInstance](../resources/intune-deviceintent-devicemanagementcomplexsettinginstance.md) object.</span></span>

<span data-ttu-id="c9e91-128">次の表に、 [Devicemanagementcomplexsettinginstance](../resources/intune-deviceintent-devicemanagementcomplexsettinginstance.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="c9e91-128">The following table shows the properties that are required when you create the [deviceManagementComplexSettingInstance](../resources/intune-deviceintent-devicemanagementcomplexsettinginstance.md).</span></span>

|<span data-ttu-id="c9e91-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c9e91-129">Property</span></span>|<span data-ttu-id="c9e91-130">型</span><span class="sxs-lookup"><span data-stu-id="c9e91-130">Type</span></span>|<span data-ttu-id="c9e91-131">説明</span><span class="sxs-lookup"><span data-stu-id="c9e91-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c9e91-132">id</span><span class="sxs-lookup"><span data-stu-id="c9e91-132">id</span></span>|<span data-ttu-id="c9e91-133">String</span><span class="sxs-lookup"><span data-stu-id="c9e91-133">String</span></span>|<span data-ttu-id="c9e91-134">[Devicemanagementsettinginstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)から継承された設定インスタンス ID</span><span class="sxs-lookup"><span data-stu-id="c9e91-134">The setting instance ID Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="c9e91-135">definitionId</span><span class="sxs-lookup"><span data-stu-id="c9e91-135">definitionId</span></span>|<span data-ttu-id="c9e91-136">String</span><span class="sxs-lookup"><span data-stu-id="c9e91-136">String</span></span>|<span data-ttu-id="c9e91-137">[Devicemanagementsettinginstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)から継承されたこのインスタンスの設定定義の ID</span><span class="sxs-lookup"><span data-stu-id="c9e91-137">The ID of the setting definition for this instance Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="c9e91-138">valueJson</span><span class="sxs-lookup"><span data-stu-id="c9e91-138">valueJson</span></span>|<span data-ttu-id="c9e91-139">String</span><span class="sxs-lookup"><span data-stu-id="c9e91-139">String</span></span>|<span data-ttu-id="c9e91-140">[Devicemanagementsettinginstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)から継承された値の JSON 表現</span><span class="sxs-lookup"><span data-stu-id="c9e91-140">JSON representation of the value Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|



## <a name="response"></a><span data-ttu-id="c9e91-141">応答</span><span class="sxs-lookup"><span data-stu-id="c9e91-141">Response</span></span>
<span data-ttu-id="c9e91-142">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[Devicemanagementcomplexsettinginstance](../resources/intune-deviceintent-devicemanagementcomplexsettinginstance.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="c9e91-142">If successful, this method returns a `200 OK` response code and an updated [deviceManagementComplexSettingInstance](../resources/intune-deviceintent-devicemanagementcomplexsettinginstance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c9e91-143">例</span><span class="sxs-lookup"><span data-stu-id="c9e91-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="c9e91-144">要求</span><span class="sxs-lookup"><span data-stu-id="c9e91-144">Request</span></span>
<span data-ttu-id="c9e91-145">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="c9e91-145">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/settings/{deviceManagementSettingInstanceId}
Content-type: application/json
Content-length: 158

{
  "@odata.type": "#microsoft.graph.deviceManagementComplexSettingInstance",
  "definitionId": "Definition Id value",
  "valueJson": "Value Json value"
}
```

### <a name="response"></a><span data-ttu-id="c9e91-146">応答</span><span class="sxs-lookup"><span data-stu-id="c9e91-146">Response</span></span>
<span data-ttu-id="c9e91-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="c9e91-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 207

{
  "@odata.type": "#microsoft.graph.deviceManagementComplexSettingInstance",
  "id": "4deb3935-3935-4deb-3539-eb4d3539eb4d",
  "definitionId": "Definition Id value",
  "valueJson": "Value Json value"
}
```





