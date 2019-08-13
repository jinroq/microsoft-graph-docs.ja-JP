---
title: DeviceManagementTemplate の作成
description: 新しい deviceManagementTemplate オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 8df263e974037e747eb65169f6d305cef2b7b3b5
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36343133"
---
# <a name="create-devicemanagementtemplate"></a><span data-ttu-id="c07c3-103">DeviceManagementTemplate の作成</span><span class="sxs-lookup"><span data-stu-id="c07c3-103">Create deviceManagementTemplate</span></span>

> <span data-ttu-id="c07c3-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c07c3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c07c3-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="c07c3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c07c3-106">新しい[Devicemanagementtemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="c07c3-106">Create a new [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c07c3-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="c07c3-107">Prerequisites</span></span>
<span data-ttu-id="c07c3-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c07c3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c07c3-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c07c3-110">Permission type</span></span>|<span data-ttu-id="c07c3-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="c07c3-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c07c3-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c07c3-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c07c3-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c07c3-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c07c3-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c07c3-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c07c3-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c07c3-115">Not supported.</span></span>|
|<span data-ttu-id="c07c3-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c07c3-116">Application</span></span>|<span data-ttu-id="c07c3-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c07c3-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c07c3-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c07c3-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/templates
POST /deviceManagement/templates/{deviceManagementTemplateId}/migratableTo
```

## <a name="request-headers"></a><span data-ttu-id="c07c3-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c07c3-119">Request headers</span></span>
|<span data-ttu-id="c07c3-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c07c3-120">Header</span></span>|<span data-ttu-id="c07c3-121">値</span><span class="sxs-lookup"><span data-stu-id="c07c3-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c07c3-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c07c3-122">Authorization</span></span>|<span data-ttu-id="c07c3-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="c07c3-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c07c3-124">承諾</span><span class="sxs-lookup"><span data-stu-id="c07c3-124">Accept</span></span>|<span data-ttu-id="c07c3-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c07c3-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c07c3-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="c07c3-126">Request body</span></span>
<span data-ttu-id="c07c3-127">要求本文で、deviceManagementTemplate オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="c07c3-127">In the request body, supply a JSON representation for the deviceManagementTemplate object.</span></span>

<span data-ttu-id="c07c3-128">次の表に、deviceManagementTemplate の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="c07c3-128">The following table shows the properties that are required when you create the deviceManagementTemplate.</span></span>

|<span data-ttu-id="c07c3-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c07c3-129">Property</span></span>|<span data-ttu-id="c07c3-130">型</span><span class="sxs-lookup"><span data-stu-id="c07c3-130">Type</span></span>|<span data-ttu-id="c07c3-131">説明</span><span class="sxs-lookup"><span data-stu-id="c07c3-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c07c3-132">id</span><span class="sxs-lookup"><span data-stu-id="c07c3-132">id</span></span>|<span data-ttu-id="c07c3-133">文字列</span><span class="sxs-lookup"><span data-stu-id="c07c3-133">String</span></span>|<span data-ttu-id="c07c3-134">テンプレート ID</span><span class="sxs-lookup"><span data-stu-id="c07c3-134">The template ID</span></span>|
|<span data-ttu-id="c07c3-135">displayName</span><span class="sxs-lookup"><span data-stu-id="c07c3-135">displayName</span></span>|<span data-ttu-id="c07c3-136">String</span><span class="sxs-lookup"><span data-stu-id="c07c3-136">String</span></span>|<span data-ttu-id="c07c3-137">テンプレートの表示名</span><span class="sxs-lookup"><span data-stu-id="c07c3-137">The template's display name</span></span>|
|<span data-ttu-id="c07c3-138">description</span><span class="sxs-lookup"><span data-stu-id="c07c3-138">description</span></span>|<span data-ttu-id="c07c3-139">String</span><span class="sxs-lookup"><span data-stu-id="c07c3-139">String</span></span>|<span data-ttu-id="c07c3-140">テンプレートの説明</span><span class="sxs-lookup"><span data-stu-id="c07c3-140">The template's description</span></span>|
|<span data-ttu-id="c07c3-141">versionInfo</span><span class="sxs-lookup"><span data-stu-id="c07c3-141">versionInfo</span></span>|<span data-ttu-id="c07c3-142">String</span><span class="sxs-lookup"><span data-stu-id="c07c3-142">String</span></span>|<span data-ttu-id="c07c3-143">テンプレートのバージョン情報</span><span class="sxs-lookup"><span data-stu-id="c07c3-143">The template's version information</span></span>|
|<span data-ttu-id="c07c3-144">isDeprecated</span><span class="sxs-lookup"><span data-stu-id="c07c3-144">isDeprecated</span></span>|<span data-ttu-id="c07c3-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="c07c3-145">Boolean</span></span>|<span data-ttu-id="c07c3-146">テンプレートが非推奨になっているか、使用されていません。</span><span class="sxs-lookup"><span data-stu-id="c07c3-146">The template is deprecated or not.</span></span> <span data-ttu-id="c07c3-147">推奨されていないテンプレートからは、インテントを作成できません。</span><span class="sxs-lookup"><span data-stu-id="c07c3-147">Intents cannot be created from a deprecated template.</span></span>|
|<span data-ttu-id="c07c3-148">intentCount</span><span class="sxs-lookup"><span data-stu-id="c07c3-148">intentCount</span></span>|<span data-ttu-id="c07c3-149">Int32</span><span class="sxs-lookup"><span data-stu-id="c07c3-149">Int32</span></span>|<span data-ttu-id="c07c3-150">このテンプレートから作成されたインテントの数。</span><span class="sxs-lookup"><span data-stu-id="c07c3-150">Number of Intents created from this template.</span></span>|
|<span data-ttu-id="c07c3-151">templateType</span><span class="sxs-lookup"><span data-stu-id="c07c3-151">templateType</span></span>|[<span data-ttu-id="c07c3-152">deviceManagementTemplateType</span><span class="sxs-lookup"><span data-stu-id="c07c3-152">deviceManagementTemplateType</span></span>](../resources/intune-deviceintent-devicemanagementtemplatetype.md)|<span data-ttu-id="c07c3-153">テンプレートの種類を示します。</span><span class="sxs-lookup"><span data-stu-id="c07c3-153">The template's type.</span></span> <span data-ttu-id="c07c3-154">可能な値は、`securityBaseline`、`specializedDevices`、`advancedThreatProtectionSecurityBaseline`、`deviceConfiguration`、`custom` です。</span><span class="sxs-lookup"><span data-stu-id="c07c3-154">Possible values are: `securityBaseline`, `specializedDevices`, `advancedThreatProtectionSecurityBaseline`, `deviceConfiguration`, `custom`.</span></span>|
|<span data-ttu-id="c07c3-155">publishedDateTime</span><span class="sxs-lookup"><span data-stu-id="c07c3-155">publishedDateTime</span></span>|<span data-ttu-id="c07c3-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c07c3-156">DateTimeOffset</span></span>|<span data-ttu-id="c07c3-157">テンプレートが発行されたとき</span><span class="sxs-lookup"><span data-stu-id="c07c3-157">When the template was published</span></span>|



## <a name="response"></a><span data-ttu-id="c07c3-158">応答</span><span class="sxs-lookup"><span data-stu-id="c07c3-158">Response</span></span>
<span data-ttu-id="c07c3-159">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[devicemanagementtemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="c07c3-159">If successful, this method returns a `201 Created` response code and a [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c07c3-160">例</span><span class="sxs-lookup"><span data-stu-id="c07c3-160">Example</span></span>

### <a name="request"></a><span data-ttu-id="c07c3-161">要求</span><span class="sxs-lookup"><span data-stu-id="c07c3-161">Request</span></span>
<span data-ttu-id="c07c3-162">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="c07c3-162">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/templates
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

### <a name="response"></a><span data-ttu-id="c07c3-163">応答</span><span class="sxs-lookup"><span data-stu-id="c07c3-163">Response</span></span>
<span data-ttu-id="c07c3-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="c07c3-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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






