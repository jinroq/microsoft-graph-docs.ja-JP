---
title: devicemanagementcollectionsettinginstance の更新
description: devicemanagementcollectionsettinginstance オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: cc551207d46d3ef4f0a6587bb0c2a9daf5f58a4e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32509976"
---
# <a name="update-devicemanagementcollectionsettinginstance"></a><span data-ttu-id="d7b50-103">devicemanagementcollectionsettinginstance の更新</span><span class="sxs-lookup"><span data-stu-id="d7b50-103">Update deviceManagementCollectionSettingInstance</span></span>

> <span data-ttu-id="d7b50-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d7b50-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d7b50-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="d7b50-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d7b50-106">[devicemanagementcollectionsettinginstance](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="d7b50-106">Update the properties of a [deviceManagementCollectionSettingInstance](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d7b50-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="d7b50-107">Prerequisites</span></span>
<span data-ttu-id="d7b50-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d7b50-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d7b50-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d7b50-110">Permission type</span></span>|<span data-ttu-id="d7b50-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="d7b50-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d7b50-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d7b50-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d7b50-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d7b50-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d7b50-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d7b50-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d7b50-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d7b50-115">Not supported.</span></span>|
|<span data-ttu-id="d7b50-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d7b50-116">Application</span></span>|<span data-ttu-id="d7b50-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d7b50-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d7b50-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d7b50-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="d7b50-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d7b50-119">Request headers</span></span>
|<span data-ttu-id="d7b50-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d7b50-120">Header</span></span>|<span data-ttu-id="d7b50-121">値</span><span class="sxs-lookup"><span data-stu-id="d7b50-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d7b50-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d7b50-122">Authorization</span></span>|<span data-ttu-id="d7b50-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="d7b50-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d7b50-124">承諾</span><span class="sxs-lookup"><span data-stu-id="d7b50-124">Accept</span></span>|<span data-ttu-id="d7b50-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d7b50-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d7b50-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="d7b50-126">Request body</span></span>
<span data-ttu-id="d7b50-127">要求本文で、 [devicemanagementcollectionsettinginstance](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="d7b50-127">In the request body, supply a JSON representation for the [deviceManagementCollectionSettingInstance](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md) object.</span></span>

<span data-ttu-id="d7b50-128">次の表に、 [devicemanagementcollectionsettinginstance](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="d7b50-128">The following table shows the properties that are required when you create the [deviceManagementCollectionSettingInstance](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md).</span></span>

|<span data-ttu-id="d7b50-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d7b50-129">Property</span></span>|<span data-ttu-id="d7b50-130">型</span><span class="sxs-lookup"><span data-stu-id="d7b50-130">Type</span></span>|<span data-ttu-id="d7b50-131">説明</span><span class="sxs-lookup"><span data-stu-id="d7b50-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d7b50-132">id</span><span class="sxs-lookup"><span data-stu-id="d7b50-132">id</span></span>|<span data-ttu-id="d7b50-133">String</span><span class="sxs-lookup"><span data-stu-id="d7b50-133">String</span></span>|<span data-ttu-id="d7b50-134">[devicemanagementsettinginstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)から継承された設定インスタンス ID</span><span class="sxs-lookup"><span data-stu-id="d7b50-134">The setting instance ID Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="d7b50-135">definitionId</span><span class="sxs-lookup"><span data-stu-id="d7b50-135">definitionId</span></span>|<span data-ttu-id="d7b50-136">String</span><span class="sxs-lookup"><span data-stu-id="d7b50-136">String</span></span>|<span data-ttu-id="d7b50-137">[devicemanagementsettinginstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)から継承されたこのインスタンスの設定定義の ID</span><span class="sxs-lookup"><span data-stu-id="d7b50-137">The ID of the setting definition for this instance Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="d7b50-138">valuejson</span><span class="sxs-lookup"><span data-stu-id="d7b50-138">valueJson</span></span>|<span data-ttu-id="d7b50-139">String</span><span class="sxs-lookup"><span data-stu-id="d7b50-139">String</span></span>|<span data-ttu-id="d7b50-140">[devicemanagementsettinginstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)から継承された値の JSON 表現</span><span class="sxs-lookup"><span data-stu-id="d7b50-140">JSON representation of the value Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|



## <a name="response"></a><span data-ttu-id="d7b50-141">応答</span><span class="sxs-lookup"><span data-stu-id="d7b50-141">Response</span></span>
<span data-ttu-id="d7b50-142">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[devicemanagementcollectionsettinginstance](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="d7b50-142">If successful, this method returns a `200 OK` response code and an updated [deviceManagementCollectionSettingInstance](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d7b50-143">例</span><span class="sxs-lookup"><span data-stu-id="d7b50-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="d7b50-144">要求</span><span class="sxs-lookup"><span data-stu-id="d7b50-144">Request</span></span>
<span data-ttu-id="d7b50-145">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="d7b50-145">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d7b50-146">応答</span><span class="sxs-lookup"><span data-stu-id="d7b50-146">Response</span></span>
<span data-ttu-id="d7b50-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="d7b50-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





