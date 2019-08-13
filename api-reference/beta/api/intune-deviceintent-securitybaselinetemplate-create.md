---
title: SecurityBaselineTemplate を作成する
description: 新しい securityBaselineTemplate オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b5e7c073d59474d41ccd46534c0c4f6b1bb0ba16
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36349027"
---
# <a name="create-securitybaselinetemplate"></a><span data-ttu-id="3ffee-103">SecurityBaselineTemplate を作成する</span><span class="sxs-lookup"><span data-stu-id="3ffee-103">Create securityBaselineTemplate</span></span>

> <span data-ttu-id="3ffee-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3ffee-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3ffee-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="3ffee-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3ffee-106">新しい[securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="3ffee-106">Create a new [securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3ffee-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="3ffee-107">Prerequisites</span></span>
<span data-ttu-id="3ffee-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3ffee-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3ffee-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="3ffee-110">Permission type</span></span>|<span data-ttu-id="3ffee-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="3ffee-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3ffee-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="3ffee-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3ffee-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3ffee-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3ffee-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="3ffee-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3ffee-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3ffee-115">Not supported.</span></span>|
|<span data-ttu-id="3ffee-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="3ffee-116">Application</span></span>|<span data-ttu-id="3ffee-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3ffee-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3ffee-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="3ffee-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/templates
POST /deviceManagement/templates/{deviceManagementTemplateId}/migratableTo
```

## <a name="request-headers"></a><span data-ttu-id="3ffee-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3ffee-119">Request headers</span></span>
|<span data-ttu-id="3ffee-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3ffee-120">Header</span></span>|<span data-ttu-id="3ffee-121">値</span><span class="sxs-lookup"><span data-stu-id="3ffee-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3ffee-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="3ffee-122">Authorization</span></span>|<span data-ttu-id="3ffee-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="3ffee-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3ffee-124">承諾</span><span class="sxs-lookup"><span data-stu-id="3ffee-124">Accept</span></span>|<span data-ttu-id="3ffee-125">application/json</span><span class="sxs-lookup"><span data-stu-id="3ffee-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3ffee-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="3ffee-126">Request body</span></span>
<span data-ttu-id="3ffee-127">要求本文で、securityBaselineTemplate オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="3ffee-127">In the request body, supply a JSON representation for the securityBaselineTemplate object.</span></span>

<span data-ttu-id="3ffee-128">次の表に、securityBaselineTemplate の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="3ffee-128">The following table shows the properties that are required when you create the securityBaselineTemplate.</span></span>

|<span data-ttu-id="3ffee-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3ffee-129">Property</span></span>|<span data-ttu-id="3ffee-130">型</span><span class="sxs-lookup"><span data-stu-id="3ffee-130">Type</span></span>|<span data-ttu-id="3ffee-131">説明</span><span class="sxs-lookup"><span data-stu-id="3ffee-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3ffee-132">id</span><span class="sxs-lookup"><span data-stu-id="3ffee-132">id</span></span>|<span data-ttu-id="3ffee-133">文字列</span><span class="sxs-lookup"><span data-stu-id="3ffee-133">String</span></span>|<span data-ttu-id="3ffee-134">[Devicemanagementtemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)から継承されたテンプレート ID</span><span class="sxs-lookup"><span data-stu-id="3ffee-134">The template ID Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|
|<span data-ttu-id="3ffee-135">displayName</span><span class="sxs-lookup"><span data-stu-id="3ffee-135">displayName</span></span>|<span data-ttu-id="3ffee-136">String</span><span class="sxs-lookup"><span data-stu-id="3ffee-136">String</span></span>|<span data-ttu-id="3ffee-137">[Devicemanagementtemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)から継承されたテンプレートの表示名</span><span class="sxs-lookup"><span data-stu-id="3ffee-137">The template's display name Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|
|<span data-ttu-id="3ffee-138">description</span><span class="sxs-lookup"><span data-stu-id="3ffee-138">description</span></span>|<span data-ttu-id="3ffee-139">String</span><span class="sxs-lookup"><span data-stu-id="3ffee-139">String</span></span>|<span data-ttu-id="3ffee-140">[Devicemanagementtemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)から継承されるテンプレートの説明</span><span class="sxs-lookup"><span data-stu-id="3ffee-140">The template's description Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|
|<span data-ttu-id="3ffee-141">versionInfo</span><span class="sxs-lookup"><span data-stu-id="3ffee-141">versionInfo</span></span>|<span data-ttu-id="3ffee-142">String</span><span class="sxs-lookup"><span data-stu-id="3ffee-142">String</span></span>|<span data-ttu-id="3ffee-143">[Devicemanagementtemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)から継承されたテンプレートのバージョン情報</span><span class="sxs-lookup"><span data-stu-id="3ffee-143">The template's version information Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|
|<span data-ttu-id="3ffee-144">isDeprecated</span><span class="sxs-lookup"><span data-stu-id="3ffee-144">isDeprecated</span></span>|<span data-ttu-id="3ffee-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="3ffee-145">Boolean</span></span>|<span data-ttu-id="3ffee-146">テンプレートが非推奨になっているか、使用されていません。</span><span class="sxs-lookup"><span data-stu-id="3ffee-146">The template is deprecated or not.</span></span> <span data-ttu-id="3ffee-147">推奨されていないテンプレートからは、インテントを作成できません。</span><span class="sxs-lookup"><span data-stu-id="3ffee-147">Intents cannot be created from a deprecated template.</span></span> <span data-ttu-id="3ffee-148">[Devicemanagementtemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="3ffee-148">Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|
|<span data-ttu-id="3ffee-149">intentCount</span><span class="sxs-lookup"><span data-stu-id="3ffee-149">intentCount</span></span>|<span data-ttu-id="3ffee-150">Int32</span><span class="sxs-lookup"><span data-stu-id="3ffee-150">Int32</span></span>|<span data-ttu-id="3ffee-151">このテンプレートから作成されたインテントの数。</span><span class="sxs-lookup"><span data-stu-id="3ffee-151">Number of Intents created from this template.</span></span> <span data-ttu-id="3ffee-152">[Devicemanagementtemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="3ffee-152">Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|
|<span data-ttu-id="3ffee-153">templateType</span><span class="sxs-lookup"><span data-stu-id="3ffee-153">templateType</span></span>|[<span data-ttu-id="3ffee-154">deviceManagementTemplateType</span><span class="sxs-lookup"><span data-stu-id="3ffee-154">deviceManagementTemplateType</span></span>](../resources/intune-deviceintent-devicemanagementtemplatetype.md)|<span data-ttu-id="3ffee-155">テンプレートの種類を示します。</span><span class="sxs-lookup"><span data-stu-id="3ffee-155">The template's type.</span></span> <span data-ttu-id="3ffee-156">[Devicemanagementtemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="3ffee-156">Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md).</span></span> <span data-ttu-id="3ffee-157">可能な値は、`securityBaseline`、`specializedDevices`、`advancedThreatProtectionSecurityBaseline`、`deviceConfiguration`、`custom` です。</span><span class="sxs-lookup"><span data-stu-id="3ffee-157">Possible values are: `securityBaseline`, `specializedDevices`, `advancedThreatProtectionSecurityBaseline`, `deviceConfiguration`, `custom`.</span></span>|
|<span data-ttu-id="3ffee-158">publishedDateTime</span><span class="sxs-lookup"><span data-stu-id="3ffee-158">publishedDateTime</span></span>|<span data-ttu-id="3ffee-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3ffee-159">DateTimeOffset</span></span>|<span data-ttu-id="3ffee-160">テンプレートが公開された場合 ( [Devicemanagementtemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)から継承)</span><span class="sxs-lookup"><span data-stu-id="3ffee-160">When the template was published Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|



## <a name="response"></a><span data-ttu-id="3ffee-161">応答</span><span class="sxs-lookup"><span data-stu-id="3ffee-161">Response</span></span>
<span data-ttu-id="3ffee-162">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="3ffee-162">If successful, this method returns a `201 Created` response code and a [securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3ffee-163">例</span><span class="sxs-lookup"><span data-stu-id="3ffee-163">Example</span></span>

### <a name="request"></a><span data-ttu-id="3ffee-164">要求</span><span class="sxs-lookup"><span data-stu-id="3ffee-164">Request</span></span>
<span data-ttu-id="3ffee-165">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="3ffee-165">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/templates
Content-type: application/json
Content-length: 334

{
  "@odata.type": "#microsoft.graph.securityBaselineTemplate",
  "displayName": "Display Name value",
  "description": "Description value",
  "versionInfo": "Version Info value",
  "isDeprecated": true,
  "intentCount": 11,
  "templateType": "specializedDevices",
  "publishedDateTime": "2016-12-31T23:58:16.1180489-08:00"
}
```

### <a name="response"></a><span data-ttu-id="3ffee-166">応答</span><span class="sxs-lookup"><span data-stu-id="3ffee-166">Response</span></span>
<span data-ttu-id="3ffee-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="3ffee-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 383

{
  "@odata.type": "#microsoft.graph.securityBaselineTemplate",
  "id": "3f61d4c2-d4c2-3f61-c2d4-613fc2d4613f",
  "displayName": "Display Name value",
  "description": "Description value",
  "versionInfo": "Version Info value",
  "isDeprecated": true,
  "intentCount": 11,
  "templateType": "specializedDevices",
  "publishedDateTime": "2016-12-31T23:58:16.1180489-08:00"
}
```






