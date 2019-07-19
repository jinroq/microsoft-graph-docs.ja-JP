---
title: DeviceManagementTemplate の更新
description: DeviceManagementTemplate オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 570e8d97b66db1cd34b3c7ffc84d90da943bf6e6
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34959734"
---
# <a name="update-devicemanagementtemplate"></a><span data-ttu-id="d1fef-103">DeviceManagementTemplate の更新</span><span class="sxs-lookup"><span data-stu-id="d1fef-103">Update deviceManagementTemplate</span></span>

> <span data-ttu-id="d1fef-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d1fef-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d1fef-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="d1fef-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d1fef-106">[Devicemanagementtemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="d1fef-106">Update the properties of a [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d1fef-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="d1fef-107">Prerequisites</span></span>
<span data-ttu-id="d1fef-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d1fef-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d1fef-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d1fef-110">Permission type</span></span>|<span data-ttu-id="d1fef-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="d1fef-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d1fef-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d1fef-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d1fef-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d1fef-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d1fef-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d1fef-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d1fef-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d1fef-115">Not supported.</span></span>|
|<span data-ttu-id="d1fef-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d1fef-116">Application</span></span>|<span data-ttu-id="d1fef-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d1fef-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d1fef-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d1fef-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/templates/{deviceManagementTemplateId}
PATCH /deviceManagement/templates/{deviceManagementTemplateId}/migratableTo/{deviceManagementTemplateId}
```

## <a name="request-headers"></a><span data-ttu-id="d1fef-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d1fef-119">Request headers</span></span>
|<span data-ttu-id="d1fef-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d1fef-120">Header</span></span>|<span data-ttu-id="d1fef-121">値</span><span class="sxs-lookup"><span data-stu-id="d1fef-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d1fef-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d1fef-122">Authorization</span></span>|<span data-ttu-id="d1fef-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="d1fef-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d1fef-124">承諾</span><span class="sxs-lookup"><span data-stu-id="d1fef-124">Accept</span></span>|<span data-ttu-id="d1fef-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d1fef-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d1fef-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="d1fef-126">Request body</span></span>
<span data-ttu-id="d1fef-127">要求本文で、 [Devicemanagementtemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="d1fef-127">In the request body, supply a JSON representation for the [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md) object.</span></span>

<span data-ttu-id="d1fef-128">次の表に、 [Devicemanagementtemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="d1fef-128">The following table shows the properties that are required when you create the [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md).</span></span>

|<span data-ttu-id="d1fef-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d1fef-129">Property</span></span>|<span data-ttu-id="d1fef-130">型</span><span class="sxs-lookup"><span data-stu-id="d1fef-130">Type</span></span>|<span data-ttu-id="d1fef-131">説明</span><span class="sxs-lookup"><span data-stu-id="d1fef-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d1fef-132">id</span><span class="sxs-lookup"><span data-stu-id="d1fef-132">id</span></span>|<span data-ttu-id="d1fef-133">文字列</span><span class="sxs-lookup"><span data-stu-id="d1fef-133">String</span></span>|<span data-ttu-id="d1fef-134">テンプレート ID</span><span class="sxs-lookup"><span data-stu-id="d1fef-134">The template ID</span></span>|
|<span data-ttu-id="d1fef-135">displayName</span><span class="sxs-lookup"><span data-stu-id="d1fef-135">displayName</span></span>|<span data-ttu-id="d1fef-136">String</span><span class="sxs-lookup"><span data-stu-id="d1fef-136">String</span></span>|<span data-ttu-id="d1fef-137">テンプレートの表示名</span><span class="sxs-lookup"><span data-stu-id="d1fef-137">The template's display name</span></span>|
|<span data-ttu-id="d1fef-138">description</span><span class="sxs-lookup"><span data-stu-id="d1fef-138">description</span></span>|<span data-ttu-id="d1fef-139">String</span><span class="sxs-lookup"><span data-stu-id="d1fef-139">String</span></span>|<span data-ttu-id="d1fef-140">テンプレートの説明</span><span class="sxs-lookup"><span data-stu-id="d1fef-140">The template's description</span></span>|
|<span data-ttu-id="d1fef-141">versionInfo</span><span class="sxs-lookup"><span data-stu-id="d1fef-141">versionInfo</span></span>|<span data-ttu-id="d1fef-142">String</span><span class="sxs-lookup"><span data-stu-id="d1fef-142">String</span></span>|<span data-ttu-id="d1fef-143">テンプレートのバージョン情報</span><span class="sxs-lookup"><span data-stu-id="d1fef-143">The template's version information</span></span>|
|<span data-ttu-id="d1fef-144">isDeprecated</span><span class="sxs-lookup"><span data-stu-id="d1fef-144">isDeprecated</span></span>|<span data-ttu-id="d1fef-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1fef-145">Boolean</span></span>|<span data-ttu-id="d1fef-146">テンプレートが非推奨になっているか、使用されていません。</span><span class="sxs-lookup"><span data-stu-id="d1fef-146">The template is deprecated or not.</span></span> <span data-ttu-id="d1fef-147">推奨されていないテンプレートからは、インテントを作成できません。</span><span class="sxs-lookup"><span data-stu-id="d1fef-147">Intents cannot be created from a deprecated template.</span></span>|
|<span data-ttu-id="d1fef-148">intentCount</span><span class="sxs-lookup"><span data-stu-id="d1fef-148">intentCount</span></span>|<span data-ttu-id="d1fef-149">Int32</span><span class="sxs-lookup"><span data-stu-id="d1fef-149">Int32</span></span>|<span data-ttu-id="d1fef-150">このテンプレートから作成されたインテントの数。</span><span class="sxs-lookup"><span data-stu-id="d1fef-150">Number of Intents created from this template.</span></span>|
|<span data-ttu-id="d1fef-151">templateType</span><span class="sxs-lookup"><span data-stu-id="d1fef-151">templateType</span></span>|[<span data-ttu-id="d1fef-152">deviceManagementTemplateType</span><span class="sxs-lookup"><span data-stu-id="d1fef-152">deviceManagementTemplateType</span></span>](../resources/intune-deviceintent-devicemanagementtemplatetype.md)|<span data-ttu-id="d1fef-153">テンプレートの種類を示します。</span><span class="sxs-lookup"><span data-stu-id="d1fef-153">The template's type.</span></span> <span data-ttu-id="d1fef-154">可能な値は、`securityBaseline`、`specializedDevices`、`advancedThreatProtectionSecurityBaseline`、`deviceConfiguration`、`custom` です。</span><span class="sxs-lookup"><span data-stu-id="d1fef-154">Possible values are: `securityBaseline`, `specializedDevices`, `advancedThreatProtectionSecurityBaseline`, `deviceConfiguration`, `custom`.</span></span>|
|<span data-ttu-id="d1fef-155">publishedDateTime</span><span class="sxs-lookup"><span data-stu-id="d1fef-155">publishedDateTime</span></span>|<span data-ttu-id="d1fef-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d1fef-156">DateTimeOffset</span></span>|<span data-ttu-id="d1fef-157">テンプレートが発行されたとき</span><span class="sxs-lookup"><span data-stu-id="d1fef-157">When the template was published</span></span>|



## <a name="response"></a><span data-ttu-id="d1fef-158">応答</span><span class="sxs-lookup"><span data-stu-id="d1fef-158">Response</span></span>
<span data-ttu-id="d1fef-159">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[devicemanagementtemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="d1fef-159">If successful, this method returns a `200 OK` response code and an updated [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d1fef-160">例</span><span class="sxs-lookup"><span data-stu-id="d1fef-160">Example</span></span>

### <a name="request"></a><span data-ttu-id="d1fef-161">要求</span><span class="sxs-lookup"><span data-stu-id="d1fef-161">Request</span></span>
<span data-ttu-id="d1fef-162">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="d1fef-162">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/templates/{deviceManagementTemplateId}
Content-type: application/json
Content-length: 334

{
  "@odata.type": "#microsoft.graph.deviceManagementTemplate",
  "displayName": "Display Name value",
  "description": "Description value",
  "versionInfo": "Version Info value",
  "isDeprecated": true,
  "intentCount": 11,
  "templateType": "specializedDevices",
  "publishedDateTime": "2016-12-31T23:58:16.1180489-08:00"
}
```

### <a name="response"></a><span data-ttu-id="d1fef-163">応答</span><span class="sxs-lookup"><span data-stu-id="d1fef-163">Response</span></span>
<span data-ttu-id="d1fef-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="d1fef-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 383

{
  "@odata.type": "#microsoft.graph.deviceManagementTemplate",
  "id": "edd764ca-64ca-edd7-ca64-d7edca64d7ed",
  "displayName": "Display Name value",
  "description": "Description value",
  "versionInfo": "Version Info value",
  "isDeprecated": true,
  "intentCount": 11,
  "templateType": "specializedDevices",
  "publishedDateTime": "2016-12-31T23:58:16.1180489-08:00"
}
```





