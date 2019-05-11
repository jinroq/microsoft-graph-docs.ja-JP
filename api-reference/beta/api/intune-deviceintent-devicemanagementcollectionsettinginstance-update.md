---
title: DeviceManagementCollectionSettingInstance の更新
description: DeviceManagementCollectionSettingInstance オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1cd6c40b208b1f8e87a076a06726bac9d26cd704
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33916588"
---
# <a name="update-devicemanagementcollectionsettinginstance"></a><span data-ttu-id="a5192-103">DeviceManagementCollectionSettingInstance の更新</span><span class="sxs-lookup"><span data-stu-id="a5192-103">Update deviceManagementCollectionSettingInstance</span></span>

> <span data-ttu-id="a5192-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a5192-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a5192-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="a5192-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a5192-106">[Devicemanagementcollectionsettinginstance](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="a5192-106">Update the properties of a [deviceManagementCollectionSettingInstance](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a5192-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="a5192-107">Prerequisites</span></span>
<span data-ttu-id="a5192-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a5192-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a5192-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a5192-110">Permission type</span></span>|<span data-ttu-id="a5192-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="a5192-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a5192-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a5192-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a5192-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a5192-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a5192-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a5192-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a5192-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a5192-115">Not supported.</span></span>|
|<span data-ttu-id="a5192-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a5192-116">Application</span></span>|<span data-ttu-id="a5192-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a5192-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a5192-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a5192-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="a5192-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a5192-119">Request headers</span></span>
|<span data-ttu-id="a5192-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a5192-120">Header</span></span>|<span data-ttu-id="a5192-121">値</span><span class="sxs-lookup"><span data-stu-id="a5192-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a5192-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a5192-122">Authorization</span></span>|<span data-ttu-id="a5192-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="a5192-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a5192-124">承諾</span><span class="sxs-lookup"><span data-stu-id="a5192-124">Accept</span></span>|<span data-ttu-id="a5192-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a5192-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a5192-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="a5192-126">Request body</span></span>
<span data-ttu-id="a5192-127">要求本文で、 [Devicemanagementcollectionsettinginstance](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="a5192-127">In the request body, supply a JSON representation for the [deviceManagementCollectionSettingInstance](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md) object.</span></span>

<span data-ttu-id="a5192-128">次の表に、 [Devicemanagementcollectionsettinginstance](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="a5192-128">The following table shows the properties that are required when you create the [deviceManagementCollectionSettingInstance](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md).</span></span>

|<span data-ttu-id="a5192-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a5192-129">Property</span></span>|<span data-ttu-id="a5192-130">型</span><span class="sxs-lookup"><span data-stu-id="a5192-130">Type</span></span>|<span data-ttu-id="a5192-131">説明</span><span class="sxs-lookup"><span data-stu-id="a5192-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a5192-132">id</span><span class="sxs-lookup"><span data-stu-id="a5192-132">id</span></span>|<span data-ttu-id="a5192-133">String</span><span class="sxs-lookup"><span data-stu-id="a5192-133">String</span></span>|<span data-ttu-id="a5192-134">[Devicemanagementsettinginstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)から継承された設定インスタンス ID</span><span class="sxs-lookup"><span data-stu-id="a5192-134">The setting instance ID Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="a5192-135">definitionId</span><span class="sxs-lookup"><span data-stu-id="a5192-135">definitionId</span></span>|<span data-ttu-id="a5192-136">String</span><span class="sxs-lookup"><span data-stu-id="a5192-136">String</span></span>|<span data-ttu-id="a5192-137">[Devicemanagementsettinginstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)から継承されたこのインスタンスの設定定義の ID</span><span class="sxs-lookup"><span data-stu-id="a5192-137">The ID of the setting definition for this instance Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="a5192-138">valueJson</span><span class="sxs-lookup"><span data-stu-id="a5192-138">valueJson</span></span>|<span data-ttu-id="a5192-139">String</span><span class="sxs-lookup"><span data-stu-id="a5192-139">String</span></span>|<span data-ttu-id="a5192-140">[Devicemanagementsettinginstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)から継承された値の JSON 表現</span><span class="sxs-lookup"><span data-stu-id="a5192-140">JSON representation of the value Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|



## <a name="response"></a><span data-ttu-id="a5192-141">応答</span><span class="sxs-lookup"><span data-stu-id="a5192-141">Response</span></span>
<span data-ttu-id="a5192-142">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[Devicemanagementcollectionsettinginstance](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="a5192-142">If successful, this method returns a `200 OK` response code and an updated [deviceManagementCollectionSettingInstance](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a5192-143">例</span><span class="sxs-lookup"><span data-stu-id="a5192-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="a5192-144">要求</span><span class="sxs-lookup"><span data-stu-id="a5192-144">Request</span></span>
<span data-ttu-id="a5192-145">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="a5192-145">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/settings/{deviceManagementSettingInstanceId}
Content-type: application/json
Content-length: 161

{
  "@odata.type": "#microsoft.graph.deviceManagementCollectionSettingInstance",
  "definitionId": "Definition Id value",
  "valueJson": "Value Json value"
}
```

### <a name="response"></a><span data-ttu-id="a5192-146">応答</span><span class="sxs-lookup"><span data-stu-id="a5192-146">Response</span></span>
<span data-ttu-id="a5192-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="a5192-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 210

{
  "@odata.type": "#microsoft.graph.deviceManagementCollectionSettingInstance",
  "id": "6ce278f7-78f7-6ce2-f778-e26cf778e26c",
  "definitionId": "Definition Id value",
  "valueJson": "Value Json value"
}
```




